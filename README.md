# Skintillate Skin Clinic website

Website for Dr. Kiruthika's Skintillate Skin Clinic, Salem. The site is published at https://skintillate.co.in/.

It's a static site built with [Jekyll](https://jekyllrb.com/). GitHub Pages builds it automatically on every push to `main`, so there's no build step to run and no server to manage.

## Where things live

| What | Where |
|---|---|
| Clinic name, phone, address, hours, map links, doctor's registration | `_data/clinic.yml` |
| List of treatments: names, short blurbs, URL slugs, groups | `_data/services.yml` |
| Interface text: menu, buttons, footer, address lines | `_data/i18n/en.yml` |
| Home, doctor, clinic, contact pages | `index.html`, `dr-kiruthika.html`, `clinic.html`, `contact.html` |
| Treatment pages (one per treatment) | `services/*.md` |
| Page templates | `_layouts/`, `_includes/` |
| Styles | `assets/css/main.css` |
| Optimised images, icons, social-share image | `assets/img/` |

**Changing the phone number, hours or address:** edit `_data/clinic.yml` and the address lines in `_data/i18n/en.yml`. Every page, the footer and the structured data for Google update together. Keep them identical to the Google Business Profile.

**Editing a treatment page:** open the file in `services/`. The front matter (between the `---` lines) holds the SEO title, meta description, intro, FAQs and related treatments. The body below it is ordinary Markdown.

**Content rules:**
- No prices, price ranges or words like "cheap", "affordable" or "nominal cost".
- No superlatives such as "best" or "No. 1".
- No guaranteed results.
- No patient testimonials or before/after claims.

## Medical review

Every treatment page has `last_reviewed:` in its front matter. Once Dr. Kiruthika has approved a page, set it to the date, e.g. `last_reviewed: 2026-10-20`. The page then shows "Medically reviewed by Dr. Kiruthika S." and tells Google the same through structured data. See `CONTENT-REVIEW.md` for the checklist.

## Preview locally (optional)

Local builds need Ruby 3.x. Ruby 4 is not yet supported by the GitHub Pages gem.

```sh
brew install ruby@3.3
export PATH="/opt/homebrew/opt/ruby@3.3/bin:$PATH"
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Adding Tamil (or another language)

The site is set up for this already; nothing needs to change in the templates.

1. Copy `_data/i18n/en.yml` to `_data/i18n/ta.yml` and translate the values. Set `hreflang: ta-IN`, `og_locale: ta_IN` and `language_name: தமிழ்`.
2. Create translated pages under `ta/` using the same structure: `ta/index.html`, `ta/services/acne-scar-treatment.md`, and so on. Give each page the same `ref` as its English version. Links inside pages should start with `/ta/`.
3. Add the Tamil `name` and `blurb` for each treatment in `_data/services.yml` under a `ta:` key.
4. Add a Tamil font (e.g. Noto Sans Tamil) to the font link in `_includes/head.html`.

Once a translated page exists, its English and Tamil versions automatically get:
- hreflang tags
- a language switcher in the header
- alternate links in `sitemap.xml`

Pages that haven't been translated yet never link to a missing page.

## After launch

- Verify the site in [Google Search Console](https://search.google.com/search-console) and submit `https://skintillate.co.in/sitemap.xml`.
- Add the website link to the Google Business Profile and the Instagram bio.
- Check each page with Google's [Rich Results Test](https://search.google.com/test/rich-results) and [PageSpeed Insights](https://pagespeed.web.dev/).
