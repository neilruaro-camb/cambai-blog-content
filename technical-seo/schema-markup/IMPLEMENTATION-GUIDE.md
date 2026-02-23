# Schema Markup Implementation Guide for Webflow

## Overview

This directory contains JSON-LD structured data templates for every page type on camb.ai. JSON-LD is Google's recommended format for structured data and is the easiest to implement in Webflow.

## How to Add JSON-LD in Webflow

### Option 1: Per-Page Custom Code (Recommended for unique pages)
1. Go to **Pages panel** in Webflow Designer
2. Click the **gear icon** on the target page
3. Scroll to **Custom Code > Before </head> tag**
4. Paste the JSON-LD wrapped in a `<script>` tag:

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "CAMB.AI",
  ...
}
</script>
```

### Option 2: Site-Wide Custom Code (For Organization + WebSite schema)
1. Go to **Site Settings > Custom Code > Head Code**
2. Paste the Organization and WebSite schema (these should appear on every page)

### Option 3: Webflow CMS + Embed Block (For blog posts, translation pages)
1. Create a **Custom Code Embed** element in your CMS template
2. Use CMS field references to dynamically populate JSON-LD fields
3. Example with Webflow CMS fields:

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BlogPosting",
  "headline": "{{wf {&quot;path&quot;:&quot;name&quot;,&quot;type&quot;:&quot;PlainText&quot;} }}",
  "datePublished": "{{wf {&quot;path&quot;:&quot;published-date&quot;,&quot;type&quot;:&quot;Date&quot;} }}",
  ...
}
</script>
```

## Files in This Directory

| File | Use On | Priority |
|------|--------|----------|
| `homepage-organization.json` | Homepage (site-wide OK) | Critical |
| `homepage-website.json` | Homepage (site-wide OK) | Critical |
| `blog-listing-collection.json` | /blog page | High |
| `blog-post-template.json` | Every /blog-post/* page | Critical |
| `translation-page-template.json` | Every /translate/* page | High |
| `product-page-template.json` | /mars, /streams | High |
| `event-template.json` | /events/* pages | Medium |
| `comparison-page-template.json` | /compare/* pages (new) | High |
| `case-study-template.json` | /case-studies/* pages (new) | High |

## Implementation Order

1. **Week 1**: Add Organization + WebSite schema site-wide (homepage files)
2. **Week 1**: Add BlogPosting + FAQPage schema to blog post CMS template
3. **Week 2**: Add CollectionPage schema to blog listing page
4. **Week 2**: Add SoftwareApplication schema to translation page CMS template
5. **Week 3**: Add Product schema to Mars and Streams pages
6. **Week 3**: Add Event schema to events pages
7. **As created**: Add comparison, case study schemas to new pages

## Validation

After adding any schema, validate using:
- **Google Rich Results Test**: https://search.google.com/test/rich-results
- **Schema.org Validator**: https://validator.schema.org/
- **Google Search Console**: Monitor "Enhancements" tab for schema errors

## Common Webflow Gotchas

1. **Escape quotes**: In Webflow CMS embed blocks, use `&quot;` for quotes inside JSON strings
2. **Date format**: Ensure dates are ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
3. **Image URLs**: Use full absolute URLs (https://www.camb.ai/...), not relative paths
4. **Testing**: After publishing, allow 24-48 hours for Google to pick up new schema
5. **Multiple schemas**: You can combine multiple schemas in one `<script>` tag using `@graph`
