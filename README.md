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

### Currently

Working through industrial control and power generation systems, and looking for remote
work where embedded and backend meet.
