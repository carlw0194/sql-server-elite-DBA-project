# SQL Server Elite DBA Project

## GitHub Folder Structure
sql-server-elite-dba/                     ← root repo (keep name short & searchable)
│
├── .github/                              ← GitHub plumbing (actions & templates)
│   ├── workflows/
│   │   └── ci.yml                        ← lints PowerShell, T-SQL, Markdown
│   └── ISSUE_TEMPLATE.md                 ← drives structured issue capture
│
├── README.md                             ← elevator pitch, setup, badges 🌟
├── CONTRIBUTING.md                       ← PR etiquette, code-style rules
├── LICENSE                               ← MIT (or your choice)
│
├── docs/                                 ← *markdown source of the “course book”*
│   ├── 00-ProjectCharter.md              ← goals, scope, success criteria ℹ️
│   ├── Phase01-CoreFoundations/
│   │   ├── Scenario01-HealthCheck.md
│   │   ├── Scenario02-Automation.md
│   │   └── …
│   ├── Phase02-PerfTuning/
│   ├── Phase03-HA-DR/
│   ├── Phase04-Security/
│   ├── Phase05-CloudHybrid/
│   └── Phase06-Leadership/
│
├── src/                                  ← **source code** (version-controlled)
│   ├── PowerShell/
│   │   └── dbHealthChecks/               ← PSModule manifest + functions
│   ├── TSQL/
│   │   ├── Maintenance/                  ← Ola jobs, index scripts
│   │   ├── Performance/                  ← Query Store views, wait-stat sproc
│   │   └── Security/                     ← RBAC, auditing, DDL triggers
│   └── CSharp/                           ← CLR helpers, if any
│
├── baselines/                            ← raw perf/data captures (CSV, JSON)
│   ├── 2025-07-11/                       ← “Day-0” benchmark of lab
│   └── template/                         ← README on how to add new baseline
│
├── datasets/                             ← sample DB backups & synthetic data
│   ├── AdventureWorks2022/
│   ├── WideWorldImporters/
│   └── TPCH-HammerDB/
│
├── media/                                ← screenshots, short Loom/OBS clips
│   ├── images/
│   └── videos/
│
├── notebooks/                            ← Azure Data Studio or Jupyter *.ipynb
│   └── perf-analysis.ipynb
│
├── deployments/                          ← **Infrastructure-as-Code**
│   ├── terraform/                        ← Azure VM + MI
│   ├── arm/                              ← ARM/Bicep examples
│   └── docker-compose/                   ← local multi-node AG lab
│
├── tests/                                ← automated validation
│   ├── tSQLt/                            ← unit tests for sprocs
│   └── Pester/                           ← PowerShell module tests
│
└── capstone/                             ← final project assets
    ├── architecture-diagrams/
    ├── exec-summary.pdf                  ← C-level deliverable
    └── demo-scripts/
