I build the systems behind the money.
Loan books, payment approvals, donor payments, Salesforce automation, and the websites people find you through. I work at NRCF in Nairobi, building software for small teams. It has to be careful with money, keep a record of every change, and be easy for non-technical staff to use.

1,500+ contributions this year · 220+ pull requests merged · 930+ automated tests on one app

Most of my code is private because it handles real people's money or belongs to clients. The summaries below describe what each project does.

Selected work
Project	What it is	Built with
Loan Portal · live	A full loan book: interest, late charges, extensions and rollovers, partly funded loans with funder payouts, a daily email summary, and expenses imported from M-Pesa messages. 383 commits, 157 PRs, and 160+ written design decisions. Deploys automatically through GitHub Actions.	Google Apps Script, Node tests, CI/CD
Approval Portal · pilot	Payment requests and approvals for Google Workspace. Each role gets its own dashboard view, a processing queue keeps requests from being lost, and every step is on a full audit trail.	Google Apps Script
SchoolPress · v2.14	A reusable WordPress block theme for schools: Full Site Editing, parent-focused home pages, mobile quick actions.	WordPress, theme.json, PHP
Ozon Fix · client	A lead-generation theme for a commercial refrigeration firm. Staff track quote requests and edit services without touching the layout. Needs no plugins.	WordPress, PHP, SEO
Salesforce for a nonprofit (NPSP)
I build and run the Salesforce org for a children's charity in Kenya and its US fundraising arm. I've merged 69 pull requests there. GitHub Actions does a test deploy of every pull request before merge, then deploys to the sandbox automatically.

Stripe ↔ Salesforce (sandbox, phase 0)
Card payments close the right NPSP donation, and donors get the right thank-you email automatically.
A reconciliation backstop matches each payment by Stripe ID, then recurring donation, then email and amount.
An LWC admin console switches each of 13 email types between Live, Test and Off. It logs every change and has a preview and one-click resend.
26/26 Apex tests pass at 89–92% coverage, and 11/11 Jest tests pass.
Staff Attendance & Staff Portal
Check in and out with location checks against the office radius.
Staff without a Salesforce login sign in to a staff website with an emailed code.
Corrections need admin approval.
Reminders, weekly summaries, and public holidays filled in automatically each year.
Sponsor & donor communications: bulk email with test mode and a preview before sending, scheduled sends, branded unsubscribe pages, and correspondence history.
NPSP data & org health: a nightly recalculation of the DLRS roll-ups, donation and GAU automation, and CI checks on profiles and permission sets.
Automation & AI
WorkTrail: from meeting promises to verified delivery. It began as a meeting recorder and now tracks whether promised work actually got done:

Records meetings without a bot joining the call, and transcribes them on the device.
Pulls out actions, decisions, questions and risks.
Looks for proof that each one was done in GitHub, Basecamp, Gmail, Calendar, Slack and Salesforce.
Drafts agendas and a monthly report that cites its sources.
Waits for approval before sending or creating anything.
Python · FastAPI · SQLite · on-device transcription (MLX) · Claude API

Also: live operations dashboards built from Basecamp, Gmail and AI-usage data, and an M-Pesa sorting desk that turns SMS receipts into categorised expenses.

How I work
Rules written down first. Every money rule is agreed and numbered before it's coded.
Tested, then shipped. Every change goes through a pull request and CI before it deploys.
A record of every change. Every save is logged, and every change can be traced to who made it and why.
Guides for real users. Each app ships with a plain-language guide that has screenshots, plus a change log.
Stack
Salesforce: Apex · LWC · Flow · NPSP · DLRS · SFDX CI
Payments: M-Pesa Daraja · Flutterwave · Stripe · double-entry ledgers · webhooks
Web: Google Apps Script · JavaScript / Node · PHP · Laravel · WordPress block themes
Data & automation: Python · SQLite · GitHub Actions

Next: Salesforce Administrator and Platform Developer I certifications.
Open to: payment integrations and nonprofit tech projects.

📫 victorwambua004@gmail.com · LinkedIn
