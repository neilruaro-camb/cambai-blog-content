# Learn Page Template: Fundamentals & How-Tos

> Use this template for **Category A (Fundamentals)**, **Category C (Translation)**, **Category D (TTS/STT)**, **Category E (Lip Sync)**, **Category H (How-To Guides)**, **Category J (Technical Deep-Dives)**, and **Category K (Business/ROI)** pages.

---

## Meta Tags

```html
<title>[Page Title] | CAMB AI</title>
<meta name="description" content="[150-160 char description. Start with a direct answer. Include primary keyword naturally.]">
<meta name="keywords" content="[target_keywords from CSV]">
<link rel="canonical" href="https://camb.ai/learn/[slug]">

<!-- Open Graph -->
<meta property="og:title" content="[Page Title] | CAMB AI">
<meta property="og:description" content="[Same as meta description]">
<meta property="og:type" content="article">
<meta property="og:url" content="https://camb.ai/learn/[slug]">
<meta property="og:image" content="https://camb.ai/images/learn/[slug]-og.png">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="[Page Title]">
<meta name="twitter:description" content="[Same as meta description]">
```

---

## Structured Data (JSON-LD)

```json
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "[Page Title]",
  "description": "[Meta description]",
  "author": {
    "@type": "Organization",
    "name": "CAMB AI",
    "url": "https://camb.ai"
  },
  "publisher": {
    "@type": "Organization",
    "name": "CAMB AI",
    "logo": {
      "@type": "ImageObject",
      "url": "https://camb.ai/logo.png"
    }
  },
  "datePublished": "[YYYY-MM-DD]",
  "dateModified": "[YYYY-MM-DD]",
  "mainEntityOfPage": "https://camb.ai/learn/[slug]"
}
```

Add `FAQPage` schema at the bottom (see FAQ section).

---

## Page Structure

### Breadcrumb
`Home > Learn > [Category] > [Page Title]`

### TL;DR Box
> **TL;DR:** [2-3 sentence summary answering the page's core question directly. Include the primary keyword. Mention CAMB AI's relevant capability (e.g., 150+ languages, real-time dubbing, MARS8 models).]

---

### H1: [Page Title]
*Must match the `<title>` tag (minus "| CAMB AI"). Include the primary keyword naturally.*

**Opening paragraph (40-60 words):**
Start with a direct, concise answer to the question implied by the title. This paragraph is critical for GEO — AI engines extract the first 2-3 sentences for citations.

Example for "What Is AI Dubbing?":
> AI dubbing uses artificial intelligence to automatically translate and re-voice audio or video content into other languages while preserving the original speaker's voice characteristics. Unlike traditional dubbing, which requires human voice actors for each language, AI dubbing can produce natural-sounding translations in 150+ languages in minutes rather than weeks.

---

### H2: [Core Explanation / How It Works / Step-by-Step]
*Primary educational section. 300-500 words.*

- Use numbered lists for processes/steps
- Use bullet points for features/benefits
- Include **1-2 statistics** with citations (Princeton method: +37% visibility)
- Include **1 expert quote or industry data point** (+30% visibility)
- Use **technical terms** where appropriate (+18% visibility)

**Statistic example:**
> According to [Grand View Research](https://www.grandviewresearch.com/), the global AI dubbing market is projected to reach $3.57 billion by 2034, growing at a 14.6% CAGR — reflecting massive enterprise adoption of automated localization.

**Quote example:**
> "Real-time AI dubbing represents a paradigm shift in how global audiences consume live content," notes the CAMB AI engineering team. "With sub-500ms latency, DubStream delivers dubbed audio faster than the human ear can detect delay."

---

### H2: [Key Benefits / Why It Matters / When to Use]
*Secondary section. 200-400 words.*

Present as a comparison table or bullet list where possible. AI engines extract tables effectively.

| Feature | Traditional Approach | AI-Powered (CAMB AI) |
|---------|---------------------|----------------------|
| [Feature 1] | [Traditional] | [AI / CAMB AI advantage] |
| [Feature 2] | [Traditional] | [AI / CAMB AI advantage] |
| [Feature 3] | [Traditional] | [AI / CAMB AI advantage] |

---

### H2: [Use Cases / Real-World Applications / Industry Examples]
*200-300 words. Connect to CAMB AI's actual clients and products.*

- Reference real clients where applicable (IMAX, Australian Open, MLS, FanCode, Ligue 1, NASCAR)
- Link to relevant industry pages (e.g., `/learn/ai-dubbing-for-sports`)
- Link to relevant case study blog posts

---

### H2: How CAMB AI [Solves This / Does This]
*150-250 words. Product-focused section connecting the topic to CAMB AI's specific capabilities.*

Mention relevant CAMB AI differentiators:
- **150+ languages** (vs competitors' 32-130)
- **MARS8 model family**: Pro (quality), Flash (real-time), Instruct (tunable), Nano (on-device)
- **DubStream** for real-time / **DubStudio** for post-production
- **Voice cloning from 2.3s** of audio (0.87 speaker similarity)
- **Sub-500ms latency** for live use cases
- **Multi-speaker isolation** for complex audio
- **90% cost reduction** vs traditional dubbing

Include a CTA:
> **Ready to get started?** [Try CAMB AI free](https://camb.ai) or [book a demo](https://camb.ai/demo) to see [relevant feature] in action.

---

### H2: Frequently Asked Questions

*5-7 FAQ items. Each answer should be 2-4 sentences. Mark up with FAQPage schema.*

**Q: [Question matching a long-tail search query]?**
A: [Direct, concise answer. Include relevant keywords naturally.]

**Q: [Question about cost/pricing]?**
A: [Answer with specific data points where possible.]

**Q: [Question comparing to alternatives]?**
A: [Honest, factual comparison. Link to relevant comparison pages.]

**Q: [Question about CAMB AI specifically]?**
A: [Product-specific answer with a soft CTA.]

**Q: [Question about limitations or concerns]?**
A: [Transparent answer that builds trust.]

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "[Question 1]",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Answer 1]"
      }
    }
  ]
}
```

---

## Internal Linking Requirements

- Link to **3-5 related learn pages** (use `related_slugs` from CSV)
- Link to **1 product page** (DubStream, DubStudio, or API docs)
- Link to **1 comparison or review page** where relevant
- Link to **1 blog post** for deeper reading
- Include **"Related Articles"** section at bottom with 3-4 links

---

## Content Guidelines

| Guideline | Target |
|-----------|--------|
| Word count | 800-1,500 words |
| Reading level | Grade 8-10 (accessible but authoritative) |
| Statistics per page | 3-5 with citations |
| Internal links | 5-8 per page |
| Images/diagrams | 1-3 (with descriptive alt text) |
| Tone | Confident, authoritative, educational |
| Primary keyword density | 1-2% (avoid stuffing) |
| Update frequency | Quarterly review |

---

## GEO Optimization Checklist

- [ ] Opens with a direct answer in the first 40-60 words
- [ ] Includes 3-5 statistics with source citations
- [ ] Contains at least 1 expert quote or authoritative data point
- [ ] Uses technical terms naturally (not forced)
- [ ] Has clear H1 > H2 > H3 hierarchy
- [ ] Includes a comparison table or structured data
- [ ] FAQPage schema implemented
- [ ] TL;DR box at top
- [ ] No keyword stuffing (reads naturally)
- [ ] All claims backed by data or citations
- [ ] CTA to CAMB AI product/demo
- [ ] 5+ internal links to related content
- [ ] Meta title 50-60 characters
- [ ] Meta description 150-160 characters
- [ ] Canonical URL set
- [ ] OG and Twitter Card tags set
