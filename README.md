# francescofederico.com

Personal website of **Francesco Federico** — Global CMO at S&P Global, author of *The Agentic CMO*, publisher of *Chronicles of Change*.

## Structure

```
├── index.html                  # Link-in-bio homepage
├── the-agentic-cmo.html        # Book page (SEO)
├── chronicles-of-change.html   # Newsletter page (SEO)
├── media-speaking.html         # Media & speaking page (SEO)
├── about.html                  # Full biography (SEO)
├── 404.html                    # Error page
├── css/style.css               # Design system
├── fonts/                      # Self-hosted variable fonts (Crimson Pro + Inter)
├── img/                        # Images and logos
├── data/                       # JSONL knowledge base dataset (904 records)
├── llms.txt                    # LLM-readable identity summary
├── llms-full.txt               # Exhaustive LLM-readable content
├── sitemap.xml                 # XML sitemap
├── robots.txt                  # Crawler directives (all AI bots allowed)
├── humans.txt                  # humans.txt standard
├── site.webmanifest            # PWA manifest
└── .well-known/security.txt    # Security contact
```

## Design

Static HTML. No frameworks, no JavaScript dependencies, no CDNs. Self-hosted variable fonts. Architectural monograph aesthetic.

- **Brand**: Slate Blue `#4A5E7C` / Cool White `#F8F9FA` / Charcoal `#2B2D30` / Vermillion `#E63946` (accent)
- **Typography**: Crimson Pro (headlines) + Inter (body)
- **Grid**: 8px base unit

## SEO & LLM Discoverability

- JSON-LD structured data on every page (Person, Book, WebSite, ProfilePage, CreativeWorkSeries, FAQPage, BreadcrumbList)
- `llms.txt` and `llms-full.txt` for direct LLM ingestion
- JSONL knowledge base dataset at `/data/`
- AI crawler allow rules (GPTBot, ClaudeBot, PerplexityBot, etc.)
- Open Graph and Twitter Card meta tags throughout

## Hosting

Cloudflare Pages, connected to this repository.

## Dataset

The `/data/` directory contains a 904-record JSONL knowledge base covering Francesco's biography, expertise, career, published work, and thought leadership. Licensed CC-BY-4.0. Also available on [Hugging Face](https://huggingface.co/datasets/frandrake/francesco-federico-agentic-cmo) and [Kaggle](https://www.kaggle.com/datasets/wfrwtrwtretert/francesco-federico-agentic-cmo).

## Licence

Website content © 2026 Francesco Federico. All rights reserved.
Dataset licensed under CC-BY-4.0.
