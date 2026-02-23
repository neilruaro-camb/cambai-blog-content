# camb.ai SEO/GEO Implementation Kit

Comprehensive SEO and GEO (Generative Engine Optimization) assets for camb.ai's Webflow website.

## Directory Structure

```
cambai-blog/
├── README.md                          ← You are here
│
├── plan/
│   └── SEO-GEO-PLAN.md               ← Full strategic plan (7 sections, 24-week roadmap)
│
├── technical-seo/
│   ├── robots.txt                     ← Ready-to-deploy robots.txt (allows all AI crawlers)
│   ├── webflow-custom-head-code.html  ← Site-wide <head> code (schemas, Twitter Cards)
│   ├── WEBFLOW-IMPLEMENTATION-CHECKLIST.md  ← Step-by-step Webflow implementation guide
│   ├── sitemap-index.xml              ← Sitemap index (splits into sub-sitemaps)
│   ├── sitemap-pages.xml              ← Core pages sitemap (priority 0.8-1.0)
│   ├── sitemap-blog.xml               ← Blog posts sitemap (priority 0.7-0.8)
│   ├── sitemap-translate.xml          ← Translation pages sitemap (priority 0.4-0.6)
│   ├── schema-markup/
│   │   ├── IMPLEMENTATION-GUIDE.md    ← How to add JSON-LD in Webflow
│   │   ├── homepage-organization.json ← Organization schema (site-wide)
│   │   ├── homepage-website.json      ← WebSite schema (site-wide)
│   │   ├── blog-listing-collection.json  ← CollectionPage for /blog
│   │   ├── blog-post-template.json    ← BlogPosting + FAQPage + Breadcrumb
│   │   ├── translation-page-template.json  ← SoftwareApplication + FAQ
│   │   ├── product-page-template.json ← Product schema for Mars/Streams
│   │   ├── event-template.json        ← Event schema
│   │   ├── comparison-page-template.json  ← WebPage + FAQ for /compare/
│   │   └── case-study-template.json   ← Article + Breadcrumb for /case-studies/
│   └── meta-tags/
│       └── all-pages-meta-tags.md     ← Title, description, OG tags for every page type
│
├── templates/
│   ├── GEO-CONTENT-OPTIMIZATION-GUIDE.md  ← Princeton GEO methods + platform strategies
│   ├── blog-posts/
│   │   └── GEO-OPTIMIZED-BLOG-TEMPLATE.md  ← Universal blog post template
│   ├── comparison-pages/
│   │   └── COMPARISON-PAGE-TEMPLATE.md     ← Template for /compare/ pages
│   ├── case-studies/
│   │   └── CASE-STUDY-TEMPLATE.md          ← Template for /case-studies/ pages
│   ├── industry-verticals/
│   │   └── INDUSTRY-VERTICAL-TEMPLATE.md   ← Template for /solutions/ pages
│   └── regional-pages/
│       └── REGIONAL-LANDING-TEMPLATE.md    ← Template for /regions/ pages
│
└── content-outlines/
    ├── PRIORITY-BLOG-POST-OUTLINES.md      ← 10 high-priority blog post outlines
    ├── comparisons/
    │   └── ALL-COMPARISON-OUTLINES.md      ← 7 comparison + 3 alternative page outlines
    ├── verticals/
    │   └── ALL-VERTICAL-OUTLINES.md        ← 9 industry vertical page outlines
    ├── case-studies/
    │   └── ALL-CASE-STUDY-OUTLINES.md      ← 5 customer case study outlines
    └── regional/
        └── ALL-REGIONAL-OUTLINES.md        ← 5 regional landing page outlines
```

## Quick Start

### 1. Technical SEO (Do First)
1. Deploy `technical-seo/robots.txt` → Webflow Site Settings > SEO
2. Add `technical-seo/webflow-custom-head-code.html` → Site Settings > Custom Code > Head
3. Update meta tags for all pages per `technical-seo/meta-tags/all-pages-meta-tags.md`
4. Add schema markup per `technical-seo/schema-markup/IMPLEMENTATION-GUIDE.md`
5. Follow the full checklist: `technical-seo/WEBFLOW-IMPLEMENTATION-CHECKLIST.md`

### 2. Content Creation (Use Templates)
1. Read `templates/GEO-CONTENT-OPTIMIZATION-GUIDE.md` for GEO best practices
2. Use the relevant template from `templates/` for each new page type
3. Reference `content-outlines/` for specific page outlines and talking points

### 3. Track Progress
Follow the phased roadmap in `plan/SEO-GEO-PLAN.md` (Section 7).

## Key Files to Start With

| Priority | File | What It Does |
|----------|------|-------------|
| 1 | `technical-seo/robots.txt` | Allows AI crawlers (GPTBot, ClaudeBot, etc.) |
| 2 | `technical-seo/webflow-custom-head-code.html` | Adds Organization + WebSite schema site-wide |
| 3 | `technical-seo/meta-tags/all-pages-meta-tags.md` | Title + meta description for every page |
| 4 | `technical-seo/schema-markup/blog-post-template.json` | BlogPosting + FAQ schema for blog CMS |
| 5 | `templates/GEO-CONTENT-OPTIMIZATION-GUIDE.md` | How to write GEO-optimized content |
| 6 | `content-outlines/comparisons/ALL-COMPARISON-OUTLINES.md` | High-impact comparison pages to create |
