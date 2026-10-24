# CIFOG: CIVILIAN INTEROPERABILITY FIELD OPERATIONS GUIDE

**VERSION:** 2026.1-MASTER | **AUTHORITY:** THE ARCHITECT

> [!NOTE]
> **SOPHISTICALLY SIMPLE:** Complexity is a vulnerability. The Architect builds systems refined for immediate execution. We have done the complex work so that you don't have to.

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
