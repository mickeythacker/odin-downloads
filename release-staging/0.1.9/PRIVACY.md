# Privacy and Data Handling Notice

Project Odin is currently a desktop research project, not a hosted consumer service.

The application stores research records, journals, reports, configuration, and related
runtime data in local project or configured data directories. Live `data/` evidence
is excluded from Git by project policy.

Project Odin also makes outbound network requests to third-party services when a
feature requires them. The current market-data proof of concept uses public
CoinPaprika and Coinbase Exchange endpoints. Those providers may receive ordinary
network information such as the requesting IP address and are governed by their own
privacy policies and terms.
Project Odin does not claim that using the software is anonymous or entirely offline.
Future plugins, notification services, hosted components, analytics, brokerage
connections, or other integrations may change data flows and must be documented
before release.

Do not place passwords, tokens, private keys, personally sensitive information, or
confidential third-party data into source files, test fixtures, screenshots, sample
journals, or public issue reports.

Project Odin does not sell personal information as part of its current project policy.

This notice describes the current project posture and must be reviewed whenever data
collection, cloud services, telemetry, authentication, or external account access is
added or materially changed.