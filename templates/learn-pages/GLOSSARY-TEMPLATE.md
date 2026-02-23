# Glossary Page Template

> Use this template for **Category M: Glossary** pages — short-form definition pages targeting "what is [term]?" search queries.
>
> **Must read first:** `templates/GEO-CONTENT-OPTIMIZATION-GUIDE.md` — contains the Three-Pillar Framework, AEO/GEO content block patterns (especially the **Definition Block** pattern), and platform-specific optimization rules.

---

## Meta Tags

```html
<title>What Is [Term]? Definition & Explanation | CAMB AI</title>
<meta name="description" content="[Term] is [one-sentence definition]. Learn how [term] works, why it matters for AI dubbing and localization, and how CAMB AI uses it.">
<meta name="keywords" content="[target_keywords from CSV]">
<link rel="canonical" href="https://camb.ai/learn/glossary-[term-slug]">

<!-- Open Graph -->
<meta property="og:title" content="What Is [Term]? | CAMB AI Glossary">
<meta property="og:description" content="[Same as meta description]">
<meta property="og:type" content="article">
<meta property="og:url" content="https://camb.ai/learn/glossary-[term-slug]">
<meta property="og:image" content="https://camb.ai/images/learn/glossary-og.png">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary">
<meta name="twitter:title" content="What Is [Term]?">
<meta name="twitter:description" content="[Same as meta description]">
```

---

## Structured Data (JSON-LD)

```json
{
  "@context": "https://schema.org",
  "@type": "DefinedTerm",
  "name": "[Term]",
  "description": "[One-paragraph definition]",
  "inDefinedTermSet": {
    "@type": "DefinedTermSet",
    "name": "CAMB AI Glossary",
    "url": "https://camb.ai/learn"
  },
  "url": "https://camb.ai/learn/glossary-[term-slug]"
}
```

Also include `FAQPage` schema for the FAQ section.

---

## Page Structure

### Breadcrumb
`Home > Learn > Glossary > [Term]`

### Definition Box (Featured Snippet Target)
> **[Term]** is [1-2 sentence definition in plain language]. [One sentence connecting it to AI dubbing or voice technology.]

*This box is the primary featured snippet / AI citation target. Keep it under 50 words.*

---

### H1: What Is [Term]?

**Opening paragraph (40-60 words):**
Expand on the definition box with slightly more detail. Explain why someone searching for this term would care. Connect to AI dubbing, voice cloning, or localization.

---

### H2: How [Term] Works

*150-250 words. Accessible technical explanation.*

- Use an analogy if the concept is abstract
- Include a simple diagram or visual description if helpful
- Use 1-2 technical terms but define them inline
- Include **1 statistic** with citation if available

**Example for "What Is Prosody?":**
> Prosody refers to the patterns of stress, rhythm, intonation, and timing in speech. Think of it as the "music" of language — the rises and falls in pitch, the pauses between phrases, and the emphasis placed on certain words. In AI dubbing, prosody transfer ensures that a dubbed voice doesn't just say the right words but says them with the same emotional inflection as the original speaker.

---

### H2: Why [Term] Matters for AI Dubbing

*100-200 words. Connect the term to CAMB AI's domain.*

- Explain the practical relevance of this concept
- How does it affect dubbing quality, user experience, or technical performance?
- Reference CAMB AI's approach where relevant

**Example:**
> In AI dubbing, accurate prosody transfer is the difference between a translation that sounds robotic and one that sounds natural. CAMB AI's MARS8 models are specifically trained to preserve prosodic features across 150+ languages, ensuring that emotion, emphasis, and rhythm carry through even when the words change.

---

### H2: [Term] in Practice

*100-150 words. 2-3 concrete examples or applications.*

- **Example 1:** [Brief real-world application]
- **Example 2:** [Brief real-world application]
- **Example 3:** [Brief real-world application]

---

### H2: Related Terms

*Internal linking to other glossary pages and deeper learn pages.*

| Term | Definition | Learn More |
|------|-----------|------------|
| [Related Term 1] | [One-line definition] | [/learn/glossary-term-1](/learn/glossary-term-1) |
| [Related Term 2] | [One-line definition] | [/learn/glossary-term-2](/learn/glossary-term-2) |
| [Related Term 3] | [One-line definition] | [/learn/glossary-term-3](/learn/glossary-term-3) |

**For a deeper dive, see:** [Full Learn Page Title](/learn/[detailed-page-slug])

---

### H2: Frequently Asked Questions

*3-5 short FAQ items with FAQPage schema.*

**Q: What is [term] in simple terms?**
A: [Plain-language answer, 1-2 sentences.]

**Q: How does [term] relate to AI dubbing?**
A: [Connection to dubbing/localization.]

**Q: Why is [term] important?**
A: [Practical significance.]

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
| Word count | 400-800 words |
| Reading level | Grade 6-8 (highly accessible) |
| Statistics per page | 1-2 with citations |
| Internal links | 3-5 per page (other glossary terms + deeper learn pages) |
| Tone | Educational, concise, accessible |
| Definition box | Under 50 words (featured snippet target) |
| Unique content | Each term MUST have a unique "Why it matters for AI dubbing" section |

---

## GEO Optimization Checklist (Three-Pillar Framework)

> See `templates/GEO-CONTENT-OPTIMIZATION-GUIDE.md` for full details.

### Structure (Extractability)
- [ ] **Definition Block** (under 50 words) directly answers "What is [term]?" — featured snippet target
- [ ] Opening paragraph expands definition as Self-Contained Answer Block (40-60 words)
- [ ] First sentence is under 30 words (voice search: "What is [term]?" → direct answer)
- [ ] "How it works" section uses Step-by-Step or analogy format
- [ ] Related terms table provides structured internal links
- [ ] FAQ section with 3+ natural-language questions + FAQPage schema

### Authority (Citability)
- [ ] At least 1 Statistic Citation Block with named source
- [ ] "Why it matters for AI dubbing" section — unique per term, not generic
- [ ] Authoritative, confident tone
- [ ] `dateModified` in JSON-LD reflects actual last update

### Presence (Distribution)
- [ ] DefinedTerm + FAQPage JSON-LD schema implemented
- [ ] Link to deeper learn page for the topic
- [ ] Related terms table links to 3+ other glossary pages
- [ ] Meta title under 60 characters
- [ ] Meta description 150-160 characters
- [ ] Canonical URL set
