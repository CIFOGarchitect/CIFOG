# CIFOG: CIVILIAN INTEROPERABILITY FIELD OPERATIONS GUIDE

**VERSION:** 2026.2 | **AUTHORITY:** THE ARCHITECT

> [!NOTE]
> **SOPHISTICALLY SIMPLE:** Complexity is a vulnerability. The Architect builds systems refined for immediate execution. We have done the complex work so that you don't have to.

> [!IMPORTANT]
> **LICENSING & USE:** This guide teaches and organizes. It does not authorize anyone to transmit on any frequency. Use only the frequencies and services you are authorized for, under the rules of that service, with the proper FCC authorization or licensing. Channels listed for monitoring are receive-only: listen, do not transmit.

---

## INTRODUCTION: FUNDAMENTALS

Interoperability means this: different people, with different radios, can still talk to each other when it matters. Everything in this guide serves that one idea. If you understand the fundamentals below, the rest of the guide is just details.

**The escalation ladder.** When you need to get a message through, work this ladder from the top down, and stop at the first method that works:

1. Face to face, where possible.
2. Your local, everyday method (cell, mesh, home).
3. A shared system your group already uses.
4. A mutual-aid channel both sides have (for CIFOG groups, the Vanguard channels).
5. A gateway or patch between two systems, if one is available.
6. A cache radio handed to someone who needs one.
7. A relay: a person carries the message.

The ladder is the whole philosophy. Never depend on a single method. Always know the next step down.

**PACE is the ladder, made personal.** Primary, Alternate, Contingency, Emergency. Section II gives you the table; the idea is older than the table: always have a backup to the backup, and know what it is *before* you need it.

**Same names in every radio.** Every radio in the group programs these channels with identical names. If one radio calls it WARPIGEON and another calls it something else, you do not have interoperability — you have confusion. Program alike, verify after programming, and re-verify after any change.

**A tone is not privacy.** DPL and CTCSS tones only filter what your speaker plays. Anyone tuned to the frequency hears everything you transmit, tone or not. Never say anything on the radio you would not say in a room full of strangers.

**Say who you are first.** Announce your group and identifier before your message, every time. ("[Group], [identifier] — message.") On a shared channel, nobody can answer you if they don't know who you are.

**Strict net control, and someone always listening.** During any activation, one station runs the net, and one station keeps a listening watch on the calling channel (WARPIGEON). Uncontrolled channels fill up, and filled channels fail. Net control keeps the channel clear for traffic that matters.

**How to read a channel entry.** Every channel in this guide has five parts: callsign (the name you say on the air), frequency (where it lives), tone/DPL (the code that opens squelch), mode (how the signal is carried — the Vanguard channels are analog narrowband FM), and purpose (what the channel is for). Example: WARPIGEON — 151.625 MHz, DPL 023, analog narrowband, command and calling. If you can read one entry, you can read them all.

---

## I. OPERATIONAL DOCTRINE

### 1.1 Radio Etiquette

- **LISTEN FIRST:** Monitor for 30 seconds before transmitting.
- **1-SECOND RULE:** Key the mic, wait 1 second, then speak.
- **PLAIN LANGUAGE:** No 10-codes. Use: *Copy, Affirmative, Negative, Wait, Say Again.*

### 1.2 LCAN Reporting Format

Use this structure for all status updates:

- **L - Location:** Your current position.
- **C - Conditions:** Fire, Medical, Flood, or All Clear.
- **A - Actions:** What you are doing now.
- **N - Needs:** Resources required.

Worked example (fill in your own details):

> "WARPIGEON, this is [group] [identifier] — Location: north trailhead parking lot. Conditions: All Clear. Actions: moving to checkpoint two. Needs: none."

---

## II. PERSONAL ADAPTIVE COMMS (PACE)

*Failure to plan is planning to fail.*

| LEVEL | METHOD | CHANNEL / FREQ | TONE / DPL |
| --- | --- | --- | --- |
| **P - PRIMARY** | **Local/Daily** | Cell / Mesh / Home | N/A |
| **A - ALTERNATE** | **Vanguard 01** | 151.625 MHz | DPL 023 |
| **C - CONTINGENCY** | **3-3-3 Rule** | MURS 3 / GMRS 3 | CSQ |
| **E - EMERGENCY** | **Interop Monitor** | VTAC11 / UTAC1 | RX ONLY |

> [!TIP]
> **THE 3-3-3 RULE:** On the 3rd hour, tune to CH 3, listen/transmit for 3 minutes.

---

## III. THE VANGUARD 16 (TACTICAL OVERLAY)

*Standardized Analog Tactical Zone. All channels use **DPL (Digital Private Line)**.*

| CH | CALLSIGN | FREQ (MHz) | DPL | PURPOSE |
| --- | --- | --- | --- | --- |
| **01** | **WARPIGEON** | 151.625 | 023 | **COMMAND:** Main Muster/Calling. |
| **02** | **PRIVATE 1** | 151.820 | 023 | User Defined Family Channel 1 |
| **03** | **PRIVATE 2** | 151.880 | 023 | User Defined Family Channel 2 |
| **04** | **RAZORBACK** | 151.505 | 032 | **LOGISTICS:** Convoy/Heavy Equipment. |
| **05** | **GHOSTWALK** | 154.5275 | 043 | **TECH OPS:** Setup & Testing. |
| **06** | **NIGHTHAWK** | 464.500 | 047 | **INDOOR:** Deep-structure/Industrial. |
| **07** | **BULLSEYE** | 464.550 | 051 | **SECURITY:** Gate & Perimeter. |
| **08** | **VULCAN** | 469.500 | 054 | Vanguard Maintenance |
| **09** | **COBALT** | 469.550 | 065 | Vanguard Admin |
| **10** | **SABRE** | 151.700 | 071 | Vanguard Perimeter |
| **11** | **VORTEX** | 151.760 | 072 | Vanguard Alert |
| **12** | **RAPTOR** | 467.7625 | 073 | Vanguard Courier |
| **13** | **TITAN** | 467.8125 | 074 | Vanguard PM |
| **14** | **REVENANT** | 151.895 | 114 | Vanguard Shadow |
| **15** | **OVERLORD** | 151.925 | 115 | **ALL-CALL:** Emergency Muster. |
| **16** | **BLACKOUT** | 154.600 | 116 | **SILENCE:** Emergency Protocol. |

*Matches Vanguard16_Master.csv.*

---

## IV. VANGUARD AUTHENTICATION & VECTOR MATRIX

**"The signal is the truth. The seed is the key."** To shift channels securely, Overlord will broadcast a **Vector**. Add the Vector to the **Daily Seed** to find the target channel. (*Formula: Vector + Seed = Channel*)

| DAY | SEED | DAY | SEED | DAY | SEED | DAY | SEED |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **01** | 04 | **09** | 11 | **17** | 08 | **25** | 05 |
| **02** | 12 | **10** | 06 | **18** | 12 | **26** | 10 |
| **03** | 07 | **11** | 09 | **19** | 04 | **27** | 02 |
| **04** | 01 | **12** | 02 | **20** | 15 | **28** | 09 |
| **05** | 10 | **13** | 15 | **21** | 03 | **29** | 07 |
| **06** | 03 | **14** | 06 | **22** | 11 | **30** | 13 |
| **07** | 14 | **15** | 13 | **23** | 08 | **31** | 01 |
| **08** | 05 | **16** | 01 | **24** | 14 |  |  |

*Complete 31-day table — matches the Vanguard Authentication Key Card.*

---

## V. STATUS CODES

*From the Vanguard Authentication Key Card.*

| CODE | STATUS | MEANING |
| --- | --- | --- |
| **10** | Green | Normal |
| **20** | Yellow | Instability |
| **30** | Orange | Emergency |
| **40** | Red | Grid Down |
| **99** | Black | Threat/Silence |

---

## VI. GROUP ROLES & NET CONTROL

A channel plan without people to run it is just a list. Every group using CIFOG names these roles, with a backup for each:

- **OVERLORD (net control).** Runs the net. Declares all-calls and silence, broadcasts Vectors, lifts silence, stands the net down. One net control per net — if two groups merge, agree on one net control first, before operating together.
- **Monitor.** Keeps a listening watch on WARPIGEON during any activation and logs traffic.
- **Logger.** Keeps the written log: times, stations, messages, problems. If it isn't logged, it didn't happen.
- **Tech.** Keeps every group radio programmed alike, charged, and tested. Owns the cache (Section VIII).
- **Every member.** Knows the plan, keeps their keycard current, checks in when called.

**Adopting CIFOG as a group.** Keep it lightweight, but do it deliberately: agree on the plan and its version, program every radio alike, name the roles and backups, set a test cadence (Section VII), and review changes together. When the guide version changes, re-print the keycards. A group that has never practiced together does not have a plan — it has a document.

**When groups merge.** Agree on three things before operating together: one net control, one common channel plan, and how callsigns work across groups. Then operate as one net. Two nets on one channel is not interoperability.

---

## VII. ACTIVATION & PROCEDURES

**Activation sequence.** When the group needs to operate:

1. Need identified — a member or net control calls for activation.
2. Verify a common channel — every station confirms it has the current plan before anyone moves.
3. Check in — stations check in on WARPIGEON, group and identifier first.
4. Net control posts the working channel(s) and the plan for the operation.
5. Operate — net control directs traffic; all other stations wait for direction.
6. Stand down — net control announces return to normal operations, stations acknowledge, and the activation is logged.

**All-call (OVERLORD).** When OVERLORD declares an all-call, all stations switch to channel 15 (OVERLORD) and check in. Net control directs traffic from there. WARPIGEON remains the day-to-day calling channel; OVERLORD is the emergency muster channel.

**Silence (BLACKOUT).** When OVERLORD declares silence, all stations cease transmitting immediately and monitor channel 16 (BLACKOUT) until OVERLORD lifts silence. The only exception is immediate life-safety traffic. Only OVERLORD lifts silence.

**Vector procedure.** OVERLORD broadcasts the Vector in plain language on the active net channel ("Vector 3"). Each station adds the Vector to today's seed from the keycard and switches to the resulting channel. If the result is not a valid channel (1–16), disregard it and await a corrected Vector — do not guess, and do not wrap around.

**Stand-down and after-action.** Every activation and every exercise ends twice: once on the air (net control stands the net down, stations acknowledge) and once on paper (a short hot wash: what worked, what didn't, what changes). Lessons go back into the plan, or they will be re-learned the hard way.

**Testing cadence.** A plan that is never tested is a guess. Proposed cadence: a brief weekly check-in on WARPIGEON, and a monthly net that exercises one PACE fallback (one month the alternate channel, another month the 3-3-3 contingency). Test the cache radios monthly: charge, power on, check in.

**Troubleshooting.** If you cannot reach the group: check channel, then tone, then battery, then antenna, then position (move higher or clearer). If still nothing, fall back per PACE. If still nothing, relay through another station. Then fall to contingency at the next 3-3-3 window. Work the ladder — never sit on a dead channel hoping.

---

## VIII. PROGRAMMING & EQUIPMENT

**Programming template.** Every group radio gets the full Vanguard zone, with identical names, as its base. Family PRIVATE channels are added per group on top of the base — never instead of it. After programming, verify by read-back: channel, frequency, tone. After any change, verify again. Never improvise programming mid-incident; mismatched radios are how nets fail.

**Group cache.** A box of charged spare radios, programmed identically to the group's radios, stored in a known place, with a named keeper and a checkout/return log. Spares are checked monthly: charge, power on, check in. A cache nobody maintains is a box of dead weight.

**Asset list.** One page, kept with the plan: member, callsign, radio(s), bands, mobile or portable, vehicle rig, notes. Update it when gear changes. A group that doesn't know what it owns cannot plan around it.

**Amateur radio bridge.** Licensed amateur operators and volunteer groups are a real resource: wider nets, repeaters, and experienced operators. Know your local clubs and repeaters — look them up through current directories rather than relying on printed lists that go stale. Transmitting on amateur bands requires an amateur license; the bridge works because hams are licensed, trained, and practiced.

---

## IX. READINESS SELF-ASSESSMENT

Grade your group honestly. Any unchecked box is your next job.

- [ ] A written plan adopted by the group, with a named net control and backup.
- [ ] Every radio programmed alike, names identical, tested on the air.
- [ ] Keycards printed, current, and matching the guide version.
- [ ] Cache charged, tested, and its keeper named.
- [ ] Every PACE level exercised at least once in practice.
- [ ] A test cadence running: weekly check-in, monthly net.
- [ ] A log habit: activations and exercises logged.
- [ ] An after-action habit: short hot wash after every exercise and activation, lessons folded into the plan.
- [ ] Version control: the group knows which version it runs, and changes are reviewed together.
- [ ] A fallback for total radio failure: runners, meeting points, the relay step of the ladder.

---

## X. WATCH-OUTS

Learn these before they teach you:

- **Congestion.** Too many voices on one channel. Net control directs; everyone else waits.
- **Unfamiliar radio.** You cannot run what you have never practiced on. Train on your own radio.
- **Unclear assignments.** If you don't know your job, ask before transmitting.
- **Dead zones.** Buildings, garages, and valleys kill signal. Move, elevate, or relay.
- **No net control.** Two nets on one channel with nobody directing is not a net.
- **Different words.** Groups using different terms for the same thing cause confusion. Plain language, always.
- **Dead batteries and untested gear.** Check before you need it, not during.
- **Assuming privacy.** DPL and CTCSS are not encryption. Anyone on the frequency hears you.
- **Programming at the incident.** Multiple people reprogramming creates mismatched radios. Program before, verify after.
- **Too few channels.** If the working channel is busy, net control moves traffic — don't just pile on.
- **The emergency you didn't plan for.** Know your group's emergency procedure before you need it, including what happens when someone breaks silence with life-safety traffic.

---

## APPENDIX: GLOSSARY

- **Cache.** Spare radios and equipment held in reserve for issue.
- **Callsign.** The name a station uses on the air (in CIFOG, the Vanguard channel names double as callsigns for the net).
- **CSQ (carrier squelch).** No tone or code; any signal on the frequency opens the speaker.
- **CTCSS.** Continuous Tone-Coded Squelch System — a sub-audible tone that opens squelch only for matching signals. Filtering, not privacy.
- **Direct / simplex.** Radio-to-radio without a repeater (talk-around).
- **DPL (Digital Private Line).** A digital code that opens squelch only for matching signals. Filtering, not privacy, not encryption.
- **Gateway / patch.** A connection between two systems or channels so users on each can hear each other.
- **GMRS.** General Mobile Radio Service — a licensed UHF service for families and groups.
- **ICS / NIMS.** Incident Command System / National Incident Management System — the standard framework for managing incidents.
- **Keycard.** The printed card carrying the seed table and status codes, kept with the radio.
- **LCAN.** Location, Conditions, Actions, Needs — the status report format (Section I).
- **MURS.** Multi-Use Radio Service — a license-free VHF short-range service.
- **Muster.** A gathering or check-in, on the air or in person.
- **Net control.** The station directing traffic on a net (in CIFOG, OVERLORD).
- **NFM.** Narrowband FM — the voice mode used by the Vanguard channels.
- **NIFOG.** National Interoperability Field Operations Guide (CISA) — the national model CIFOG adapts for civilian use.
- **PACE.** Primary, Alternate, Contingency, Emergency — a layered plan so losing one method never leaves you with nothing.
- **Repeater.** A station that receives and retransmits signals to extend range.
- **Seed.** The daily number from the keycard, added to a broadcast Vector to find the target channel.
- **Vector.** A number broadcast by OVERLORD; Vector + Seed = Channel.
- **VTAC / UTAC.** National interoperability tactical channel names. V = VHF, U = UHF; TAC = tactical (CALL = calling). In CIFOG's PACE these are monitor-only for civilians: listen, do not transmit.

---

## VERSION NOTES

- **2026.2** — Adds fundamentals, licensing note, group roles, activation & procedures, programming & equipment, readiness self-assessment, watch-outs, and glossary.
- **2026.1** — First full sync: all 16 Vanguard channels, complete 31-day seed table, status codes.
