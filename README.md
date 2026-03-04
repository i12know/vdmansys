# Vietnamese District Management System (vdmansys)

> A **C&MA Vietnamese District** office initiative to build a reliable data repository and reporting foundation using ChMeetings — starting with the pastors' directory and the online annual report.

---

## Current Status

**Scope narrowed per Executive Sponsor direction (Feb 10, 2026).**

This is currently a **District office initiative**, not a church-wide rollout. The focus is on two immediate deliverables in ChMeetings, with a single church pilot running in parallel.

---

## Immediate Priorities

### 1. Pastors' Directory & Profiles
- Establish the official list of pastors and workers in the Vietnamese District
- Standardize names, titles, roles, and contact information in ChMeetings
- Groundwork initiated by Pastor Peter Đoàn in October 2025; directory framework shared Feb 2026

### 2. Online Annual Report
- Enable churches to submit their annual report through ChMeetings
- Define minimum required data elements and reporting template
- Replace or supplement the current form-filling process with year-round data discipline

---

## ChMeetings — The Platform

- [chmeetings.com](https://chmeetings.com) — cloud-based SaaS church management platform
- The District operates its own **Diocese-model tenant**
- Already in use: [vay.chmeetings.com](https://vay.chmeetings.com) (VAY Sports Fest), [rpc.chmeetings.com](https://rpc.chmeetings.com) (RP Church)
- C&MA national CMS remains the required compliance system; goal is to align naming conventions between the two

---

## Jacksonville Pilot

Chi Liêu is working directly with MS Phát Mạnh Lê (Jacksonville, FL) to pilot ChMeetings adoption at the local church level. Learnings from this experiment will inform any future broader adoption strategy for the District.

> A concrete implementation timeline from Chi is a pending action item.

---

## Governance

| Role | Person |
|---|---|
| Executive Sponsor | Pastor Trường Xuân Hồ |
| Product Owner | Pastor Bumble Hồ |
| Data Steward & Timeline Owner | Pastor Peter Đoàn |
| Implementation Lead | Mr. Simon (Chi) Liêu |
| Technical Reviewer | Mr. Thanh Dang, Ph.D. (Meta systems architect) |
| District Operations | Cô Trang |
| Pilot Church | Jacksonville, FL — MS Phát Mạnh Lê |

---

## Open Action Items

| Owner | Action Item |
|---|---|
| Pastor Peter Đoàn | Provide a realistic timeline for directory and annual reporting delivery — by end of Feb 2026 |
| Chi Liêu | After working with MS Phát, share assessment of a reasonable ChMeetings implementation timeline for Jacksonville |

---

## What's On Hold

The following were proposed in the v1.1 Project Charter but are **not in scope at this time**:

- ChurchCM local church front-end evaluation (Phase 2-A)
- District-wide ChurchCM adoption (Phase 2-B)
- DEXCOM formal approval process (removed from Feb 11 agenda)
- Budget approval
- Integration API specifications

These will be revisited once the District office foundation is in place and the Jacksonville pilot produces learnings.

---

## Data Sources & Golden Master

The goal is to reconcile data from three independent sources into a **golden master directory** of licensed workers in the Vietnamese District.

| Source | Folder | What it contains | PII level |
|---|---|---|---|
| **C&MA Denomination CMS** | `CMA-CMS-data-dump/` | Official church list (110 churches) and licensed individuals (257 workers) — codes, names, status, years of service | Low (names only in xlsx) |
| **VD Conference Registration** | `VD-Conf-Registration-data-dump/` | HD50 conference registrants & spouses (450 rows), Pastor Directory 2025 MASTER (6 sheets — workers, secretaries, Si Bo, Qua Phu, Thong Cong) with titles, roles, addresses, phone, email | **High** |
| **ChMeetings Export** | `ChMeetings-data-dump/` | People export from the District ChMeetings tenant (256 rows, 50 fields) — names, contact info, church, roles, notes | **High** |

> **Note:** Only the CMA CMS xlsx is committed to GitHub. The VD Conference Registration and ChMeetings folders are excluded via `.gitignore` because they contain full PII (addresses, phone numbers, emails). CMS screenshots (`.png`) are also excluded.

---

## Repository Structure

```
vdmansys/
├── context/                            # Background research and reference documents
│   ├── CMA-CMS-data-dump/            # C&MA Denomination CMS data (Feb 2026)
│   │   ├── *.png (local only — contains PII, not committed)
│   │   └── CMS VN District Churches 2026 0218.xlsx
│   ├── VD-Conf-Registration-data-dump/  # (local only — high PII, not committed)
│   │   ├── MSTDCTV and spouses - HD50.xlsx
│   │   └── Pastor Directory 2025 MASTER.xlsx
│   ├── ChMeetings-data-dump/          # (local only — high PII, not committed)
│   │   └── People 03-04-2026.xlsx
│   ├── project-charter-v1.1.md        # Original charter (pre-descope)
│   ├── project-charter-v1.2.md        # Current charter (descoped per Feb 10 direction)
│   ├── VN-District-Management-System-Charter-(1_2).docx
│   ├── Gmail-VD-Starting-Ideas-2026-02-06.pdf
│   └── VN-District-Management-System-Charter.pdf
├── .gitignore
└── README.md
```

---

## Related Repositories

| Repo | Description |
|---|---|
| [i12know/vaysf](https://github.com/i12know/vaysf) | ChMeetings ↔ WordPress integration for VAY Sports Fest |

---

*This repository serves as the working record for the District office team. Updates will be made as action items are completed and scope evolves.*
