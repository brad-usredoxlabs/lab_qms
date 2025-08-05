lab-qms/
├─ 00_README.md
├─ 01_QUALITY_MANUAL/
│   ├─ QM-000_Master-Quality-Manual.md
│   └─ QM-001_Record-Control.md
├─ 02_PROCEDURES/
│   ├─ PR-LAB-001_Document-Control.md
│   ├─ PR-LAB-002_Internal-Audit.md
│   ├─ PR-CHEM-101_Sample-Login.md
│   ├─ PR-CHEM-102_Calibration-GC-FID.md
│   └─ PR-CHEM-103_Calibration-LC-MSMS.md
├─ 03_METHODS/
│   ├─ M-FA-001_FAME-GC-FID.md
│   └─ M-PST-001_Multi-Residue-Pesticides-LC-MSMS.md
├─ 04_WORK_INSTRUCTIONS/
│   ├─ WI-GC-01_Inlet-Liner-Change.md
│   └─ WI-LC-01_Source-Cleaning.md
├─ 05_FORMS_TEMPLATES/
│   ├─ F-01_Sample-Chain-of-Custody.xlsx
│   ├─ F-02_Calibration-Curve-Template.xlsx
│   └─ F-03_Internal-Audit-Checklist.docx
├─ 06_RECORDS/                       ← **immutable** lab data (JSON/CSV)
│   ├─ 2025/
│   │   ├─ FA/   2025-08-05_sample123_FA.json
│   │   └─ PEST/ 2025-08-05_sample123_PST.json
│   └─ index.sqlite
├─ 07_VALIDATION/
│   ├─ VAL-M-FA-001_Validation-Report.pdf
│   └─ VAL-M-PST-001_Validation-Report.pdf
├─ 08_RISK_OPP/                      ← risk & opportunity register
│   └─ RO-001_Risk-Register.xlsx
├─ 09_CHANGE_CONTROL/
│   └─ CC-2025-01_GC-Column-Change.md
├─ 10_EQUIPMENT/                     ← **new**
│   ├─ EQ-LCMS-001_QExactive/
│   │   ├─ 10_PO_Invoice.pdf
│   │   ├─ 20_Tech-Spec.pdf
│   │   ├─ 30_IQ-OQ-PQ_Report.pdf
│   │   ├─ 40_Calibration-Certs/
│   │   └─ 50_Maintenance-Log.csv
│   └─ EQ-GC-001_Agilent-6890/
│       └─ (same sub-structure)
├─ 11_TRAINING_COMPETENCE/           ← staff CVs, training plans & records
│   ├─ TR-Matrix.xlsx
│   └─ TR-EMP045_Smith_Jane.csv
├─ 12_SUPPLIERS/                     ← approved-supplier list & evaluations
│   └─ SUP-List_2025.xlsx
├─ 13_PROFICIENCY_TESTING/           ← PT/ILC enrolment & results
│   └─ PT-2025-FA-UK_NML_Round1.pdf
├─ 14_NONCONFORM_CORRECTIVE/
│   ├─ NC-2025-03_BatchFailure.md
│   └─ CA-2025-03_RootCauseAnalysis.xlsx
├─ 15_MANAGEMENT_REVIEW/
│   └─ MR-2025_Q3_Minutes.pdf
├─ 90_SAFETY/                        ← (optional) SDS, chemical inventory
│   └─ SDS_Isooctane.pdf
├─ scripts/
│   ├─ ingest_record.py
│   └─ regenerate_index.py
└─ .github/
    ├─ workflows/qms-lint.yml
    └─ ISSUE_TEMPLATE/Document_Change_Request.md
