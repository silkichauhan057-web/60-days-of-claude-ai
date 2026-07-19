# Day 13 — Job Discovery with Indeed Connector

## Task
Use Claude's Indeed Connector to build a professional profile, define job search criteria, and discover matching job opportunities with match scores, skill-gap analysis, and market demand insights.

## Important Note — Connector Not Available in This Session
This Claude session (claude.ai chat interface, as used here) did **not** have an Indeed Connector or any live job board/web search tool available. Connectors are set up per-account under Settings, and none were active in this conversation. Rather than fabricate job postings, company names, or application links — which would be actively misleading for a real job search — I did the following instead:

1. Built out **Prompt 1 (Professional Profile)** and **Prompt 2 (Job Search Criteria)** fully, using real resume data and the user's stated preferences.
2. For **Prompt 3 (Job Discovery)**, since no connector was available, generated a **manual search strategy** — exact Boolean search queries and filters for LinkedIn, Naukri, and Indeed — so the user could run the discovery themselves and get real, current results.
3. Offered to build the full Match Score / Skill Gap / CTC comparison table once the user pastes back real postings they find.

**If you do have Indeed Connector access in your own Claude account** (via Settings → Connectors), reconnect there and rerun Prompt 3 directly — it will work as intended in that environment. This session simply didn't have it enabled.

## Professional Profile (Prompt 1 Output)
- **Current role:** CS Engineering Student (Final Year) + Data Analytics Trainee, Anudip Foundation
- **Experience:** 0 years (fresher/entry-level)
- **Key skills:** Java, Python, SQL (MySQL), JDBC, DSA, Excel, Power BI (in progress), Pandas (basic)
- **Domain expertise:** Database-integrated software development + emerging Data Analytics
- **Location:** Baghpat, Uttar Pradesh, India
- **Achievements:** Java DSA certification, CGPA 7.62/10, Hospital Management System project, active on GitHub & LeetCode

## Job Search Criteria (Prompt 2 Output)
- **Desired titles:** Data Analyst, Junior Data Analyst, Java Developer (Fresher), Associate Software Engineer, SQL Developer, Business Analyst Trainee, Graduate Engineer Trainee
- **Work mode:** Remote
- **Location:** Delhi NCR (remote-based)
- **Posting recency:** Last 24 hours
- **Salary expectations:** Not yet specified
- **Excluded industries/companies:** None specified

## Job Discovery (Prompt 3) — Manual Strategy Used Instead
Since live discovery wasn't possible, exact search strategies were generated for:
- **LinkedIn Jobs** — Boolean query + Remote/24hr/Entry-level filters
- **Naukri.com** — search terms + Delhi/NCR + Remote + 0-1 years filters, with Job Alert tip
- **Indeed** — search terms + Remote + Delhi NCR + Last 24 hours filters
- **Bonus platforms:** AngelList/Wellfound, Internshala (Jobs not Internships), Cutshort.io

Full details saved in `Job_Search_Profile_Strategy.pdf` (from Day 12/13 work).

## Skill Gap & Market Demand Insights
(Carried forward from earlier analysis, applicable to target roles)
- **Strong:** Java, Python, SQL, JDBC, DSA (certified), Excel, Power BI (in progress)
- **Missing:** Tableau, NumPy, formal statistics, cloud basics, a full end-to-end analytics project, formal internship experience
- **Market signal:** Entry-level Data Analyst and Java Developer postings consistently emphasize SQL + a visualization tool (Power BI/Tableau) + basic statistics — matches the gap areas identified

## Screenshots
- [ ] Screenshot of Prompt 1/2 outputs (Professional Profile + Job Search Criteria)
- [ ] Screenshot of the search strategy document
- [ ] If Indeed Connector is available in your own account: screenshot of actual discovered job listings with match scores

## Key Learnings
- Not every tool mentioned in a task list is available in every session/account — verifying tool access before promising output matters more than pushing through with fabricated results.
- A manual search strategy (exact Boolean queries + filters) is a solid fallback when a live connector isn't available — it gets the user real results, just with one extra manual step.
- Being explicit about *why* something couldn't be done (rather than silently faking it) preserves trust in the rest of the toolkit's output.
- Once real job postings are gathered, the earlier-built resume, cover letter, and outreach templates (Day 11/12) are what actually get used to apply — the discovery step feeds directly into those.
