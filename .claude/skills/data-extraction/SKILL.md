---
name: data-extraction
description: Convert verified Canadian university and master's program findings into consistent JSON, CSV, and Markdown records.
---

# Data Extraction

Create consistent evidence-linked records.

Required fields: institution, province, program_name, degree, degree_format, mandatory_requirements, tuition, duration, cgpa_requirement, degree_prerequisites, ielts_requirement, international_eligibility, application_deadline, required_documents, source_urls, publication_dates, access_date, and verification_status.

- Preserve source values and units exactly.
- Use `null` for missing values.
- Use `NEEDS VERIFICATION` for uncertain values.
- Never put estimates in verified fields.
- Emit valid JSON or CSV and a consistent Markdown table.
- Link every important field to a source URL.
