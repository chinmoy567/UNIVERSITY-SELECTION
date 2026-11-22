---
name: website-extraction
description: Crawl and extract tuition, admission, curriculum, and degree structure information from official Canadian university pages.
---

# Website Extraction

Extract only from official or primary-source pages.

Targets: tuition and fees, length and study options, coursework/project/thesis/capstone/internship/co-op requirements, admission CGPA/prerequisites/English tests/deadlines/documents, courses, and governing calendar requirements.

Workflow:
1. Start from the official program or faculty page.
2. Crawl linked graduate calendar and admissions documents.
3. Prefer the current academic year and preserve PDF/page dates.
4. Capture exact supporting sections and source URLs.
5. Mark inaccessible, PDF-only, dynamic, or conflicting content as `NEEDS VERIFICATION`.

Adapted from `firecrawl/skills` crawl, scrape, map, and extraction patterns. Firecrawl use requires `FIRECRAWL_API_KEY` in the integration environment, never in project files.
