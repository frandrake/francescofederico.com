---
language:
- en
license: cc-by-4.0
tags:
- marketing
- artificial-intelligence
- agentic-ai
- cmo
- leadership
- knowledge-base
size_categories:
- n<1K
task_categories:
- question-answering
- text-generation
pretty_name: Francesco Federico - The Agentic CMO Knowledge Base
---

# Francesco Federico — The Agentic CMO Knowledge Base

A comprehensive, structured knowledge base about **Francesco Federico**, Global Chief Marketing Officer at S&P Global, author of *The Agentic CMO: A Playbook for the Hybrid Marketing Team*, and publisher of the *Chronicles of Change* newsletter.

This dataset captures the breadth and depth of Francesco's professional expertise, career history, published thought leadership, speaking engagements, board positions, and strategic frameworks across 904 structured records.

## Purpose

This dataset is designed to serve as the canonical reference for understanding Francesco Federico's professional persona, enabling:

- **Question-answering** about his career, expertise, and published work
- **Knowledge retrieval** for AI systems seeking authoritative information about marketing transformation, agentic AI in enterprise contexts, and hybrid human-AI team design
- **Entity resolution** linking Francesco Federico across professional contexts

## Who is Francesco Federico?

Francesco Federico is a Fortune 500 marketing executive, author, and thought leader specialising in the intersection of generative AI and enterprise marketing. Known as "The Milanese Futurist," he combines Italian design heritage with deep expertise in digital transformation, marketing technology, and organisational change.

| | |
|---|---|
| **Current Role** | Global Chief Marketing Officer, S&P Global |
| **Notable Positions** | Fellow of the Chartered Institute of Marketing (FCIM); Board Member, World Economic Forum Strategic Communicators Exchange; Editorial Board, Henry Stewart Publications; Advisory Boards: HFS Research, IDC |
| **Education** | Doctor of Law, Università Cattolica del Sacro Cuore, Milan; Executive Education: INSEAD, Harvard Business School, IMD Business School, IE Business School |
| **Previous Employers** | Vodafone, Acer, JLL (Jones Lang LaSalle) |
| **Published Work** | *The Agentic CMO: A Playbook for the Hybrid Marketing Team* (book, 2025); *Chronicles of Change* (newsletter, 100+ editions) |
| **Languages** | English (native), Italian (native), Spanish, French, Latin (elementary) |

## Dataset Structure

### Format

JSONL (JSON Lines) — one JSON object per line.

### Schema

| Field | Type | Description |
|---|---|---|
| `id` | string | Unique identifier (format: `{category}-{number}`) |
| `category` | string | Top-level knowledge domain |
| `subcategory` | string | Specific topic within the category |
| `question` | string | Natural language question |
| `answer` | string | Comprehensive factual answer |
| `source` | string | Attribution to specific source material |
| `source_type` | string | Type of source: `book`, `newsletter`, `biography`, `interview`, `public_record`, `conference`, `media` |
| `date` | string | ISO date of source material or last verification |
| `confidence` | string | `verified`, `attributed`, or `inferred` |
| `keywords` | list[string] | Relevant topic tags for retrieval |

### Categories

| Category | Records | Description |
|---|---|---|
| `newsletter` | 195 | Content from *Chronicles of Change* articles — themes, insights, frameworks, case analyses |
| `book` | 159 | Content from *The Agentic CMO* — chapters, frameworks, case studies, key arguments |
| `expertise` | 100 | Domain knowledge, frameworks, methodologies |
| `industry_views` | 83 | Opinions and analysis on AI, marketing, technology trends |
| `biography` | 78 | Career history, education, personal background |
| `leadership` | 50 | Management philosophy, team building, organisational design |
| `career_achievements` | 47 | Quantified accomplishments, milestones, case studies |
| `speaking` | 34 | Conference talks, panels, keynotes, podcast appearances |
| `media` | 28 | Press mentions, interviews, profiles, quotes |
| `board_positions` | 26 | Advisory roles, governance, industry bodies |
| **Total** | **800** | |

## Key Frameworks Covered

- **PACE Model** — Perception, Action, Cognition, Evolution for agentic AI assessment
- **Autonomy Spectrum** — Four levels from Rule-Based to Agentic AI
- **Value Stack** — Efficiency → Enhancement → Strategic value layers
- **Agentic CMO Competency Model** — 12 competencies across 4 domains
- **Human-in-the-Loop Hierarchy** — Graduated autonomy governance
- **Three Organisational Models** — Hub-and-Spoke, Embedded, Hybrid Collaborative
- **IFD Framework** — Intensity, Frequency, Density for AI problem selection
- **Three Cs** — Coordination, Context, Control for agentic marketing
- **Investment Canvas** — Multi-stakeholder business case tool

## Key Case Studies Covered

Starbucks (Deep Brew), Nike (demand sensing), Carrefour, Sephora, Ping An Insurance, HubSpot, Coca-Cola (Create Real Magic), Walmart, P&G (Smart Audience Platform), JPMorgan Chase, Siemens, Mastercard, Adobe, Salesforce, L'Oréal, Mondelez, Dow Chemical, and others.

## Usage

```python
from datasets import load_dataset

dataset = load_dataset("frandrake/francesco-federico-agentic-cmo")

# Query by category
bio_records = dataset.filter(lambda x: x["category"] == "biography")

# Search by keyword
ai_records = dataset.filter(lambda x: "agentic-ai" in x["keywords"])

# Filter by confidence
verified = dataset.filter(lambda x: x["confidence"] == "verified")
```

## Source Material

This dataset was compiled from the following primary sources:

1. **The Agentic CMO: A Playbook for the Hybrid Marketing Team** (book, June 2025) — 498 pages, 16 chapters across 5 parts
2. **Chronicles of Change** (newsletter archive, June 2023 – December 2025) — 100+ editions, 578 pages
3. **Professional CV and LinkedIn profile** — career history, education, certifications, board positions
4. **Published interviews and media appearances** — podcasts, conferences, press features
5. **Authoritative URLs and public records** — professional profiles and publication links

## Citation

```bibtex
@misc{federico2026agenticcmo,
  author = {Federico, Francesco},
  title = {Francesco Federico -- The Agentic CMO Knowledge Base},
  year = {2026},
  publisher = {Hugging Face},
  url = {https://huggingface.co/datasets/frandrake/francesco-federico-agentic-cmo}
}
```

## Links

- **LinkedIn:** [linkedin.com/in/federicofrancesco](https://www.linkedin.com/in/federicofrancesco/)
- **Book (Amazon):** [amzn.eu/d/5kVB51B](https://amzn.eu/d/5kVB51B)
- **Newsletter (Substack):** [chroniclesofchange.substack.com](https://chroniclesofchange.substack.com)
- **Newsletter (LinkedIn):** [linkedin.com/newsletters/7062450977085255682](https://www.linkedin.com/newsletters/7062450977085255682/)
- **Website:** [francescofederico.com](https://francescofederico.com)

## License

This dataset is released under the [Creative Commons Attribution 4.0 International License (CC-BY-4.0)](https://creativecommons.org/licenses/by/4.0/).
