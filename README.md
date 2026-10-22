# VerifyMe Account Management Workspace

A clickable concept prototype for an account management workspace built around identity verification services. It shows how account managers, technical support and implementation (TSI), the Verification Services (VS) team, Admins and team leads could work from one shared view of every customer.

**Live demo:** open `index.html` in a browser, or visit https://victorobioha017-ship-it.github.io/verifyme-am-workspace/.

## What you can try

- **Home:** portfolio health, open signals, escalations with live SLA clocks, and tasks due today
- **Notifications:** one inbox for everything waiting on you (customer messages, escalations from other teams, technical tickets, updates on what you raised, handovers, onboarding, customer health, automatic log sends, upsell, invoices and reports), sorted by level (Critical, High, Normal, Info), each with a button to take the next action
- **Organisation IDs:** every customer has an org ID, shown on the account, in pickers, exports and invoices, and searchable in Accounts and Escalations. Add update takes an org ID to find the customer
- **Request IDs:** escalations carry the request ID of each applicant or address involved (a batch shows every ID with its status), and cases can be filtered by org ID, request ID, case ID or batch
- **Role-based access:** everyone can see the full customer list. TSI and Admins see everything an AM sees (including Signals and Opportunities); the VS Team sees the pages and account tabs its work needs. Anything outside a role shows a "not part of this view" screen
- **Accounts:** filter by account manager, pending last-mile checks per customer, wallet balance or expected monthly billing on each customer, agreed vs actual volume, a 360 view with timeline, usage, invoices, escalations and opportunities. Accounts handed over from TSI show the full onboarding journey from the day Sales assigned them, plus next steps for the AM
- **Add update:** a button in the header (and a card on Home) to log a call, WhatsApp, email, Slack message or meeting against any customer in seconds. Visits and referrals feed their report logs
- **Timeline:** emails, Slack messages, WhatsApp, calls and meeting notes, auto-tagged by topic, sentiment, commitments and risk language
- **Notes:** pick the channel (meeting, call, WhatsApp, email or Slack); action items are pulled out of plain notes, with owner and due date
- **Onboarding and support (TSI):** new customers from Sales tracked from CRM assignment through contact, demo, integration and go-live to AM handover (contact within 30 mins, live within 5 days), plus first-line technical tickets raised by AMs (customer problems) and VS (system problems such as the field agent app), with first response within 20 mins, resolution in L1 2 hrs, L2 3 hrs, L3 48 hrs, and a push to QA. Every ticket opens for its history, notes and actions, and whoever raised it sees TSI's typed updates
- **Escalations:** one case model in both directions, reminders at 50% and 80%, auto-escalation when a standard is missed, and a "Simulate time passing" control (+15 min to +1 day). Every case has a task owner and people looped in (Admin, Head of AM, Director of VS, TSI), shows who it is waiting on and for how long, and reads as a chat. Everyone on the case sees every update, on the case and in Notifications. The VS Team logs what it pushed to coordinators off the platform. An "Address checks at risk" tab lists batches close to the 72-hour standard so the AM can ask VS to prioritise them before the customer chases
- **Escalation follow-up (Admin):** Admins cover Key or Scale accounts, chase every escalation until it is closed, log off-portal conversations with field agents, state coordinators, VS and TSI on the case, and confirm closure
- **Signals:** dropped, low and reduced volume detection, editable thresholds, and suppression during provider incidents. Customer alerts sit beside them: an occasional customer who returns after going quiet, a live customer with no first request, and a low wallet (below 20% of a normal day's spend, or empty), each with a drafted email
- **Invoices and usage logs:** AMs request an invoice for wallet funding or a prepaid service. The request is emailed to Finance from Outlook; Finance raises it in QuickBooks and replies, and the reply is matched to the request so the AM can send it on. Finance is not a workspace user. Usage logs on request for one customer, a whole AM portfolio or the customers TSI is onboarding, over any dates in the last 90 days, with a choice of services and columns, CSV download and send to customer. AMs can download any invoice with a note printed on it, send it themselves, and record it as sent. Automatic log delivery per customer (daily, weekly or monthly, to the contact they choose, for the services they choose), set by TSI during onboarding and by the AM after handover
- **Opportunities:** rule-based upsell and cross-sell suggestions with drafted emails, then Sales handoff
- **Manager dashboard:** response and resolution times, escalation aging, signal-to-action rate and revenue at risk
- **Reports:** a weekly operational report per AM (week-on-week transactions and revenue, customers to worry about, escalations and complaints, opportunities, general and strategic updates) and a monthly portfolio report (revenue against target, month-on-month and year-on-year growth, retention, revenue from newly assigned accounts, new business from upsells, lost business and churn, performance by AM), both organised around five questions: revenue, retention, growth, service delivery and execution. Weekly, monthly and quarterly views for every user, and for the Head of AM a team view with each AM, TSI, Admin and VS person's scorecard against the standards. Figures come from the system and cannot be edited; only commentary can. Plus AM approval, overdue flags and a submission tracker
- **Tasks:** anyone can give a quick task to a colleague (with an optional customer and due date); it shows in their notifications
- **Account managers:** TSI picks the AM with "Assign AM" at handover, and the Head of AM can reassign any customer. The new AM is emailed and notified
- **Data setup:** org IDs are created by QoreID when a customer opens an account. The page lists customers whose org ID is missing in Zoho CRM, with a sheet to download, fill in and upload
- **Mobile:** on a phone the workspace switches to a mobile layout: a compact header (tap your name to switch role), a bottom tab bar (Home, Alerts, Cases or the role's main page, Customers, More), customer cards instead of tables, and bottom sheets for Add update and the menu
- **Guided demo:** a 21-step walkthrough of one customer story from start to finish

**Build phases:** the Phase 1, 2 and 3 buttons in the header (or More, then Build phase, on mobile) show what each phase delivers in the same workspace.

- Phase 1, Operational visibility: Home, Accounts (Usage) and Data setup, for the AM and the Head of AM
- Phase 2, Escalations and support: adds Notifications, Escalations, Onboarding and support, Signals and customer alerts, Admin follow-up, tasks and Add update
- Phase 3, Reports and automation: adds Reports, Invoices and logs, Opportunities and the Guided demo

Switch between the five roles (Account Manager, TSI, VS Team, Admin, Head of Account Management) from the header.

## Notes

- All data, people and companies are fictional. Nothing is really sent.
- Email is assumed to run through Outlook (Microsoft 365, existing licences). WhatsApp is not integrated: WhatsApp conversations are logged by hand with Add update, like calls and meetings.
- Escalation clocks follow real team standards: AMs reply to a VS query within 15 minutes, VS resolves an escalated address check in about 2 hours, invoices take about 1 hour from request to customer, and verification itself runs 24 to 72 hours. Baseline figures are illustrative.
- The demo date is fixed at 15 October 2026 so the stories always read the same. Currency is NGN.
- Single HTML file. React 18, htm and Tailwind load from public CDNs, so there is no build step.

## Run locally

```bash
git clone https://github.com/victorobioha017-ship-it/verifyme-am-workspace.git
cd verifyme-am-workspace
open index.html   # or double-click it
```

## Author

Victor Obioha
