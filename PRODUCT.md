# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Primary: a local patient in Salem or nearby, usually on a phone, looking for a dermatologist or a specific skin, hair or laser treatment. They want to confirm the clinic is legitimate, see hours and location, and book by WhatsApp or phone. Secondary (inferred from the service pages, not separately confirmed): a patient reading a treatment page to understand it before deciding.

## Product Purpose

Website for Dr. Kiruthika's Skintillate Skin Clinic, Salem (https://skintillate.co.in/). It helps local patients find the clinic, understand its treatments and contact it. Success is a WhatsApp message or phone call to +91 77088 74297 (WhatsApp and phone are the same number).

## Positioning

Doctor-led, personal care: Dr. Kiruthika (TNMC Reg. No. 117795) sees and treats patients herself, and the clinic is her own practice.

## Operating Context

- Static Jekyll site built by GitHub Pages on push to `main`; custom domain via GoDaddy DNS.
- Clinic data lives in `_data/clinic.yml`, treatments in `_data/services.yml`, interface text in `_data/i18n/en.yml`.
- Address (use exactly): No: 54, Srinivasa Complex, Nagaramalai Main Road, Dhurpathi Amman Kovil Opposite, North Alagapuram, Salem - 636 016.
- Hours: Mon–Sat 11AM–7PM, Sunday closed.
- Treatment pages are drafted by Claude and reviewed by Dr. Kiruthika (`last_reviewed:` front matter; checklist in `CONTENT-REVIEW.md`).

## Capabilities and Constraints

- English at the root now; Tamil later under `/ta/`. The architecture must support it (hreflang, language switcher, per-language data).
- Lasers are fractional CO2 and diode only. Never mention Q-switched Nd:YAG. Other services: peels, microneedling, subcision, HydraFacial and other aesthetic work.
- Never mention prices, price ranges or `priceRange` in schema. Avoid words like "cheap", "affordable", "nominal cost".
- Indian NMC advertising rules apply: no superlatives, guaranteed results, patient testimonials or before/after claims.
- SEO and AI-search visibility are a core goal (schema.org, `llms.txt`, sitemap, off-site profile links).
- Performance matters: GA4 is deferred until interaction or 5s after load.

## Brand Commitments

Name: "Dr. Kiruthika's Skintillate Skin Clinic". Design direction was a refresh of the original carrd.co site, not a 1:1 copy.

## Evidence on Hand

Doctor registration (TNMC 117795), clinic address and geo coordinates (11.6772035, 78.1390042), Instagram, Practo and Justdial listings. No testimonials, case studies, prices or press; none may be invented.

## Product Principles

1. Contact is one tap away: WhatsApp and call are always reachable on mobile.
2. Trust comes from facts (registration, address, hours, medical review), never from claims or superlatives.
3. Plain, calm, informative copy that respects medical-advertising rules.
4. Every page and schema block is checked against the content rules before publishing.
5. Bilingual from the start; nothing hard-coded to English.

## Accessibility & Inclusion

Patients include non-English readers (Tamil support planned) and users on low-end phones and slow connections; keep pages light and text readable.
