---
name: website-extraction
description: Crawl and extract tuition, admission, curriculum, and degree structure information from official Canadian university pages.
---

# Website Extraction

Extract only from official or primary-source pages using local Python and BeautifulSoup.

Targets: tuition and fees, length and study options, coursework/project/thesis/capstone/internship/co-op requirements, admission CGPA/prerequisites/English tests/deadlines/documents, courses, and governing calendar requirements.

Workflow:
1. Fetch a public HTML page with Python's standard HTTP support or a normal HTTP client.
2. Parse and inspect it locally with BeautifulSoup.
3. Start from the official program or faculty page, then follow linked graduate calendar and admissions documents.
4. Use Playwright MCP for JavaScript-rendered pages or browser interactions that BeautifulSoup cannot handle.
5. Prefer the current academic year and preserve PDF/page dates.
6. Capture exact supporting sections and source URLs.
7. Mark inaccessible, PDF-only, dynamic, or conflicting content as `NEEDS VERIFICATION`.

Do not use a crawling API, paid extraction service, credentials, or API keys.
