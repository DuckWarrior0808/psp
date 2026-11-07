# Team Agreement — Team Gavel

PS Software Design, VU MIF, autumn 2026. Lecturer: Vasilij Savin.
System under design: **AuctionHub** — multi-type auction platform.

Version 1.0, agreed on 2026-11-07. Every member confirmed the agreement in
[Section 10](#10-confirmation).

| Member | GitHub | Role |
|---|---|---|
| Deividas Matonis | `DuckWarrior0808` | API contract and integration; submissions |
| Klaidas Blandis | **[TODO]** | Backend: auction domain, concurrency, data model |
| Arnas Vyšniauskas | **[TODO]** | Frontend and UI/UX |
| Justinas Jarmalavičius | **[TODO]** | Notifications and realtime; testing and deployment |

Team repository: [DuckWarrior0808/psp](https://github.com/DuckWarrior0808/psp). The lecturer
(`chabbrik`) has write access; every team member is added as a collaborator.
Team chat: Microsoft Teams group chat. Phone numbers and other personal contacts are shared in the
chat, not in this document.

## 1. Team name and leadership

Team name: **Team Gavel**, after the hammer that closes an auction.

### 1.1 Why we have no designated leader

The team decided not to elect a leader. There are four of us with similar experience, and three of
us already work together on another course project. Each member owns clearly defined areas
([Section 4](#4-work-distribution)), decisions are made together ([Section 3](#3-key-team-rules)),
and a single leader would become a bottleneck for questions and reviews.

If the team becomes disorganised — two missed internal deadlines in a row, or decisions that keep
getting postponed — we reconsider this at the next weekly sync and may elect a leader by open vote.

### 1.2 How the leader's duties are shared

| Duty | Who |
|---|---|
| Running the weekly sync, writing its notes, keeping the task board up to date | Facilitator of the week |
| Checking two days before a deadline that every part is ready | Facilitator of the week |
| Submitting deliverables to the repository and messaging the lecturer in Teams | Deividas Matonis (repository owner) |
| Answering the partner team's questions | Owner of the area the question is about |
| Assigning a task that has no owner, or reassigning a missed one | Majority vote at the weekly sync |

The facilitator role rotates weekly in alphabetical order — Arnas, Deividas, Justinas, Klaidas —
starting with the week of November 9. The facilitator has no extra authority: they organise, the
team decides.

## 2. Team ambition

Course points: Lab I — 4, Lab II — 4, personal essay — 1, lecture quizzes — 1.

Common target: final grade **9**, which means at least **3.5 / 4** for Lab I and **3.5 / 4** for
Lab II. The essay and quizzes are individual, so they are not part of the team target.

In practice this means that in Lab II we implement every Must requirement of the project we receive,
add Should requirements where time allows, and show a working live demo from a clean deployment.

## 3. Key team rules

1. On weekdays, answer messages in the team chat within 24 hours.
2. If you will be unavailable or miss a date, say so at least 48 hours before the deadline.
3. Every task has exactly one owner and a due date on the board.
4. All work is pushed to the team repository. Nothing that matters lives only on someone's
   computer.
5. Changes to the documents and the code go through a pull request, and at least one other member
   approves it.
6. Our internal deadline is 48 hours before the official one, so there is time for review.
7. Criticise the work, not the person. Disagreements are discussed on a call, not in long chat
   threads.
8. Decisions are made by consensus. If there is no consensus at a meeting, the majority wins. If
   the vote is tied, the owner of the area the decision concerns decides; if it concerns no single
   area, the facilitator of the week decides. Decisions are written in the meeting notes.

## 4. Work distribution

- We split the work into areas, and each area has one owner. Every member owns at least one
  substantial area in each lab.
- We aim for an equal workload in estimated hours, not an equal number of tasks.
- Less popular work (formatting, diagrams, reviews, test data) rotates between members.
- The owner of an area answers questions about it, including questions from the partner team.

Lab I (AuctionHub specification). Each owner answers the implementing team's questions about their
area and keeps it up to date:

| Area | Owner |
|---|---|
| Overview, actors, functional requirements (sections 1–3) | Deividas Matonis |
| Auction rules, algorithms, business flows, settlement (sections 4–7) | Klaidas Blandis |
| Notifications and realtime protocol (sections 8–9) | Justinas Jarmalavičius |
| NFRs, architecture, modules (sections 10–12) | Justinas Jarmalavičius |
| Data model (sections 13–14) | Klaidas Blandis |
| UI/UX wireframes (section 15) | Arnas Vyšniauskas |
| HTTP API and `openapi.yaml` (sections 16–19) | Deividas Matonis |
| Acceptance tests and handover (sections 20–21) | Arnas Vyšniauskas |

Evaluating the Lab I document we receive: every member reads the whole document and writes
findings for the same kinds of areas they own above; Deividas merges them into the evaluation form.

Lab II (implementing the received project): each member keeps the role from the member table.
Concrete areas of the received project are assigned at the first meeting after it is assigned and
recorded in version 1.1 of this agreement.

### 4.1 First tasks

| Task | Owner | Due |
|---|---|---|
| Add all members as collaborators to the team repository | Deividas Matonis | Nov 8 |
| Upload `openapi.yaml` next to the Lab I PDF | Deividas Matonis | Nov 8 |
| Fill in your GitHub username in this agreement | every member | Nov 9 |
| Send this agreement to the lecturer in Teams | Deividas Matonis | Nov 9 |
| Create the GitHub Projects board and the `meetings/` folder | Justinas Jarmalavičius | Nov 9 |
| Read the received Lab I document; each member writes findings for their areas | every member | 2 days before the evaluation deadline |
| Merge the findings into the evaluation form and submit it | Deividas Matonis | evaluation deadline |
| Lab II skeleton: repository layout, build, database migrations, CI | Justinas Jarmalavičius | 1 week after assignment |
| Lab II domain model and core business rules | Klaidas Blandis | 2 weeks after assignment |
| Lab II screens following the received wireframes | Arnas Vyšniauskas | 2 weeks after assignment |

## 5. Meetings and group work

- Weekly sync: **Sundays at 20:00**, a Teams call of at most 30 minutes.
- Agenda: what was done, what is blocked, who does what until the next meeting.
- In the week before a deadline we hold an extra working session the evening before the internal
  deadline.
- The facilitator of the week writes short notes in `meetings/YYYY-MM-DD.md` in the repository.
- Anyone who cannot attend says so before the meeting and posts their update in the chat.

## 6. Progress tracking

We use a GitHub Projects board in the team repository with the columns *To do*, *In progress*,
*Review* and *Done*. Each task is an issue with an owner and a due date. The board is reviewed at
every weekly sync.

## 7. Sanctions for breaking the agreement

Sanctions escalate step by step:

1. **First missed date or no response without notice:** reminder in the team chat and a new date
   agreed within 24 hours.
2. **Second time:** discussed at the weekly meeting and recorded in the notes; the team may
   reassign the task by majority vote.
3. **Repeated problems, or unreachable for a week (MIA):** any member informs the lecturer after
   telling the team. Each member's real contribution is described in the Lab II evaluation and in
   the personal essays.

## 8. Use of AI tools

One team member uses AI tools in the lab work; the others do not.

- Deividas Matonis uses Claude (Anthropic). In Lab I it was used to check the specification
  against the assignment and the lecture recommendations, and to draft this agreement.
- Klaidas Blandis, Arnas Vyšniauskas and Justinas Jarmalavičius do not use AI tools.
- If a member starts using AI tools, they add them here in a new version of this agreement.
- Allowed uses: drafting and proofreading text, reviewing documents, diagrams and the API for
  inconsistencies, code assistance, generating test data.
- Rules: the member who uses AI output is responsible for it and reads and checks every line before
  committing. We do not paste other teams' documents or personal data into AI tools. When a
  significant part of a pull request was generated with AI, its description says so.

## 9. When we contact the lecturer immediately

Following the lecturer's guidance, any member contacts the lecturer as soon as possible if the team
experiences:

- disrespect or humiliation by other team members;
- lack of organisation that the team cannot fix itself (see [Section 1.1](#11-why-we-have-no-designated-leader));
- a team member who is missing in action;
- a conflict the team cannot resolve.

## 10. Confirmation

The agreement can be changed when all members agree. Each change gets a new version number and
date in the header.

| Member | I agree (date) |
|---|---|
| Deividas Matonis | 2026-11-07 |
| Klaidas Blandis | 2026-11-07 |
| Arnas Vyšniauskas | 2026-11-07 |
| Justinas Jarmalavičius | 2026-11-07 |
