# VerifyMe Account Management Workspace

A clickable concept prototype for an account management workspace built around identity verification services. It shows how account managers, verification agents, finance and team leads could work from one shared view of every customer.

**Live demo:** open `index.html` in a browser, or visit https://victorobioha017-ship-it.github.io/verifyme-am-workspace/.

## What you can try

- **Home:** portfolio health, open signals, escalations with live SLA clocks, and tasks due today
- **Accounts:** agreed vs actual volume, a 360 view with timeline, usage, invoices, escalations and opportunities
- **Timeline:** emails, Slack messages and meeting notes, auto-tagged by topic, sentiment, commitments and risk language
- **Meeting notes:** action items pulled out of plain notes, with owner and due date
- **Escalations:** one case model in both directions, reminders at 50% and 80%, auto-escalation on breach, and a "Simulate time passing" control
- **Signals:** dropped, low and reduced volume detection, editable thresholds, and suppression during provider incidents
- **Invoices and logs:** requests checked against contract rules, auto-approval for standard cases and a Finance queue for exceptions
- **Opportunities:** rule-based upsell and cross-sell suggestions with drafted emails, then Sales handoff
- **Manager dashboard:** response and resolution times, escalation aging, signal-to-action rate and revenue at risk
- **Guided demo:** an 11-step walkthrough of one customer story from start to finish

Switch between the four roles (Account Manager, Verification Services Agent, Finance, Head of Account Management) from the header.

## Notes

- All data, people and companies are fictional. Nothing is really sent.
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
