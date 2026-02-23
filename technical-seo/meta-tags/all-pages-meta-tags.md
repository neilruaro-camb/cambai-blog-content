# Meta Tags Configuration for All camb.ai Pages

## How to Implement in Webflow

### Per-Page Meta Tags
In Webflow, go to **Pages panel > Page Settings** for each page and fill in:
- **Title Tag** — paste the `<title>` value
- **Meta Description** — paste the `<meta name="description">` value
- **Open Graph Title** — paste the OG title
- **Open Graph Description** — paste the OG description
- **Open Graph Image** — upload the OG image (1200x630px recommended)
- **Canonical URL** — set under "SEO Settings" (self-referencing)

### Site-Wide Twitter Cards
In Webflow, go to **Site Settings > Custom Code > Head Code** and add:
```html
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:site" content="@camaborai">
```

---

## Homepage: camb.ai

```html
<title>CAMB.AI — AI Dubbing & Voice Translation in 150+ Languages</title>
<meta name="description" content="CAMB.AI is the leading AI dubbing and voice translation platform. Translate audio, video, and text across 150+ languages. Trusted by IMAX, Australian Open, and MLB.">
<link rel="canonical" href="https://www.camb.ai/">

<!-- Open Graph -->
<meta property="og:type" content="website">
<meta property="og:title" content="CAMB.AI — AI Dubbing & Voice Translation in 150+ Languages">
<meta property="og:description" content="Translate audio, video, and text across 150+ languages with AI. Trusted by IMAX, Australian Open, and MLB.">
<meta property="og:url" content="https://www.camb.ai/">
<meta property="og:image" content="https://www.camb.ai/images/og-homepage.png">
<meta property="og:site_name" content="CAMB.AI">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:site" content="@camaborai">
<meta name="twitter:title" content="CAMB.AI — AI Dubbing & Voice Translation in 150+ Languages">
<meta name="twitter:description" content="Translate audio, video, and text across 150+ languages with AI. Trusted by IMAX, Australian Open, and MLB.">
<meta name="twitter:image" content="https://www.camb.ai/images/og-homepage.png">
```

---

## Mars (Product Page)

```html
<title>CAMB.AI Mars — AI Dubbing Platform for Video & Audio</title>
<meta name="description" content="Mars by CAMB.AI: upload video or audio and get AI-dubbed content in 150+ languages. Professional-quality dubbing with voice cloning and lip sync.">
<link rel="canonical" href="https://www.camb.ai/mars">

<meta property="og:type" content="product">
<meta property="og:title" content="CAMB.AI Mars — AI Dubbing Platform for Video & Audio">
<meta property="og:description" content="Upload video or audio, get AI-dubbed content in 150+ languages. Professional-quality dubbing with voice cloning.">
<meta property="og:url" content="https://www.camb.ai/mars">
<meta property="og:image" content="https://www.camb.ai/images/og-mars.png">
```

---

## Streams (Product Page)

```html
<title>CAMB.AI Streams — Real-Time AI Translation & Dubbing API</title>
<meta name="description" content="Streams by CAMB.AI: real-time AI translation and dubbing API for live events, broadcasts, and streaming. Sub-second latency in 150+ languages.">
<link rel="canonical" href="https://www.camb.ai/streams">

<meta property="og:type" content="product">
<meta property="og:title" content="CAMB.AI Streams — Real-Time AI Translation & Dubbing API">
<meta property="og:description" content="Real-time AI translation and dubbing API for live events and streaming. Sub-second latency in 150+ languages.">
<meta property="og:url" content="https://www.camb.ai/streams">
<meta property="og:image" content="https://www.camb.ai/images/og-streams.png">
```

---

## Blog Listing

```html
<title>CAMB.AI Blog — AI Dubbing, Translation & Localization Insights</title>
<meta name="description" content="Expert insights on AI dubbing, voice translation, TTS, and localization. Industry guides, case studies, benchmarks, and product updates from the CAMB.AI team.">
<link rel="canonical" href="https://www.camb.ai/blog">

<meta property="og:type" content="website">
<meta property="og:title" content="CAMB.AI Blog — AI Dubbing, Translation & Localization Insights">
<meta property="og:description" content="Expert insights on AI dubbing, voice translation, and localization. Guides, case studies, and updates from CAMB.AI.">
<meta property="og:url" content="https://www.camb.ai/blog">
<meta property="og:image" content="https://www.camb.ai/images/og-blog.png">
```

---

## Blog Post Template

```html
<title>{{POST_TITLE}} | CAMB.AI Blog</title>
<meta name="description" content="{{150-160 char description summarizing the post's key takeaway}}">
<link rel="canonical" href="https://www.camb.ai/blog-post/{{SLUG}}">

<meta property="og:type" content="article">
<meta property="og:title" content="{{POST_TITLE}}">
<meta property="og:description" content="{{OG description — slightly shorter, 100-120 chars}}">
<meta property="og:url" content="https://www.camb.ai/blog-post/{{SLUG}}">
<meta property="og:image" content="{{FEATURED_IMAGE_URL}}">
<meta property="article:published_time" content="{{YYYY-MM-DDTHH:MM:SSZ}}">
<meta property="article:modified_time" content="{{YYYY-MM-DDTHH:MM:SSZ}}">
<meta property="article:author" content="{{AUTHOR_NAME}}">
<meta property="article:section" content="{{CATEGORY}}">
<meta property="article:tag" content="{{TAG_1}}">
<meta property="article:tag" content="{{TAG_2}}">
```

---

## Pricing Page

```html
<title>CAMB.AI Pricing — AI Dubbing & Translation Plans</title>
<meta name="description" content="Explore CAMB.AI pricing plans for AI dubbing, voice translation, and TTS. Free tier available. Enterprise plans for high-volume localization.">
<link rel="canonical" href="https://www.camb.ai/pricing">

<meta property="og:type" content="website">
<meta property="og:title" content="CAMB.AI Pricing — AI Dubbing & Translation Plans">
<meta property="og:description" content="AI dubbing and translation plans. Free tier available. Enterprise pricing for high-volume localization needs.">
<meta property="og:url" content="https://www.camb.ai/pricing">
<meta property="og:image" content="https://www.camb.ai/images/og-pricing.png">
```

---

## About Page

```html
<title>About CAMB.AI — AI Localization Company & Team</title>
<meta name="description" content="Learn about CAMB.AI, the AI dubbing and voice translation company trusted by IMAX, MLB, and the Australian Open. Meet our team, mission, and investors.">
<link rel="canonical" href="https://www.camb.ai/about">

<meta property="og:type" content="website">
<meta property="og:title" content="About CAMB.AI — AI Localization Company & Team">
<meta property="og:description" content="The AI dubbing company trusted by IMAX, MLB, and the Australian Open. Meet our team and mission.">
<meta property="og:url" content="https://www.camb.ai/about">
<meta property="og:image" content="https://www.camb.ai/images/og-about.png">
```

---

## Events Page

```html
<title>CAMB.AI Events — AI Dubbing Demos & Industry Conferences</title>
<meta name="description" content="Join CAMB.AI at upcoming events, conferences, and live AI dubbing demonstrations. See real-time translation technology in action.">
<link rel="canonical" href="https://www.camb.ai/events">

<meta property="og:type" content="website">
<meta property="og:title" content="CAMB.AI Events — AI Dubbing Demos & Industry Conferences">
<meta property="og:description" content="Upcoming events, conferences, and live AI dubbing demonstrations from CAMB.AI.">
<meta property="og:url" content="https://www.camb.ai/events">
<meta property="og:image" content="https://www.camb.ai/images/og-events.png">
```

---

## Translation Page Template

```html
<title>Free {{Source_Lang}} to {{Target_Lang}} AI Translator | CAMB.AI</title>
<meta name="description" content="Translate {{Source_Lang}} to {{Target_Lang}} with AI dubbing and voice translation. Free online translator for audio, video, and text by CAMB.AI.">
<link rel="canonical" href="https://www.camb.ai/translate/{{source}}-to-{{target}}">

<meta property="og:type" content="website">
<meta property="og:title" content="Free {{Source_Lang}} to {{Target_Lang}} AI Translator | CAMB.AI">
<meta property="og:description" content="AI-powered {{Source_Lang}} to {{Target_Lang}} translation for audio, video, and text. Free online translator by CAMB.AI.">
<meta property="og:url" content="https://www.camb.ai/translate/{{source}}-to-{{target}}">
<meta property="og:image" content="https://www.camb.ai/images/og-translate.png">
```

---

## Comparison Page Template

```html
<title>CAMB.AI vs {{Competitor}} — AI Dubbing Comparison (2026)</title>
<meta name="description" content="Compare CAMB.AI and {{Competitor}} for AI dubbing and translation. Side-by-side feature comparison, pricing, language support, and use cases.">
<link rel="canonical" href="https://www.camb.ai/compare/camb-ai-vs-{{competitor-slug}}">

<meta property="og:type" content="article">
<meta property="og:title" content="CAMB.AI vs {{Competitor}} — AI Dubbing & Translation Comparison">
<meta property="og:description" content="Side-by-side comparison of CAMB.AI and {{Competitor}}. Features, pricing, and language support.">
<meta property="og:url" content="https://www.camb.ai/compare/camb-ai-vs-{{competitor-slug}}">
<meta property="og:image" content="https://www.camb.ai/images/og-compare-{{competitor-slug}}.png">
```

---

## Case Study Template

```html
<title>{{Client_Name}} Case Study — AI Dubbing Results | CAMB.AI</title>
<meta name="description" content="How {{Client_Name}} used CAMB.AI for AI dubbing and translation. {{Key_metric_or_result}}. Read the full case study.">
<link rel="canonical" href="https://www.camb.ai/case-studies/{{slug}}">

<meta property="og:type" content="article">
<meta property="og:title" content="{{Client_Name}} Case Study — AI Dubbing with CAMB.AI">
<meta property="og:description" content="How {{Client_Name}} achieved {{Key_result}} with CAMB.AI's AI dubbing platform.">
<meta property="og:url" content="https://www.camb.ai/case-studies/{{slug}}">
<meta property="og:image" content="https://www.camb.ai/images/og-case-study-{{slug}}.png">
```

---

## Industry/Solutions Page Template

```html
<title>AI Dubbing for {{Industry}} — CAMB.AI Solutions</title>
<meta name="description" content="AI dubbing and voice translation solutions for {{Industry}}. Localize {{content_type}} in 150+ languages with CAMB.AI. {{Key_benefit}}.">
<link rel="canonical" href="https://www.camb.ai/solutions/{{industry-slug}}">

<meta property="og:type" content="website">
<meta property="og:title" content="AI Dubbing for {{Industry}} | CAMB.AI">
<meta property="og:description" content="AI dubbing and translation solutions built for {{Industry}}. 150+ languages, real-time capabilities.">
<meta property="og:url" content="https://www.camb.ai/solutions/{{industry-slug}}">
<meta property="og:image" content="https://www.camb.ai/images/og-solutions-{{industry-slug}}.png">
```

---

## Regional Landing Page Template

```html
<title>CAMB.AI in {{Region}} — AI Dubbing & Translation</title>
<meta name="description" content="CAMB.AI's AI dubbing and translation services for {{Region}}. Support for {{key_languages}}. Local case studies and regional solutions.">
<link rel="canonical" href="https://www.camb.ai/regions/{{region-slug}}">

<meta property="og:type" content="website">
<meta property="og:title" content="CAMB.AI in {{Region}} — AI Dubbing & Translation">
<meta property="og:description" content="AI dubbing and translation for {{Region}}. {{key_languages}} and {{num_languages}}+ more languages supported.">
<meta property="og:url" content="https://www.camb.ai/regions/{{region-slug}}">
<meta property="og:image" content="https://www.camb.ai/images/og-region-{{region-slug}}.png">
```
