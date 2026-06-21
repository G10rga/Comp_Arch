# Computer Architecture — Final Exam Question Prediction

**Subject:** Computer Hardware & Architecture (chapters 8–17)
**Source pool:** `allweeks.pdf` — 113 questions/answers
**Exam format:** 5 open (written) questions
**Method:** Pattern analysis of the lecturer's midterm emphasis (chapters 4–6), transferred forward to the final's chapters.

---

## 1. How this ranking was built

This is **not** a generic "how exams usually work" guess. It is reverse-engineered from the lecturer's *own* behavior, using the midterm document (`arkitektura 4-6.docx`) where the questions he emphasized were marked in **green**.

Decoding the midterm colors revealed:

- **Green `00B050`** = emphasized questions
- **Blue `1F3864` / `002060`** = normal (not emphasized) questions
- **Red `EE0000`** = lecture/chapter headers
- **Black `000000`** = answers

### What the lecturer EMPHASIZED (green)

1. **Named technologies** — *every single* "Intel X technology" question was green (Wide Dynamic Execution, Intelligent Power Capability, Advanced Smart Cache, Smart Memory Access, Advanced Digital Media Boost, Turbo Boost, Tick-Tock, Process-Architecture-Optimization), plus MMX, SSE, AVX, Hyper-threading, NetBurst.
2. **Comparison / “შედარებითი ანალიზი” questions** — Xeon vs Core, Pentium D vs Extreme Edition, PGA vs PGA2 vs SPGA, Socket vs Slot, LGA vs predecessors, passive vs active cooling, multiprocessor mode comparison.
3. **Mechanism / “how it works” concepts** — superscalar architecture, dynamic execution, branch prediction, speculative execution, data-flow analysis, micro-ops cache, hyperpipelining.

### What the lecturer DE-EMPHASIZED (blue)

1. **Basic “purpose / definition” questions** — “what is a CPU’s purpose,” “which firms make CPUs,” “list the main characteristics,” “cache purpose,” “addressable-memory formula.” All blue.
2. **Plain historical-model descriptions** — “describe Pentium I/II/III/4/D features.” All blue.
3. **Overclocking *methods* and pure calculations.** Blue.

**Conclusion / fingerprint:** *He tests named technologies, comparisons, and mechanisms — not textbook definitions, spec sheets, or arithmetic.*

### How that maps onto the final (chapters 8–17)

| Midterm signal (green) | Final-exam analog (ranked high) |
|---|---|
| Every Intel-technology question | ch.14 Q9–Q14 (Quiet System, Fast Memory Access, Clear Video, HD Audio, Turbo Memory, Matrix Storage) |
| Comparison questions | SATA vs ATA, PCI vs PCIe, USB 2.0 vs 3.0, DRAM vs SRAM, single-ended vs differential, CD-DA vs CD-ROM, DDR4 vs DDR3 |
| Mechanism/concept questions | serial vs parallel, differential transmission, FSB/DMI, zone-bit recording |
| “Core i” was heavily greened | ch.14 Q15 Core i platform |

| Midterm signal (blue) | Final-exam analog (ranked low) |
|---|---|
| “Purpose / which firms” (Q1+Q2) | ch.8 Q1 ROM purpose, ch.8 Q2 BIOS purpose+firms |
| “List the main characteristics” | ch.15 Q1 sector/track/cylinder + list parameters |
| Calculations & overclocking methods | all calc questions, all connector pinouts |

---

## 1b. Compound-question structure (important)

A key structural fact: this lecturer's open questions are frequently **two basic questions stapled into one** — “describe X … *and* describe/compare Y.” The midterm confirms it; many green questions were already two-part:

- “Quartz resonator **and** clock generator purpose”
- “Multiprocessor system essence. **What conditions** must a computer meet…”
- “Multiprocessor modes. **Comparative analysis** of them”
- “Math coprocessor purpose? **When** is it effective…”
- “PGA, PGA2 **and** SPGA … **comparative analysis**”
- “Socket vs Slot … **and** what drove Slot in Pentium II”
- “Radiator materials **and** how it is mounted”
- “Passive **and** active cooling … **when** is each used”

### Two consequences for the final

1. **Inherently two-part questions get a boost** — a single question that already contains two parts is exactly his preferred shape. This *rescues* a few questions I had demoted (notably **ch.15 Q1**, which is “sector/track/cylinder essence **+** list main parameters” — a textbook two-part).
2. **Two related single-topic questions may be merged** — so studying *pairs* of neighboring topics together is smart, because the exam may ask both halves in one question.

### Most probable compound pairings (study these as a unit)

| Likely combined question | Parts |
|---|---|
| Color modes | ch.17 Q6 (Hi-Color/Real Color) **+** Q7 (True Color) |
| Writable optical discs | ch.16 Q3 (CD-R) **+** Q4 (CD-RW) |
| File systems | ch.15 Q14 (FAT32/exFAT) **+** Q15 (NTFS) |
| PSU control signals | ch.13 Q4 (Power Good) **+** Q5 (Power_On / +5V Stand By) |
| Wireless/flexible USB | ch.12 Q6 (USB OTG) **+** Q7 (USB Wireless) |
| Data transmission | ch.10 Q3 (single-conductor) **+** Q4 (differential), or framed as Q5 comparison |
| Monitor operating modes | ch.17 Q1 (text/alphanumeric) **+** Q2 (graphics) |
| Intel technologies | any two of ch.14 Q9–Q14 asked together |
| DDR generations | e.g. ch.9 Q17 (DDR3) **+** Q20 (DDR4) |
| ROM | ch.8 Q1 (ROM purpose) **+** Q9 (ROM chip types) |

> **Note:** the “monitor modes” (ch.17 Q1+Q2) and “ROM” (ch.8 Q1+Q9) pairings are the main reason some Tier-C items can still surface — individually weak, but a natural two-part combo. Likewise **ch.15 Q1** effectively moves up from Tier C toward Tier B because it is already a compound question.

---

## 2. Full ranking (1 → 113, most → least likely)

### 🟩 Tier S — his clear favorites (study first)

| # | Chapter | Q# | Topic | Why |
|---|---|---|---|---|
| 1 | ch.11 | Q4 | SATA vs ATA | Comparison — his #1 favorite format |
| 2 | ch.8 | Q8 | UEFI vs classic BIOS | Named modern tech + comparison |
| 3 | ch.10 | Q5 | Single-ended vs differential bus | Comparison |
| 4 | ch.9 | Q6 | DRAM vs SRAM | Comparison |
| 5 | ch.12 | Q9 | USB 2.0 vs USB 3.0 | Comparison |
| 6 | ch.10 | Q11 | PCI vs PCI Express | Comparison |
| 7 | ch.16 | Q1 | CD-DA vs CD-ROM | Comparison |
| 8 | ch.14 | Q15 | Core i architecture platform | “Core i” block was heavily greened at midterm |
| 9 | ch.15 | Q6 | SMART | Named technology |

### 🟦 Tier A — named technologies & mechanisms (strongly favored)

| # | Chapter | Q# | Topic | Why |
|---|---|---|---|---|
| 10 | ch.14 | Q9 | Intel Quiet System | Every Intel-tech question was green at midterm |
| 11 | ch.14 | Q10 | Intel Fast Memory Access | Intel-tech block |
| 12 | ch.14 | Q11 | Intel Clear Video | Intel-tech block |
| 13 | ch.14 | Q12 | Intel High Definition Audio | Intel-tech block |
| 14 | ch.14 | Q13 | Intel Turbo Memory | Intel-tech block |
| 15 | ch.14 | Q14 | Intel Matrix Storage | Intel-tech block |
| 16 | ch.14 | Q8 | Legacy Free architecture | Named architecture concept |
| 17 | ch.14 | Q1 | FSB / DMI function | Core architecture mechanism |
| 18 | ch.13 | Q4 | Power Good signal | Named signal/mechanism |
| 19 | ch.13 | Q5 | Power_On / +5V Stand By | Named signal/mechanism |
| 20 | ch.15 | Q2 | Zone bit recording | Named mechanism |
| 21 | ch.10 | Q1 | Serial vs parallel transmission | Mechanism + implicit comparison |
| 22 | ch.12 | Q6 | USB On-The-Go (OTG) | Named technology |
| 23 | ch.17 | Q7 | True Color | Named mode |
| 24 | ch.17 | Q6 | Hi-Color / Real Color | Named modes + comparison |
| 25 | ch.16 | Q3 | CD-R technology | Named technology |
| 26 | ch.16 | Q4 | CD-RW technology | Named technology |
| 27 | ch.9 | Q11 | DDR technology | Named technology |

### 🟨 Tier B — likely

| # | Chapter | Q# | Topic | Why |
|---|---|---|---|---|
| 28 | ch.9 | Q13 | DDR2 technology | Named tech (“არსი” phrasing = green pattern) |
| 29 | ch.9 | Q17 | DDR3 technology | Named tech |
| 30 | ch.9 | Q20 | DDR4 technology | Named tech |
| 31 | ch.9 | Q27 | DDR5 | Named tech |
| 32 | ch.9 | Q22 | DDR3/DDR4 bus comparison | Comparison |
| 33 | ch.9 | Q28 | DDR5 vs DDR4 | Comparison |
| 34 | ch.9 | Q23 | DDR4 vs DDR3 voltage | Comparison |
| 35 | ch.9 | Q24 | DDR4 vs DDR3 capacity | Comparison |
| 36 | ch.9 | Q26 | DDR4 vs DDR3 modules | Comparison |
| 37 | ch.9 | Q25 | DDR4 energy-efficiency cause | Mechanism |
| 38 | ch.10 | Q4 | Differential transmission | Mechanism |
| 39 | ch.10 | Q3 | Single-conductor transmission | Mechanism |
| 40 | ch.10 | Q13 | PCI Express encoding | Mechanism |
| 41 | ch.10 | Q10 | PCI Express characteristics | Named bus |
| 42 | ch.10 | Q2 | Interface development trends | Concept |
| 43 | ch.10 | Q12 | Compatibility principle | Concept |
| 44 | ch.8 | Q7 | Low- vs high-level drivers | Comparison/mechanism |
| 45 | ch.8 | Q5 | BIOS load process | Mechanism |
| 46 | ch.16 | Q2 | Reading info from CD | Mechanism |
| 47 | ch.16 | Q12 | UDF | Named file system |
| 48 | ch.15 | Q14 | FAT32 / exFAT | Named file systems + comparison |
| 49 | ch.15 | Q15 | NTFS | Named file system |
| 50 | ch.12 | Q7 | USB Wireless | Named technology |
| 51 | ch.14 | Q5 | I/O Controller Hub | Named component/mechanism |
| 52 | ch.11 | Q5 | SATA standards | Named-tech adjacent |
| 53 | ch.11 | Q7 | SATA organizational structure | Mechanism |
| 54 | ch.11 | Q8 | SATA physical layer | Mechanism |
| 55 | ch.11 | Q10 | SATA channel layer | Mechanism |
| 56 | ch.11 | Q11 | SATA error detection/correction | Mechanism |
| 57 | ch.12 | Q8 | USB 3.0 standard | Named-tech adjacent |
| 58 | ch.12 | Q4 | USB 2.0 transfer modes | Mechanism |
| 59 | ch.9 | Q16 | Memory timing | Concept |
| 60 | ch.9 | Q21 | DDR4 error detection/correction | Mechanism |

### ⬜ Tier C — de-emphasized (definition / spec types)

| # | Chapter | Q# | Topic | Why low |
|---|---|---|---|---|
| 61 | ch.8 | Q1 | ROM purpose | “Purpose” definition — blue at midterm |
| 62 | ch.8 | Q2 | BIOS purpose + manufacturers | Direct analog to blue midterm Q1+Q2 |
| 63 | ch.15 | Q1 | Sector/track/cylinder + list parameters | Analog to blue “list main characteristics” |
| 64 | ch.13 | Q1 | PSU purpose | “Purpose” definition |
| 65 | ch.15 | Q5 | HDD cache purpose | “Purpose” definition (cache purpose was blue) |
| 66 | ch.12 | Q1 | USB port advantages | Basic listing |
| 67 | ch.9 | Q3 | RAM structure | Basic description |
| 68 | ch.9 | Q4 | Register memory | Basic description |
| 69 | ch.9 | Q2 | Program load order | Basic description |
| 70 | ch.11 | Q2 | ATA objects | Spec listing |
| 71 | ch.17 | Q3 | Resolution | Basic definition |
| 72 | ch.17 | Q1 | Text (alphanumeric) mode | Basic description |
| 73 | ch.17 | Q2 | Graphics mode | Basic description |
| 74 | ch.17 | Q5 | VGA analog signals | Narrow concept |
| 75 | ch.17 | Q8 | VGA / DVI / HDMI | Comparison (saves it from Tier D) but interface-spec heavy |
| 76 | ch.8 | Q4 | BIOS subprograms | Listing |
| 77 | ch.8 | Q6 | POST results | Listing |
| 78 | ch.8 | Q9 | ROM chip types | Listing |
| 79 | ch.8 | Q3 | CMOS Setup location/power | Narrow spec |
| 80 | ch.13 | Q6 | ATX standard | Standard description |
| 81 | ch.16 | Q11 | CD writing methods | Listing |
| 82 | ch.15 | Q7 | SMART analyzed parameters | Listing (the SMART *concept* ranks high, this listing does not) |
| 83 | ch.15 | Q12 | Low-level formatting | Narrow |
| 84 | ch.15 | Q13 | Partitioning | Narrow |
| 85 | ch.15 | Q16 | Logical formatting | Narrow |
| 86 | ch.15 | Q8 | Register filter | Narrow component |
| 87 | ch.15 | Q9 | Barometric filter | Narrow component |
| 88 | ch.15 | Q10 | Cache types | Listing |
| 89 | ch.9 | Q7 | DIP array drawbacks | Narrow spec |

### 🟥 Tier D — lowest (calculations, pinouts, spec trivia — all blue at midterm)

| # | Chapter | Q# | Topic | Why lowest |
|---|---|---|---|---|
| 90 | ch.13 | Q2 | PSU output voltages | Spec list |
| 91 | ch.13 | Q8 | 20-pin connector | Pinout |
| 92 | ch.13 | Q12 | 24-pin connector | Pinout |
| 93 | ch.13 | Q9 | ATA connector | Pinout |
| 94 | ch.13 | Q10 | SATA connector | Pinout |
| 95 | ch.13 | Q13 | 4-pin ATX 12V | Pinout |
| 96 | ch.13 | Q14 | 6-pin ATX 12V | Pinout |
| 97 | ch.13 | Q15 | 8-pin ATX 12V | Pinout |
| 98 | ch.13 | Q18 | Video adapter power options | Spec |
| 99 | ch.12 | Q5 | USB 2.0 connectors/pins | Pinout |
| 100 | ch.12 | Q10 | USB 3.0 connectors/pins | Pinout |
| 101 | ch.11 | Q13 | SATA cable pins | Pinout |
| 102 | ch.9 | Q31 | DDR2 min frequency | Calculation |
| 103 | ch.9 | Q32 | DDR3 min frequency | Calculation |
| 104 | ch.9 | Q33 | DDR4 min frequency | Calculation |
| 105 | ch.10 | Q20 | PCIe bandwidth | Calculation |
| 106 | ch.10 | Q21 | PCIe bandwidth | Calculation |
| 107 | ch.13 | Q16 | CPU power | Calculation |
| 108 | ch.13 | Q17 | CPU power | Calculation |
| 109 | ch.13 | Q19 | Video adapter power | Calculation |
| 110 | ch.13 | Q20 | Video adapter power | Calculation |
| 111 | ch.15 | Q3 | Average seek time | Calculation |
| 112 | ch.15 | Q4 | Transfer rate | Calculation |
| 113 | ch.16 | Q5 | CD-ROM transfer rate | Calculation |

---

## 3. Bottom line

If betting on the 5 open questions, lock in **Tier S** plus the **ch.14 Intel-technology block** (Tier A). Comparisons + named technologies are this lecturer's fingerprint, and chapters 14–17 are rich in exactly that.

Because his questions are typically **two-part**, prepare answers as *pairs*: for each Tier S/A topic, also be ready for a likely “… and describe/compare [neighboring topic]” second half (see the compound-pairing table in section 1b).

**Caveat:** the midterm covered chapters 4–6 (processors); the final covers 8–17. This transfers his *style* forward (reliable), but a second emphasized midterm would tighten the prediction further. The single strongest override is anything he explicitly stressed in lectures.
