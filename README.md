# Krishnendu Biswas

**AI Product Manager | IPM, IIM Ranchi**

I turn repeated, messy work into small products people use. I write the spec, decide what ships and what waits, and run AI coding agents to build it, with a human check at every step where judgement matters.

I'm looking for **AI product manager and product manager roles**.

**Contact:** [krishnendu.me](https://krishnendu.me) · [LinkedIn](https://linkedin.com/in/krshnndu) · [krishnendu.biswasi22@iimranchi.ac.in](mailto:krishnendu.biswasi22@iimranchi.ac.in)

---

## Products

| Product | Problem | User | Key decision | Where it stands |
|---|---|---|---|---|
| **Termly** | Classes, attendance against absence caps, deadlines and course mail are scattered across portals and inboxes | IIM Ranchi students, sign-in limited to `@iimranchi.ac.in` | Rules first, model second: the AI runs only when no rule matches, under daily caps enforced in the database | Live. Used by IIM Ranchi students. Private repo |
| **[CogPrep Arcade](https://krshnndu.github.io/aptitude-game-practice/)** | Game-based cognitive aptitude tests are hard to practise for | Candidates preparing for game-based aptitude assessments | Show *what you did next to what you should have done* for every puzzle, and keep progress in the browser, no account | Live and open source (MIT). Six games, 531 passing tests. [Repo](https://github.com/krshnndu/aptitude-game-practice) |

### Termly, in more detail

- **Scope.** Today's classes, a calendar, attendance against absence caps, deadlines, course materials and a one-way Google Calendar sync.
- **Feature ideas go through a gate.** An LLM triages each suggestion for type, effort, risk and duplicates, then holds it for my decision. I approve, deny, ask for more, or merge, and every decision is logged. 24 decisions are on that audit trail so far.
- **Security as a product requirement.** Row-level security is forced on in Postgres and every write goes through a controlled database function. I commissioned three security review rounds and acted on the findings, including prompt-injection containment, a content security policy and account binding.
- **Who wrote the code.** I defined the requirements, the architecture and the review loop. AI agents wrote most of the implementation from my briefs.

---

## How I work

| | What it looks like in practice |
|---|---|
| **Discovery** | I start with a workflow I or the people around me repeat every week, and write down who does it and where it breaks. |
| **Spec first** | The specification is the thing I iterate on. At QualityKiosk a 1,322-line EARS spec doubled as the acceptance criteria for a module that merged as PR #1. |
| **Prioritisation** | Ideas wait in a queue until I decide on them. A denial is logged with its reason, the same as an approval. |
| **Metrics** | I pick the metric before building and report it as it is: F1 over accuracy on an imbalanced target, counts with a date next to them. |
| **Shipping with AI agents** | Agents implement against the spec; I review, test and decide. I keep a human in the loop wherever a wrong call would be expensive, and I write that rule into the product. |

---

## Experience

**QualityKiosk Technologies**, Data & AI Intern · Apr to Jun 2026

- Took internal estimation and QA tooling from spreadsheets to software: 7 applications on one platform plus 3 standalone tools, in about two months.
- Wrote a 1,147-line ML estimation PRD with 20 requirements and 6 regression targets, and built the pipeline that captures estimate-versus-actual records and scores MAPE by domain.
- Automated Azure DevOps test-case prep in Python, reshaping 18,456 rows across 61 QA workbooks for upload.
- Wrote the deploy runbook and a 402-line monorepo blueprint, then reused the blueprint on a second scaffold, so the next module cost less than the first.

**IIM Ranchi, Corporate Relations and Placement Committee** · Executive Member 2025, Senior Executive Member 2026 to 2027

- Converted 46 corporate accounts and led a 20-member placement coordinator team through training and weekly reviews.
- Automated 5+ placement workflows, saving 500+ hours, and kept the shortlisting and allocation calls with people.

**Tata Steel**, Research Analyst, IR & Rewards · Apr to Jun 2025

- Compensation benchmarking for the IR and Rewards department.

---

## Research

- **Multi-Class Affect Detection in Educational Chatbots: Evidence from Imbalanced Dialogue Data.** Sarkar, Biswas, Pramanik. Accepted, FICTA 2026, Springer Nature (SIST series). RoBERTa with SVMSMOTE reached 74.19% recall on the Confused class.
- **Adoption and Implications of Generative AI in Marketing: A Systematic Review and Research Agenda.** Pandey, Binu Raji, Biswas. Presented at the 10th Pan-IIM World Management Conference (WMC 2025), IIM Ranchi. A PRISMA review of 29 Scopus-indexed articles.

---

## Technical background

<details>
<summary>The hands-on work behind the product calls</summary>

<br>

| Project | What I did | Result |
|---|---|---|
| Smart MCQ Solver | LoRA fine-tuning (r=8) of DeBERTa-v3-base and RoBERTa-base, 70:30 ensemble | 0.74242 MAP@3 on Kaggle's public leaderboard |
| Comment classification | 198K comments, n-gram features, 100-trial Optuna study on LightGBM | F1-Macro from 0.6221 to 0.8293 on 39.6K held-out rows |
| Virtual teaching assistant | RAG pipeline with OpenAI embeddings, SQLite vector store and FastAPI endpoints | Answers cite the course content they came from |

Python, SQL, R, Power BI (PL-300, scored 751), scikit-learn, LightGBM, XGBoost, FastAPI, PostgreSQL. Also a BS in Data Science and Applications at IIT Madras, in progress.

</details>

---

**Education.** Integrated Programme in Management, IIM Ranchi (BBA 2025, MBA phase to Mar 2027). BS in Data Science and Applications, IIT Madras.
