# Project Odin User Guide

This guide explains how to use the Project Odin dashboard without needing to understand its source code or internal file structure.

Odin is an evidence-first research and simulation system. It collects market evidence, walks the Captain through a scientific-method workflow, preserves predictions and outcomes, and lets Neo test trading rules with virtual money. It is designed to keep facts, hypotheses, decisions, and simulated trading separate.

> **Important:** Current Odin builds do not place real trades. Neo's Active Paper and Sandbox modes use virtual funds only. Add-ons are isolated from the core system and are disabled by default unless explicitly enabled.

## 1. Five-minute quick start

1. Open Odin and wait for the first successful refresh.
2. Start on **Home**. Read Market State, Current Posture, and Next Move.
3. Open **Inbox** if it shows a number. An empty Inbox means Odin is not asking you to do anything.
4. Use **Workflow** when Odin says a research stage is ready.
5. Use **Analytics** to inspect the Top 100 market snapshot and saved timeline.
6. Use **Agent** to review Neo's paper-trading experiments.
7. Use **Health Reports** if anything looks stale, broken, or unavailable.
8. Click **Refresh Odin** whenever you want the dashboard to reread saved evidence immediately.
9. Click **Check updates** to look for a newer packaged release.
10. Open **Help** whenever you need this guide.

If Odin tells you to wait for a check date, waiting is a valid action. The system is intentionally designed not to manufacture work just to look busy.

## 2. The basic idea

Odin separates four things that people routinely mash together:

- **Evidence:** what was actually observed or collected.
- **Reasoning:** what the evidence might mean.
- **Prediction:** what should happen if the reasoning is correct.
- **Outcome:** what actually happened later.

The normal research path is:

**Evidence → Observation → Hypothesis → Prediction → Objection → Decision → Outcome → Lesson**

Odin preserves each stage rather than silently rewriting old records after the fact. A failed prediction is still useful evidence.
## 3. Main navigation

### Home

Home is the executive summary. Use it to answer three questions:

- **What is happening?** Market State summarizes the current evidence.
- **What is Odin's posture?** Current Posture explains whether the system is observing, waiting, reviewing, or otherwise constrained.
- **What should I do next?** Next Move points to the next Captain-controlled step.

Use **Why does Odin think this?** when you want the supporting evidence, contrary evidence, confidence limits, and conditions that could change the current judgment.

Home is a summary, not a trading signal.

### Workflow

Workflow is the Captain-controlled research process. The stage cards show what each step means, whether it is available, and what Odin expects next.

Click a stage to read its guidance. Use the **?** button beside a stage to open its glossary explanation.

**Open Guided Workflow** launches the interactive process. Odin may recommend a next stage, but it does not silently choose answers or save decisions for you.

### Projects

Projects is the activity/change view. It surfaces large interval movements, assets that differ most from the market median, breadth changes, DOT-specific changes, and data-quality changes.

This screen answers, “What changed enough to deserve attention?” It does not answer, “What should I buy?”

### The Well

**Mímisbrunnr**, shown in the dashboard as **The Well**, is Odin's institutional-memory area. It catalogs the canonical evidence, research cycles, Neo experiment history, saved audits, and future empirical datasets that Odin has accumulated.

The depth line at the top reports how much history exists: market snapshots and observed days, Predictions → Outcomes → Lessons, Neo journal history, and empirical Forseti observations. These are depth measurements, not a claim that Odin already understands everything it has stored.

The same screen contains the glossary and explanatory material for Odin's market, evidence, and reasoning terms. Use it when a term such as Prediction, Objection, breadth, benchmark, modeled friction, or Mímisbrunnr is unclear.

The Well deliberately keeps **evidence**, **claims**, **tested results**, and **durable Lessons** distinct. A record being present does not make it proven knowledge.

### Analytics

Analytics contains the current tracked market and historical market views. The primary screens are the **Top 100** snapshot and **Timeline**.

The Top 100 view can be sorted and filtered without changing Odin's saved market data or calculations. Selecting an asset opens its evidence details.
### Agent

Agent is Neo's workspace. Neo is Odin's paper-trading and strategy-testing component.

The view selector includes:

- **Active paper** — the canonical scored Neo experiment.
- **Sandbox** — an open-ended virtual account.
- **Sandbox history** — read-only Sandbox trades, contributions, and runs.
- **Trade history** — read-only Active Paper trade history.
- **Legacy shadow history** — preserved records from the retired Shadow Neo mode.
- **Trade reviews** — saved offline proposal checks.
- **Research readiness** — whether saved data is good enough for the current forecast study.
- **Research results** — the Captain-approved saved-data research path.

Neo has no broker connection in current builds.

### Add-ons

Add-ons lists optional plugins that are deliberately isolated from core Odin.

The current Polymarket BTC 15-Minute add-on is a shadow-testing plugin. It is disabled by default and its manifest explicitly marks live execution as false.

A plugin may consume approved Odin outputs, but core Odin must not depend on the plugin.

### Health Reports

Health Reports shows Odin's current system health, evidence freshness, collection problems, dashboard errors, and recovery guidance.

Open this screen when:

- a market view says it is unavailable;
- data looks stale;
- Neo cannot load or advance;
- a collector or watchdog reports trouble;
- the dashboard refresh fails.

Health Reports is the first place to look before assuming Odin has destroyed civilization.

## 4. Top-bar controls

### Inbox

Captain Inbox is intentionally quiet. A badge such as **Inbox (1)** means Odin has something that actually requires your attention.

Examples include a due Neo review, a workflow item that needs Captain confirmation, or a health condition requiring intervention.

No badge generally means no action is required.

### Refresh Odin

Refresh rereads Odin's saved state and rebuilds the dashboard views. It does not create a trade, advance a workflow stage by itself, or rewrite research evidence.

The dashboard also refreshes automatically while it remains open.

Keyboard shortcut: **F5**.
### Check updates

Check updates immediately queries Odin's public update feed. If a newer release exists, Odin can download it and verify its SHA-256 checksum before offering to launch the installer.

Installed Odin builds also check for updates automatically on launch and periodically while open.

### Search

The search field helps locate dashboard material. Press **Ctrl+K** to focus it quickly.

Search does not change saved evidence.

### Health indicator

The status indicator near the top-right summarizes whether Odin currently considers its dashboard state healthy. Click it to open Health Reports.

## 5. Using the research workflow

### Observation — What do we see?

Record facts without adding an explanation. A good observation should be something another person could inspect or verify.

Bad observation: “DOT is about to explode.”

Better observation: “DOT gained relative strength against the tracked-market median during the saved interval.”

### Hypothesis — What might explain it?

A hypothesis proposes a possible explanation for an observation. It should be specific enough that later evidence could prove it wrong.

Odin may surface candidate hypotheses, but the Captain controls what is actually selected and saved.

### Prediction — What should happen if the hypothesis is right?

Prediction is where the idea becomes testable.

Open the guided Prediction flow and:

1. select the saved hypothesis you want to test;
2. choose a starting prediction template;
3. set or confirm the numeric success threshold;
4. review the full measurable prediction;
5. confirm the check date;
6. enter your confidence estimate;
7. explain what new evidence makes the prediction worth testing now;
8. review the complete draft before saving it.

Confidence is your estimate, not a mathematically calibrated probability unless a future system explicitly says otherwise.

### Objection — What could make us wrong?

Objection is Odin's adversarial step. Loki challenges the prediction with alternative causes, missing evidence, and reasons the apparent signal may be misleading.

The purpose is not to kill every idea. It is to make weak ideas fail before money or confidence becomes attached to them.

### Decision — What will we actually do?

Decision records the bounded action, non-action, or experiment chosen after considering the evidence and objections.

A Decision is not permission for Odin to exceed its configured authority.

### Outcome — What actually happened?

Outcome remains locked until the linked Prediction reaches its check date and valid saved evidence exists for the evaluation.

The Check-Day Assistant shows the preserved baseline, data coverage, gaps, warnings, and calculation preview. The Captain must accept or replace the suggested numeric result before the Outcome is saved.

### Lesson — What did the result teach us?

Lesson records what should be carried forward without rewriting the original Prediction or pretending the result was known in advance.
## 6. Reading the market screens

### Top 100

The current snapshot tracks 100 assets and preserves mandatory DOT coverage. If DOT falls outside the provider's top 100, Odin keeps the 99 highest-ranked assets plus DOT.

You can sort by rank, asset, symbol, price, 24-hour change, absolute movement, volume, and evidence labels. Click the active header again to reverse the order.

**Reset to Rank** restores the canonical ranking order.

Search and movement filters change only what you see on screen. They do not alter the saved snapshot.

### Selected asset details

Selecting a row shows:

- current price and movement;
- change since the previous saved snapshot;
- performance versus the tracked-market median;
- data-quality limitations;
- missing evidence;
- whether the Captain needs to do anything.

Treat this as evidence, not a recommendation.

### Timeline

Timeline turns preserved snapshots into 6-hour and 24-hour views for BTC, ETH, DOT, the tracked-market median, market breadth, and DOT's movement relative to the broader tracked market.

It also marks collection gaps and failed DOT cross-checks.

Pointer movement reveals exact saved values. Timeline never invents prices between snapshots.

### Activity / Changes

This view ranks notable interval movements and highlights unusual distance from the market median. It also surfaces breadth and data-quality changes.

It is designed to help answer, “Where should I look?” rather than “What should I trade?”

## 7. Neo: Active Paper

Open **Agent → Active paper** for Odin's canonical autonomous paper experiment.

To begin a new run:

1. make sure Odin has a current reviewed market snapshot;
2. enter the starting virtual bankroll;
3. choose the run length in whole days;
4. review the proposed paper basket;
5. select **Review & Start Active Run**;
6. confirm the locked test plan.

The current strategy can hold up to three positions and protects a 10% cash reserve. Entries and rotations use modeled fees, spread, and slippage from Forseti.

The run's strategy version is locked. Future rule changes do not rewrite an experiment already in progress.

The collector normally advances an active run after successful market collection. The dashboard itself only reads and displays that progress.
### Active Paper status card

The status card shows:

- total virtual portfolio value;
- virtual cash;
- value currently in positions;
- each holding's current paper value;
- locked run end time;
- time remaining;
- modeled trading friction.

Portfolio values include estimated exit costs so the headline reconciles with Neo's detailed accounting.

### Performance

Performance compares Neo's return after modeled costs with the locked benchmark's price return.

Use **Chart range** for Whole run, Last 24 hours, or Last 6 hours.

Click a saved point to hold its details. Previous/Next or the arrow keys move through visible saved points. **Latest** or the End key returns to the newest point.

Gaps in saved market collection break the chart rather than pretending data exists.

### Trade history

Trade history shows every verified Active Paper trade across saved runs.

Use filters to distinguish automatic rotations from Captain-approved starts and endings. Selecting a row shows quantities, reference/fill prices, fees, spread, slippage, cash change, reason, and timestamps.

Cash change is not the same thing as profit.

### Ending and scoring a run

After the locked check time, Neo stops rotating. Closing uses the first complete preserved check-time market copy and the locked benchmark.

Ending early preserves the run as incomplete and unscored. A normally completed run is scored against the plan that existed when it started.

## 8. Neo: Sandbox

Sandbox is an indefinite paper account. It is useful for watching how the same canonical strategy behaves without a fixed experiment deadline.

When starting Sandbox, choose:

- starting virtual cash;
- optional recurring virtual contribution;
- contribution schedule.

Supported schedules include daily, weekly, every two weeks, and monthly.

Sandbox keeps the protected reserve fixed at 10% of the **starting** bankroll. Later virtual contributions do not enlarge that reserve.

Contributions enter cash. They do not force a special rebalance. The normal Neo strategy decides when available cash can be deployed.

**Stop Sandbox** liquidates simulated holdings using the latest valid saved prices and preserves the completed run.

Sandbox never shares portfolio state or cash with Active Paper.
## 9. Neo research and diagnostics

### Research readiness

Research readiness answers whether Odin's saved market history is currently suitable for the approved forecast study.

It reports usable periods, sample shortfall, rejected files, collection gaps, and other blockers. A data-quality blocker is not evidence that a strategy failed. It means Odin refuses to pretend the study has cleaner evidence than it actually does.

**Check again** reruns the diagnosis. It does not repair or delete evidence.

### Research results

Research results shows the Captain-approved exclusion study using its locked rules. The screen distinguishes insufficient history from a failed data check and exposes the audit behind the summary.

**Save research audit** preserves the displayed report. **View saved audits** opens prior saved reports without rerunning the model.

A forecast error statistic is not profit and is not proof that a strategy is ready for live capital.

### Trade reviews

Trade reviews contains explicitly saved offline proposal checks. These checks compare a forecast with modeled round-trip costs, uncertainty, position limits, downside rules, objections, and other preserved assumptions.

An “eligible” review means the saved proposal passed that research gate. It is not authorization to place a real trade.

### Neo risk controls

Neo has virtual exposure controls intended to reduce damage during bad data or rapid paper losses. These controls can restrict new virtual exposure or trigger paper exits under their recorded policy.

They do not convert Neo into a live trading system.

### Forseti

Forseti is Odin's execution-friction calculator. It models costs such as fees, bid/ask spread, and slippage so a paper result is not evaluated as though trading were free.

When Neo shows “after costs,” Forseti is part of that calculation.

## 10. Add-ons

Core Odin and optional plugins are intentionally separated.

The Add-ons screen discovers plugins with manifests in Odin's plugin system. Each plugin declares what it can do, where it stores data, whether it is enabled by default, and whether it supports live execution.

The **Polymarket BTC 15-Minute** plugin currently exists for shadow testing. It compares Odin-style probability estimates with BTC 15-minute prediction-market pricing. It is disabled by default and does not have live execution authority.

Treat add-on results as separate experiments unless a future Odin version explicitly promotes a validated interface into the core research process.

## 11. Updates

Packaged Odin installations use a public binary-only update channel. The source repository remains private.

On launch and periodically while open, Odin checks the public update manifest. When a newer version is available:

1. Odin identifies the installer for the current platform;
2. the file is downloaded over HTTPS;
3. Odin calculates its SHA-256 checksum;
4. the checksum must match the published manifest;
5. Odin asks before opening the installer.

The updater does not execute a trade or overwrite your research journals simply because a new version exists.
## 12. What Odin saves

Odin uses append-only or preserved records for the parts of the system where history matters. The design goal is that a later result cannot quietly rewrite what was believed earlier.

Examples include:

- research-stage journals;
- market snapshots;
- Neo Active Paper sessions and trades;
- Sandbox sessions, trades, and virtual contributions;
- saved trade reviews;
- saved research audits.

Packaged installations keep user/runtime data separately from the installed application files. Updating or uninstalling the application is designed to preserve that local Odin data.

## 13. What Odin does not do

Current builds do **not**:

- place real brokerage or exchange orders;
- give an add-on silent authority over core Odin;
- treat a price move as proof of causation;
- call an unscored paper gain a validated strategy;
- fabricate missing market prices;
- fill collection gaps with imaginary trades;
- rewrite an old Prediction because the Outcome was inconvenient;
- automatically turn written predictions into numerical expected returns;
- treat confidence estimates as calibrated probabilities without evidence.

These restrictions are features, not missing decorative checkboxes.

## 14. Common tasks

### “What should I look at first?”

Open **Home**, then **Inbox** if it has a badge. Follow **Next Move**.

### “Something moved hard. What happened?”

Open **Projects** for notable changes, then **Analytics** and select the asset. Compare it with the tracked-market median and Timeline before forming an explanation.

### “I have an idea about why something happened.”

Use **Workflow**. Record the Observation first, then build the Hypothesis. Do not start by writing the conclusion you hope is true.

### “I want to test an idea.”

Take the workflow through Prediction, Objection, and Decision. Make the Prediction measurable and give it a check date.

### “My Prediction is due.”

Open **Inspect / Check-Day Assistant** when surfaced by Odin, review the preserved evidence, then open Outcome Review. Do not evaluate it against data that did not exist at the recorded check time.

### “I want Neo to paper-test the current strategy.”

Open **Agent → Active paper**, review the bankroll and duration, inspect the proposed basket, and explicitly confirm the run.

### “I just want a long-running virtual account.”

Use **Agent → Sandbox** instead of Active Paper.

### “Neo looks like it is getting crushed.”

Check **Performance**, **Trade history**, and **Health Reports**. Separate strategy loss from data gaps, excessive turnover, and modeled friction before changing rules.
### “Odin looks stale.”

Click **Refresh Odin**, then open **Health Reports**. Check the latest successful collection time and any collector/watchdog message.

### “I want to know whether there is a new version.”

Click **Check updates**.

### “I do not understand a term.”

Open **The Well** or use the **?** button on a Workflow stage.

## 15. Troubleshooting

### Dashboard refresh failed

Open Health Reports and read the current dashboard errors. A failed refresh does not erase existing evidence.

If a retry succeeds, the normal views will repopulate from verified saved state.

### Market data is unavailable or stale

Odin may deliberately refuse to show a current market conclusion when the underlying saved snapshot is missing, malformed, stale, or fails validation.

Do not treat “unavailable” as a hidden bearish or bullish signal. It means unavailable.

### Neo will not start

Common reasons include:

- no current reviewed market copy;
- no eligible paper holdings;
- changed test settings that require another review;
- incomplete or invalid saved market data;
- another Neo state that must be resolved first.

Read the message in the Active Paper screen and Health Reports before changing anything.

### Neo will not finish

Neo requires valid saved prices for its holdings and the appropriate preserved check-time evidence. Missing prices can block closing rather than forcing a fake valuation.

### Research readiness is blocked

Open the audit details. The diagnostic identifies rejected files and insufficient sample history. It does not automatically “fix” the evidence because doing that silently would contaminate the study.

### Update check failed

An update check can fail because of network access or GitHub availability without damaging the installed application. Odin retries packaged update checks later.
### macOS warns about the app

Current test builds may encounter Apple Gatekeeper warnings depending on signing/notarization status. Only use installers obtained from the official Project Odin downloads release.

### Windows warns about an unknown publisher

Current Windows test installers may be unsigned. Windows SmartScreen can therefore warn even when the file came from the official release. Verify that the installer came from the official Odin download channel.

## 16. Keyboard shortcuts

- **F5** — refresh Odin.
- **Ctrl+K** — focus the dashboard search field.
- **Arrow keys** — step through visible Neo Performance points when the chart has focus.
- **End** — return Neo Performance inspection to the latest point.

## 17. A note on authority

Odin is built around explicit authority boundaries.

Heimdall can block invalid or inconsistent evidence. Loki can challenge an idea. Forseti can calculate friction. Neo can run virtual experiments. Plugins can operate only inside their declared boundary.

The Captain remains responsible for decisions that require human authority.

That division is deliberate: modules should be able to disagree, evidence should be able to stop the process, and no single component should quietly become judge, historian, trader, and king.

## 18. Where to go deeper

This User Guide is the operational manual. The source repository also contains engineering documentation for architecture, module authority, principles, research methods, and development roadmap.

For ordinary use, start here. When the dashboard tells you what it needs next, follow that instruction rather than trying to manually advance every part of Odin at once.
