# Persona Page Template

> Use this template for **Category L: Persona Pages** — audience-specific landing pages targeting a particular user type or job role (e.g., "AI Dubbing for Content Creators", "AI Dubbing for Enterprise Teams").
>
> **Must read first:** `templates/GEO-CONTENT-OPTIMIZATION-GUIDE.md` — contains the Three-Pillar Framework, AEO/GEO content block patterns, and platform-specific optimization rules that apply to every page.

---

## Meta Tags

```html
<title>AI Dubbing for [Persona]: [Key Benefit] | CAMB AI</title>
<meta name="description" content="AI dubbing solutions for [persona]. [Key benefit 1] and [key benefit 2] with CAMB AI's [relevant feature]. Trusted by [client name]. Try free.">
<meta name="keywords" content="[target_keywords from CSV]">
<link rel="canonical" href="https://camb.ai/learn/ai-dubbing-for-[persona-slug]">

<!-- Open Graph -->
<meta property="og:title" content="AI Dubbing for [Persona] | CAMB AI">
<meta property="og:description" content="[Same as meta description]">
<meta property="og:type" content="article">
<meta property="og:url" content="https://camb.ai/learn/ai-dubbing-for-[persona-slug]">
<meta property="og:image" content="https://camb.ai/images/learn/persona-[slug]-og.png">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="AI Dubbing for [Persona]">
<meta name="twitter:description" content="[Same as meta description]">
```

---

## Structured Data (JSON-LD)

```json
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "AI Dubbing for [Persona]",
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
  "mainEntityOfPage": "https://camb.ai/learn/ai-dubbing-for-[persona-slug]",
  "audience": {
    "@type": "Audience",
    "audienceType": "[Persona Type — e.g., Content Creators, Enterprise L&D Teams, Film Studios]"
  }
}
```

---

## Page Structure

### Breadcrumb
`Home > Learn > [Persona Category] > AI Dubbing for [Persona]`

### Hero Section / TL;DR
> **For [Persona]:** [One sentence describing the core value proposition for this audience]. CAMB AI helps [persona] [achieve specific outcome] in 150+ languages — [key differentiator for this audience].

---

### H1: AI Dubbing for [Persona]

**Opening paragraph (40-60 words):**
Address the persona directly. Acknowledge their specific pain point, then present AI dubbing as the solution. Include the primary keyword.

**Example for Content Creators:**
> As a content creator, your audience doesn't stop at language borders — but your content does. AI dubbing lets you reach viewers in 150+ languages by automatically translating and re-voicing your videos while keeping your authentic voice. CAMB AI makes it possible to go global without hiring translators or voice actors.

---

### H2: Why [Persona] Need AI Dubbing

*200-300 words. Pain points specific to this audience.*

Frame as problems this persona actually faces:

**1. [Pain Point 1]**
[2-3 sentences explaining the problem with a relevant statistic.]

> **Stat:** [Relevant data point — e.g., "76% of consumers prefer content in their native language, but only 20% of YouTube content is non-English" with citation.]

**2. [Pain Point 2]**
[2-3 sentences.]

**3. [Pain Point 3]**
[2-3 sentences.]

---

### H2: How [Persona] Use CAMB AI

*300-400 words. Specific workflows and use cases for this persona.*

#### Use Case 1: [Specific workflow]
[150 words describing how this persona would use CAMB AI for this task. Include specific product references (DubStudio, DubStream, API).]

#### Use Case 2: [Specific workflow]
[150 words.]

#### Use Case 3: [Specific workflow]
[100 words.]

**Include a mini case study or example where possible:**
> **Example:** [Client or hypothetical example] used CAMB AI to [specific achievement]. Result: [specific metric — e.g., "3x audience growth in 6 months" or "$500K in traditional dubbing costs saved."]

---

### H2: CAMB AI Features for [Persona]

*Feature comparison table tailored to this persona's priorities.*

| What [Persona] Need | How CAMB AI Delivers |
|---------------------|---------------------|
| [Need 1 — e.g., "Fast turnaround"] | [Feature — e.g., "DubStudio processes a 10-min video in under 5 minutes"] |
| [Need 2 — e.g., "Voice preservation"] | [Feature — e.g., "MARS8-Pro clones your voice from 2.3s of audio (0.87 similarity)"] |
| [Need 3 — e.g., "Budget-friendly"] | [Feature — e.g., "90% cost reduction vs traditional dubbing ($0.50-$1.50/min)"] |
| [Need 4 — e.g., "Easy integration"] | [Feature — e.g., "SDKs in Python, Node.js, and 5 more languages"] |
| [Need 5 — e.g., "Quality control"] | [Feature — e.g., "DubStudio review interface with human-in-the-loop editing"] |

---

### H2: Getting Started as a [Persona]

*150-200 words. Clear next steps tailored to this persona.*

**Step 1:** [First action — e.g., "Sign up for a free CAMB AI account"]
**Step 2:** [Second action — e.g., "Upload your first video to DubStudio"]
**Step 3:** [Third action — e.g., "Select target languages and voice settings"]
**Step 4:** [Fourth action — e.g., "Review, edit, and export your dubbed content"]

> **[Persona]-specific tip:** [One practical tip relevant to this audience — e.g., "Start with your top 3 performing videos and dub them into Spanish, Hindi, and Portuguese for maximum reach."]

**CTAs (choose 1-2 based on persona):**
- [Start dubbing free](https://camb.ai) (for creators, freelancers, startups)
- [Book a demo](https://camb.ai/demo) (for enterprise, studios, broadcasters)
- [Read the API docs](https://docs.camb.ai) (for developers)
- [Contact sales](https://camb.ai/contact) (for agencies, large enterprises)

---

### H2: Resources for [Persona]

*Internal linking section — curated list of the most relevant content for this persona.*

**Tutorials & How-Tos:**
- [How to ... (relevant tutorial)](/learn/[slug])
- [How to ... (relevant tutorial)](/learn/[slug])

**Comparisons & Reviews:**
- [Best AI Dubbing Tools for ... (relevant review)](/learn/[slug])
- [CAMB AI vs ... (relevant comparison)](/learn/[slug])

**Industry Guides:**
- [AI Dubbing for ... (relevant industry page)](/learn/[slug])

**Technical Deep-Dives:**
- [How ... Works (relevant technical page)](/learn/[slug])

---

### H2: Frequently Asked Questions

*5-7 FAQ items tailored to this persona's concerns.*

**Q: How much does AI dubbing cost for [persona]?**
A: [Pricing answer with specific numbers relevant to their scale — e.g., per-video for creators, per-seat for enterprise.]

**Q: Do I need technical skills to use CAMB AI?**
A: [Answer tailored to persona's technical level.]

**Q: How does AI dubbing compare to hiring [relevant alternative — voice actors/translators/agencies]?**
A: [Honest comparison with cost and time data.]

**Q: Can I try CAMB AI before committing?**
A: [Answer about free tier, trial, or demo.]

**Q: What languages are most important for [persona]?**
A: [Answer with data — e.g., "For YouTube creators, Spanish, Hindi, Portuguese, Japanese, and Korean drive the most incremental views."]

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "[Question]",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Answer]"
      }
    }
  ]
}
```

---

## Content Guidelines

| Guideline | Target |
|-----------|--------|
| Word count | 1,000-1,500 words |
| Reading level | Grade 8-10 |
| Statistics per page | 3-5 with citations |
| Internal links | 6-10 per page |
| Tone | Empathetic, solution-oriented, speaks directly to the persona |
| Second person ("you") | Use frequently — speak to the reader |
| Case studies/examples | At least 1 per page |
| CTAs | 2-3 per page (tailored to persona's buying stage) |

---

## Persona-Specific Content Notes

| Persona | Key Pain Points | Buying Stage | Primary CTA |
|---------|----------------|--------------|-------------|
| Content Creators | Cost, speed, voice preservation | Self-serve | Try free |
| Enterprise Teams | Scale, compliance, integration | Sales-assisted | Book demo |
| Film/TV Studios | Quality, lip sync, emotion | Sales-assisted | Book demo |
| Educators | Budget, accessibility, multilingual | Self-serve/demo | Try free |
| Podcasters | Voice preservation, distribution | Self-serve | Try free |
| Developers | API docs, SDKs, latency | Self-serve | API docs |
| Agencies | Volume, white-label, margins | Sales-assisted | Contact sales |
| Broadcasters | Real-time, reliability, scale | Enterprise | Book demo |
| Game Studios | Voice acting, quality, volume | Sales-assisted | Book demo |
| Marketers | ROI, brand voice, campaign speed | Demo | Book demo |
| HR/L&D Teams | Compliance, global reach, budget | Demo | Book demo |
| News Organizations | Speed, accuracy, real-time | Enterprise | Book demo |
| Nonprofits | Budget, accessibility, reach | Self-serve | Try free |
| Government | Compliance, security, accessibility | Enterprise | Contact sales |
| Freelancers | Cost, ease of use, portfolio | Self-serve | Try free |

---

## GEO Optimization Checklist (Three-Pillar Framework)

> See `templates/GEO-CONTENT-OPTIMIZATION-GUIDE.md` for full details.

### Structure (Extractability)
- [ ] Opens with Self-Contained Answer Block addressing the persona directly (40-60 words)
- [ ] First sentence under 30 words (voice search: "What is AI dubbing for [persona]?")
- [ ] Comparison Table Block mapping persona needs → CAMB AI capabilities
- [ ] Evidence Sandwich Block for any ROI/cost claims
- [ ] Step-by-Step Block in "Getting Started" section
- [ ] FAQ section with 5+ persona-specific questions + FAQPage schema
- [ ] Every H2 opens with extractable standalone answer

### Authority (Citability)
- [ ] 3-5 Statistic Citation Blocks relevant to this persona with named sources
- [ ] At least 1 Expert Quote Block or case study
- [ ] No generic content — every section is persona-specific
- [ ] Authoritative tone; speaks directly to the persona ("you")
- [ ] `dateModified` in JSON-LD reflects actual last update

### Presence (Distribution)
- [ ] Article + FAQPage + Audience JSON-LD schema implemented
- [ ] CTAs appropriate for persona's buying stage (see persona table)
- [ ] Resources section links to 4+ relevant internal pages
- [ ] Meta title under 60 characters
- [ ] Meta description 150-160 characters
- [ ] Canonical URL set
