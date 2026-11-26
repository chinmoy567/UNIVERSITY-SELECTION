# CLAUDE.md — Project Rules

## 1. About the User (Student Profile)

| Item | Detail |
|---|---|
| Home country | Bangladesh |
| Goal | Master's degree in **Canada** |
| Subjects | Computer Science (CSC), AI/ML, IT, Software Engineering |
| Degree type | **Course-based only** (no thesis, no research-based) |
| CGPA | **3.33 / 4.00** (university scale) |
| University class | Not First Class (First Class = 3.75+). 3.33 counts as "below 70%" |
| Percentage | About **66%** |
| Number of programs | Apply to about **2** universities |

> **Full profile (CGPA, IELTS, semester results):** `My Profile - Check Eligibility.md` in the project root. Agents and skills must read it before any eligibility check.

### Countries
- **Target: Canada only.**
- **Do NOT research or suggest New Zealand or Australia.** The user changed their mind.
- Ignore old New Zealand / Australia notes in the git history. Do not add more.

### Program rules
- Only course-based, project-based or capstone/internship programs. No thesis route.
- Skip programs that need a thesis or a research supervisor.
- Check that a 3.33 CGPA (about 66%) can meet the minimum. Flag programs where it is too low.

---

## 2. Verify Everything

- Every fact must be checked on the web, using **official sources** (university pages, IRCC, provincial government).
- Never answer from memory for fees, deadlines, CGPA limits, IELTS, or immigration rules.
- For each fact, show: **source link** and **date checked**.
- If a fact cannot be verified, write **"Not verified"**. Do not guess.
- If sources disagree, show both and say which is more official.
- Use the agents and skills in `.claude/` for checking (admission-verifier, program-format-verifier, immigration-researcher, research-auditor).

---

## 3. Money Rules

- **Always show cost in both CAD and BDT (Bangladeshi Taka).**
- Show the exchange rate used and the date. Look up the current rate by web search each time.
- Format: `CAD 25,000 (≈ BDT X,XXX,XXX)`
- Show tuition per year and total program cost separately. Say whether fees are for international students.

---

## 4. Writing Style

- **Simple English.** Short sentences. No hard words.
- **No walls of text.** Do not bombard the user.
- Use **tables**, short bullets and clear headings.
- Keep answers short. Give the answer first, then details.
- Explain any special term in one simple line.

---

## 5. Standard Layout for Each Program File

Each program file should follow this order:

1. **Quick summary table** (University, Program, City/Province, Degree type, Duration)
2. **Cost table** (CAD + BDT)
3. **Admission table** (CGPA needed, IELTS, degree needed, documents, deadlines)
4. **Can I apply with 3.33 CGPA?** Yes / Maybe / No, and why
5. **Program format** (course-based? project? thesis?)
6. **Work and immigration** (co-op, PGWP, provincial pathway)
7. **Sources** (links + date checked)

---

## 6. Git Rule: Commit and Push After Every Change

- After **every change** to any file, even a small one, **commit and then push**.
- Do this without asking each time. The user has approved it for this project.
- One change = one commit. Use a short, clear message (what changed and why).
- Run `git status` first. Stage only the files that changed. Never commit secrets (`.env`, credentials).
- After every simple change, commit and **push to `main`**. The user approved pushing to `main` (2026-11-25). Do not ask each time.
- Do not force push.
- If the push fails, say so and show the error. Do not hide it.

---

## 7. Folder Structure

`Canada / <Province> / <University> / <Program> / <Program>.md`

Keep this structure. Number folders as already done.
