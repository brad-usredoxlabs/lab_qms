# M-FA-001 — Fatty Acid Composition by GC‑FID (FAME)

**US Redox Labs (USRL) — ISO 17025 Quality Manual**

- **Revision:** 0
- **Effective Date:** 2025‑08‑05
- **Supersedes:** N/A
- **Prepared by:** Brad Marshall
- **Approved by:** __________________________

---

## 1 Purpose

To quantify total fatty‑acid composition of food products by converting lipids to fatty‑acid methyl esters (FAME) and separating them on a gas chromatograph equipped with a flame‑ionisation detector (GC‑FID), following AOAC 996.06/991.39 with automation on the Integra Assist Plus liquid‑handling platform.

## 2 Scope

Applies to all routine client or in‑house food samples (solid, semi‑solid, liquid, dairy, meat, egg, plant, processed foods) analysed at USRL using GC‑FID system EQ‑GC‑001.

## 3 Principle

Lipids are extracted or saponified in situ, trans‑esterified to FAME, cleaned by SPE‑magnetic beads, dried, reconstituted and injected onto a highly polar cyanopropyl column (Restek Rt‑2560, 100 m × 0.25 mm × 0.20 µm). Separation is achieved with hydrogen carrier gas and detected by FID. Quantification is based on an external multi‑point calibration with internal‑standard normalisation (C19:0 FAME).

## 4 Responsibilities


| Role                | Responsibility                                        |
| --------------------- | ------------------------------------------------------- |
| Laboratory Director | Approves method, ensures resources & compliance       |
| Analysts            | Execute procedure, maintain records, perform daily QC |
| QA Manager         | Audits records, reviews QC & proficiency data         |

## 5 Definitions

- **FAME** – Fatty‑acid methyl ester
- **IS** – Internal standard (C11:0)
- **QC‑1** – Certified reference material (NIST SRM 1849a or equivalent)

## 6 References

1. AOAC Official Method 996.06 & 991.39.
2. ISO 17025:2017.
3. Manufacturer operating manuals (Agilent 6890 GC, Integra Assist Plus, Bio‑Spec Mini‑BeadBeater 96, LabConco Centrivap).

## 7 Safety & Environmental

- Wear lab coat, safety glasses, nitrile gloves.
- Work with flammables (hexane, heptane, methanol) inside a fume hood.
- Collect solvent waste in labelled fire‑safe containers for disposal by licensed vendor.

## 8 Equipment & Materials


| Item            | Model / Spec                                          |
| ----------------- | ------------------------------------------------------- |
| GC‑FID         | Agilent 6890N with FID & 7683 autosampler            |
| Column          | Restek Rt‑2560, 100 m × 0.25 mm × 0.20 µm  |
| Carrier Gas     | Hydrogen generator, 99.999 % purity                  |
| Liquid‑Handler | Integra Assist Plus w/ 8‑ch Voyager 12.5–300 µL |
| HEATMAG Module  | Heated magnetic plate for 96‑well SPE                |
| Bead Mill       | Bio‑Spec Mini‑BeadBeater 96                        |
| Plate Sealer    | Thermal, compatible w/ 96‑well deep‑well plates     |
| Vacuum Dryer    | LabConco Centrivap with deep‑well rotor              |
| SBS GC Rack     | 96‑place, 9 mm spacing glass vials & caps           |

*Consumables:* 1.2 mL PP deep‑well 96 plates, adhesive heat seals, 5 mm stainless‑steel beads, C18 magnetic beads (50 mg/mL slurry), wide‑bore sterile tips (200 & 300 µL).

## 9 Reagents & Standards


| Reagent                        | Preparation / Concentration                                             | Storage         |
| -------------------------------- | ------------------------------------------------------------------------- | ----------------- |
| **Internal Standard (IS)**     | 10 mg/mL C19:0 FAME in heptane                                         | −20 °C       |
| **37‑FAME Mix**               | Supelco CRM47885, stock 10 mg/mL in chloroform                         | −20 °C       |
| **Calibration Working Levels** | 0.05, 0.1, 0.25, 0.5, 1.0, 2.0 mg/mL (serial dilution in heptane) | −20 °C       |
| 0.5 M KOH in methanol        | Dissolve 28 g KOH in 1 L methanol                                     | RT, desiccated |
| 14 % BF₃‑methanol           | Commercial, unopened ampoules                                           | 4 °C          |
| Heptane + 0.01 % BHT        | 0.1 g BHT / L heptane                                                 | RT              |
| Saturated NaCl                 | 360 g/L H₂O                                                           | RT              |
| Hexane:Isopropanol (3:2 v/v)  | Mix fresh daily                                                         | RT              |

## 10 Procedure

### 10.1 Sample Receipt & Login

1. Verify sample integrity, assign LIMS ID, and record weight.
2. Aliquot ≤ 2 g into a 2‑mL microtube if storage required (−20 °C max 7 days).

### 10.2 Homogenisation


| Matrix                               | Action                                                                                                                                             |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Eggs & other homogeneous liquids** | Vortex 30 s; no bead‑beating                                                                                                                     |
| **Solid/semi‑solid foods**          | Weigh 0.50 ± 0.01 g into deep‑well plate, add**2 × 5 mm beads** & **1 mL Hex:Iso (3:2)**; seal, bead‑beat 2 × 45 s with 30 s rest. |

### 10.3 Trans‑Esterification & Extraction (Assist Plus Script `FAME_STEP1`)


| Step | Reagent                                                                                          | Vol (µL) | Tool          | Deck Position |
| ------ | -------------------------------------------------------------------------------------------------- | ----------- | --------------- | --------------- |
| 1    | Internal Standard                                                                                | 40        | 50 µL tips  | R1            |
| 2    | 0.5 M KOH/MeOH                                                                                  | 200       | 300 µL tips | R2            |
| 3    | **Incubate** 60 °C, 1000 rpm, 20 min (HEATMAG)                                               | —        | —            | —            |
| 4    | 14 % BF₃/MeOH                                                                                  | 200       | 300 µL tips | R3            |
| 5    | **Incubate** 60 °C, 1000 rpm, 20 min                                                         | —        | —            | —            |
| 6    | Heptane                                                                                          | 400       | 300 µL tips | R4            |
| 7    | Saturated NaCl                                                                                  | 200       | 300 µL tips | R5            |
| 8    | Seal plate, shake 3 min, magnet engage 90 s; collect**300 µL** upper (organic) to new plate. |           |               |               |

### 10.4 SPE Cleanup (Script `FAME_SPE`)

1. Pre‑dispense **20 µL** C18 magnetic bead slurry into each well of SPE plate.
2. Transfer 300 µL extract, mix 30 s at 800 rpm; magnet engage 60 s.
3. Discard supernatant; wash beads with 100 µL heptane.
4. Elute FAME with **300 µL 5 % diethyl ether in heptane** into fresh deep‑well plate.

### 10.5 Dry & Reconstitute (Manual Transfer)

1. Unseal plate, place in Centrivap: 40 °C, 10 mbar, 15 min or to dryness.
2. Add **200 µL Heptane + BHT**; vortex or Assist Plus mix 5 × 50 µL cycles.
3. Reseal plate.

### 10.6 Final Transfer to GC Vials (Script `FAME_LOAD_GC`)

1. Orient plate **landscape**; set Voyager tip spacing **9 mm** (portrait).
2. Aspirate **50 µL** from each well row‑wise; dispense into matching position in SBS 96‑vial rack.
3. Cap vials immediately.

### 10.7 GC‑FID Analysis


| Parameter   | Setting                                                                              |
| ------------- | -------------------------------------------------------------------------------------- |
| Injection   | 1 µL, split 100 : 1, 250 °C                                                    |
| Carrier Gas | H₂, constant flow 1.0 mL min⁻¹                                                  |
| Oven        | 140 °C 5 min → 4 °C min⁻¹ → 240 °C 15 min                             |
| Detector    | FID 280 °C; H₂ 35 mL min⁻¹, Air 350 mL min⁻¹, Makeup N₂ 30 mL min⁻¹ |

### 10.8 Calibration & Quality Control

1. Inject calibration levels (low→high) **before** batch and **after** every 50 samples.
2. Inject **QC‑1** every 10 samples; acceptable if each target FA within ±10 % of certified.
3. Re‑inject solvent blank after each calibration.
4. Re‑calibrate if any IS‑normalised response drifts > 10 %.

### 10.9 Calculations

\[FA (mg g⁻¹) = (Aₓ / A_IS) × (C_IS / m_sample) × RRFₓ\]
Where *A* = peak area, *C_IS* = IS mass (mg), *m_sample* = sample mass (g), *RRF* = relative response factor from calibration curve.

## 11 Maintenance & Troubleshooting

- Column bake‑out 260 °C 30 min daily.
- Replace septa & liner every 150 injections.
- Verify hydrogen leak‑free daily.

## 12 Records

- Raw chromatograms, results table, QA/QC charts retained in LIMS for 5 years.

## 13 Revision History


| Rev | Date         | Author | Changes         |
| ----- | -------------- | -------- | ----------------- |
| 0   | 2025‑08‑05 | BM     | Initial release |
