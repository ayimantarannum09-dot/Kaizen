# Kaizen

**A personal coach for students that connects sleep, study and screen habits, shows what is hurting performance, and fixes the schedule before burnout.**

Built for **wHACKiest 2026** (Online Ideathon, 26-27 Nov 2026) · **Track 3: Know Thyself** · Team **J.A.R.V.I.S** · Team ID 16d7084a

---

## The Problem

Students' sleep, study hours, screen time and mood sit in different apps, and nobody connects them. Burnout is noticed only after grades slip.

- **Who it affects:** College students, mostly during exams, when deadlines, bad sleep and stress pile up together.
- **Why it matters:** A student who sleeps 5 hours for a week misses study blocks and crashes just before the exam, with no warning.
- **Why existing apps fall short:** RescueTime tracks screen time only. Google Fit shows charts but not the reason behind them. Forest and planners are manual and ignore deadlines. None of them connect the data or act on it.

Four apps, four charts, and no answer to *why*.

## Our Solution

Kaizen (改善, "continuous improvement") connects a student's habits, explains the reason behind a bad week, and adjusts the schedule with the student's approval.

> "Slept 5 hrs. Study block moved to 4 PM."

### Key features

- Daily 10-second check-in by voice or tap
- Insights such as sleep vs focus
- Exam readiness score
- Every tip comes with its reason
- Calendar changes happen only after the student approves
- Data can be exported or deleted anytime
- Spoken morning briefing (ElevenLabs)

### User flow

Connect data → check in → get insights → approve a change → calendar updates.

## How It Works

1. The student checks in, or data is imported.
2. The backend cleans and stores the data.
3. AI finds patterns and explains the reason.
4. Nudges are shown on the dashboard and spoken aloud.
5. The student approves or rejects the change.
6. Google Calendar is updated.

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React with Chart.js |
| Backend | Python with FastAPI |
| Database | SQLite for the demo, DynamoDB later |
| AI | pandas finds the patterns, Claude API explains the insights |
| Voice | ElevenLabs for the morning briefing and check-ins |
| Integration | Google Calendar and Tasks through MCP |
| Cloud | AWS Lambda, API Gateway and S3 |
| Input | CSV import and manual check-in, no extra hardware needed |

## What We Built in 24 Hours

- Check-in screen
- CSV data import
- Three insights
- Dashboard
- Google Calendar connection
- Spoken morning briefing

## What Makes Kaizen Different

| Feature | Kaizen | RescueTime | Google Fit | Forest |
|---|---|---|---|---|
| Multi-source data | Yes | No | Partial | No |
| Exam / deadline aware | Yes | No | No | No |
| Explains why | Yes | No | No | No |
| Acts on calendar (with approval) | Yes | No | No | No |
| Voice coach | Yes | No | No | No |
| User-owned data / delete | Yes | Partial | Partial | Partial |

Wellbeing data, calendar actions (MCP) and a voice coach come together in one student-focused tool, with data the user owns.

## Impact

- Earlier burnout warnings
- Better sleep and planning
- Fewer exam-week crashes

**What we can measure:** sleep hours, tasks completed and readiness score over time.

## Feasibility and Risks

Kaizen is built on existing MCP servers, ElevenLabs and AWS, with no special hardware. Free tiers cover the prototype, and the MVP is limited to 5 or 6 features.

- **Health apps are hard to connect**, so we start with CSV data.
- **Wrong suggestions** are handled with clear reasons and an approval step.
- **Privacy:** data stays with the user and can be deleted.
- **Not medical advice:** Kaizen gives wellbeing tips, not diagnosis.

## Business Model

- **Customers:** College students in India first, then colleges and coaching institutes.
- **Free:** core insights and check-ins.
- **Premium:** deeper insights and regional-language voice.
- **College plan:** opt-in, anonymous wellbeing dashboards.
- **Reaching users:** campus clubs, hackathons, student ambassadors and a pilot with a college counselling cell.
- **Growth:** campus pilot, then wearables and regional languages, then more colleges.

## Team J.A.R.V.I.S

S J C Institute of Technology

- Ayiman Tarannum (Lead)
- Sowmya V
- Aman Raj
- Shaurya Singh

## License


