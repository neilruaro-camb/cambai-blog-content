# Webflow Implementation Checklist

Step-by-step checklist for implementing the technical SEO/GEO changes on the camb.ai Webflow site.

---

## Phase 1: Site-Wide Changes (Week 1)

### robots.txt
- [ ] Go to **Site Settings > SEO > Robots.txt**
- [ ] Replace current robots.txt with contents of `robots.txt` in this directory
- [ ] Publish and verify at https://www.camb.ai/robots.txt
- [ ] Test with Google's robots.txt tester in Search Console

### Site-Wide Custom Head Code
- [ ] Go to **Site Settings > Custom Code > Head Code**
- [ ] Paste contents of `webflow-custom-head-code.html`
- [ ] This adds: Twitter Card defaults, Organization schema, WebSite schema, preconnect hints
- [ ] Publish and verify with Google Rich Results Test

### Canonical URLs
- [ ] For each page in **Pages panel > Page Settings**:
  - [ ] Set the canonical URL to the page's own URL
  - [ ] Format: `https://www.camb.ai/[page-path]`
  - [ ] Do NOT include trailing slashes (unless Webflow adds them)

---

## Phase 2: Per-Page Meta Tags (Week 1-2)

Reference: `meta-tags/all-pages-meta-tags.md`

### Core Pages
- [ ] **Homepage** — Update title, description, OG tags per the spec
- [ ] **Mars** — Update title, description, OG tags
- [ ] **Streams** — Update title, description, OG tags
- [ ] **Blog listing** — Update title, description, OG tags
- [ ] **Pricing** — Update title, description, OG tags
- [ ] **About** — Update title, description, OG tags
- [ ] **Events** — Update title, description, OG tags
- [ ] **Contact** — Update title, description, OG tags

### CMS Templates (Blog Posts)
- [ ] Go to **CMS > Blog Post template settings**
- [ ] Set dynamic title: `{Post Title} | CAMB.AI Blog`
- [ ] Set dynamic meta description using the post's meta description field
- [ ] Set dynamic OG image using the post's featured image
- [ ] Ensure canonical URL is set dynamically

### CMS Templates (Translation Pages)
- [ ] Go to **CMS > Translation Page template settings**
- [ ] Fix title bug: ensure format is "Free [Source] to [Target] AI Translator | CAMB.AI"
  - NOT "Free [Source] to [Source] to [Target]"
- [ ] Set dynamic meta description
- [ ] Set dynamic canonical URL

---

## Phase 3: Schema Markup (Week 2-3)

Reference: `schema-markup/IMPLEMENTATION-GUIDE.md`

### Blog Post CMS Template
- [ ] Add Custom Code Embed element in blog post template
- [ ] Paste `blog-post-template.json` wrapped in `<script type="application/ld+json">`
- [ ] Replace placeholders with Webflow CMS field references
- [ ] Test with Google Rich Results Test on a published post

### Translation Page CMS Template
- [ ] Add Custom Code Embed element in translation page template
- [ ] Paste `translation-page-template.json` wrapped in `<script type="application/ld+json">`
- [ ] Replace placeholders with CMS field references
- [ ] Test with Rich Results Test

### Blog Listing Page
- [ ] Add Custom Code Embed to /blog page
- [ ] Paste `blog-listing-collection.json`
- [ ] Test

### Product Pages (Mars, Streams)
- [ ] Add Custom Code to Mars page head section
- [ ] Paste customized `product-page-template.json`
- [ ] Repeat for Streams
- [ ] Test both

### Events Pages (if CMS-based)
- [ ] Add Custom Code Embed to event template
- [ ] Paste `event-template.json` with dynamic CMS references
- [ ] Test

---

## Phase 4: Image Alt Text Audit (Week 2)

- [ ] **Homepage**: Audit all images, add descriptive alt text
  - Hero image: describe what's shown + "CAMB.AI AI dubbing platform"
  - Client logos: "IMAX logo — CAMB.AI customer," "Australian Open logo — CAMB.AI partner," etc.
  - Feature images: describe the feature shown
  - Team photos: "[Name], [Title] at CAMB.AI"
- [ ] **Product pages**: Alt text for all screenshots and feature images
- [ ] **Blog posts**: Audit top 20 posts, add alt text to all images
  - Charts/graphs: describe the data shown
  - Screenshots: describe what's on screen
  - Stock photos: describe contextually
- [ ] **Translation pages**: Alt text for any images (if present)

---

## Phase 5: Translation Page Fixes (Week 3-4)

- [ ] **Fix title bug**: "Free English to English to Spanish" → "Free English to Spanish"
  - Check CMS template for double language insertion
  - Fix the dynamic field reference
- [ ] **Reduce keyword stuffing**: Review translation page template
  - Reduce repetition of "[Source] to [Target]" in body copy
  - Replace some instances with synonyms: "translate between X and Y," "X-Y language pair"
- [ ] **Add FAQ section**: to translation page CMS template
  - 3 questions per page (can be dynamic via CMS or templated)
- [ ] **Add unique content field**: to translation CMS collection
  - Field for language-pair-specific content (cultural context, common uses)
  - Start populating for top 30 language pairs

---

## Phase 6: Blog Infrastructure (Week 3-4)

- [ ] **Add categories**: Create CMS collection "Blog Categories"
  - AI Dubbing, Voice Cloning, TTS, Localization, Case Studies, Product Updates, Industry Guides
  - Link each blog post to a category
- [ ] **Add author pages**: Create CMS collection "Authors" with bios
  - Link each post to an author
  - Create author template page with bio, photo, credentials
- [ ] **Add "Related Posts"**: section to blog post template
  - Use Webflow CMS multi-reference field or conditional visibility
- [ ] **Add reading time**: Calculate and display on each post
  - Formula: word count ÷ 200 = minutes
- [ ] **Add dates**: Ensure publish date and "last updated" date are visible on every post

---

## Phase 7: New Page Types (Weeks 5+)

### Comparison Pages (/compare/*)
- [ ] Create CMS collection "Comparisons" or build as static pages
- [ ] Follow template in `templates/comparison-pages/`
- [ ] Add schema from `schema-markup/comparison-page-template.json`
- [ ] Start with: CAMB.AI vs ElevenLabs, CAMB.AI vs Rask AI, CAMB.AI vs HeyGen

### Case Study Pages (/case-studies/*)
- [ ] Create CMS collection "Case Studies" or build as static pages
- [ ] Follow template in `templates/case-studies/`
- [ ] Add schema from `schema-markup/case-study-template.json`
- [ ] Start with: Australian Open, IMAX, MLB

### Industry Solution Pages (/solutions/*)
- [ ] Create pages following `templates/industry-verticals/`
- [ ] Start with: Sports Broadcasting, Entertainment Studios, E-Learning

### Regional Pages (/regions/*)
- [ ] Create pages following `templates/regional-pages/`
- [ ] Start with: India, Asia-Pacific

---

## Validation & Monitoring

### After each change:
- [ ] Test with [Google Rich Results Test](https://search.google.com/test/rich-results)
- [ ] Check [Google PageSpeed Insights](https://pagespeed.web.dev/) (target: all green)
- [ ] Validate schema at [Schema.org Validator](https://validator.schema.org/)

### Ongoing:
- [ ] Submit updated sitemap to Google Search Console
- [ ] Submit sitemap to Bing Webmaster Tools
- [ ] Monitor Search Console for schema errors (Enhancements tab)
- [ ] Monitor Core Web Vitals in Search Console
- [ ] Weekly GEO citation monitoring (see GEO guide)
