lab-qms/
├─ 00_README.md              ← high-level repo map + how to contribute
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
├─ 04_WORK_INSTRUCTIONS/     ← step-by-step screenshots, pipette settings, etc.
│   ├─ WI-GC-01_Inlet-Liner-Change.md
│   └─ WI-LC-01_Source-Cleaning.md
├─ 05_FORMS_TEMPLATES/
│   ├─ F-01_Sample-Chain-of-Custody.xlsx
│   ├─ F-02_Calibration-Curve-Template.xlsx
│   └─ F-03_Internal-Audit-Checklist.docx
├─ 06_RECORDS/               ← **immutable**—only JSON/CSV pushed by automation
│   ├─ 2025/
│   │   ├─ FA/
│   │   │   ├─ 2025-08-05_sample123_FA.json
│   │   │   └─ ...
│   │   └─ PEST/
│   │       ├─ 2025-08-05_sample123_PST.json
│   │       └─ ...
│   └─ index.sqlite          ← optional DB that your Python scripts update
├─ 07_VALIDATION/
│   ├─ VAL-M-FA-001_Validation-Report.pdf
│   └─ VAL-M-PST-001_Validation-Report.pdf
├─ 08_RISK_OPP/
│   └─ RO-001_Risk-Register.xlsx
├─ 09_CHANGE_CONTROL/
│   └─ CC-2025-01_GC-Column-Change.md
├─ scripts/                  ← Python utilities
│   ├─ ingest_record.py
│   └─ regenerate_index.py
└─ .github/
    ├─ workflows/
    │   └─ qms-lint.yml      ← CI checks: filename schema, JSON schema
    └─ ISSUE_TEMPLATE/       ← “Document Change Request”, etc.
