## Hey

I work where firmware meets a server. Electrical & electronics engineering background,
which mostly shows up as a habit: when the datasheet is missing or wrong, measure it.

That habit produced a hand-written 433 MHz decoder after an off-the-shelf library gave up
on a noisy receiver, and a traffic tool that turned out to be reporting *no data* as
*no traffic* — it took reading the raw API response to see the difference.

### What I build with

| | |
| --- | --- |
| **Embedded** | ESP32 / Arduino · interrupt-driven signal capture · 433 MHz RF protocol decoding · relay & actuator control |
| **Backend** | Python (asyncio, aiohttp) · MongoDB · Redis · Linux servers · systemd, cron, long-running daemons |
| **Industrial** | PLC programming (TIA Portal) · SCADA · protection and control systems · power generation plants |
| **Apps** | Swift / SwiftUI — usually for tools I need myself |

### Things I keep working on

**[OtoPosterBot](https://github.com/Pharex38/OtoPosterBot)** — Telegram channel automation.
Started in 2021 and still being edited: content forwarding, link rewriting, scheduled
delivery, ~4.900 lines across two worker processes.

**Central locking for a 24-year-old car** — an ESP32 listens to a salvaged 433 MHz receiver
and drives the door actuators. The EV1527 frame is decoded from measured edge timings,
because the noise floor on that module moves between power-up and steady state and no
fixed threshold survives both.

**A budgeting app for how credit cards actually work here** — statement cycles and payment
windows, not just a ledger. Built because the existing apps assume a billing model that
doesn't match.

### Open source

**105 merged pull requests across 37 projects.** Mostly small, focused fixes for edge cases in widely used tools.

| Project | Merged | What kind of fixes |
| --- | --- | --- |
| [diyHue](https://github.com/diyhue/diyHue/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) | 26 | Light integrations (ESPHome, WLED, Tasmota, Govee, Yeelight, Home Assistant), colour/brightness range mapping, rules and schedules |
| [i18next ecosystem](https://github.com/search?q=author%3APharex38+is%3Apr+is%3Amerged+org%3Ai18next+org%3Alocize&type=pullrequests) | 18 | i18next, react-i18next, next-i18next, i18next-cli and locize format converters: escaping, plural merging, language matching |
| [svglib](https://github.com/deeplook/svglib/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) · [ApexCharts](https://github.com/apexcharts/apexcharts.js/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) · [snapdom](https://github.com/zumerlab/snapdom/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) | 12 | Rendering and parsing edge cases |
| [Violentmonkey](https://github.com/violentmonkey/violentmonkey/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) · [Stylus](https://github.com/openstyles/stylus/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) | 6 | Date tokens across DST, `@match` ports, colour picker units |
| [Compiler Explorer](https://github.com/compiler-explorer/compiler-explorer/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) · [SchemaStore](https://github.com/SchemaStore/schemastore/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) · [Sub-Store](https://github.com/sub-store-org/Sub-Store/pulls?q=is%3Apr+author%3APharex38+is%3Amerged) | 9 | IP anonymisation, config schemas, proxy URI encoding |

Also merged in NVIDIA NeMo, electerm, mitmproxy, node-redis, Effect, pion/webrtc and others —
[full list](https://github.com/search?q=author%3APharex38+is%3Apr+is%3Amerged&type=pullrequests).

### Currently

Working through industrial control and power generation systems, and looking for remote
work where embedded and backend meet.
