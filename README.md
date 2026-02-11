# Vietnamese District Management System (vdmansys)

> Project repository for the **C&MA Vietnamese District** — tracking the initiative to give every local church a sustainable church management system and provide the District with accurate, consistent reporting.

---

## Overview

This repository contains the **project documentation, planning artifacts, integration specifications, and governance materials** for the District & Church Management System initiative.

The initiative uses a **phased hybrid approach**:

| Phase | Scope | Status |
|---|---|---|
| **1-A** | Institutionalize ChMeetings as District operational backbone and system of record | Piloting (2023–2025) |
| **1-B** | Improve ChMeetings sustainability — data standards, normalization, sample church config | In progress |
| **2-A** | Evaluate ChurchCM as local church front-end with ChMeetings integration (pilot) | Pending DEXCOM approval (Mar 1, 2026) |
| **2-B** | District-wide ChurchCM adoption decision | Pending (Oct 1, 2026) |

---

## The Two Systems

### ChMeetings — District System of Record
- [chmeetings.com](https://chmeetings.com)
- Cloud-based SaaS; the District operates a **Diocese-model tenant**
- Used for: centralized annual reporting, official pastor/worker/church lists, multi-church events (VAY Sports Fest, camp, conference)
- Pilot instances: [vay.chmeetings.com](https://vay.chmeetings.com), [rpc.chmeetings.com](https://rpc.chmeetings.com)

### ChurchCM — Local Church Front End *(under evaluation)*
- [churchcm.com](https://churchcm.com) — developed by Simon (Chi) Liêu
- Lightweight, self-hosted, per-church deployment
- Key features: member/family management, groups/ministries, courses/classes, kids check-in, prayer requests, role-based access
- Integration: secure API-key-based sync to District's ChMeetings (annual report submission)
- **Note:** Provenance pending verification — likely a derivative of the open-source [ChurchCRM](https://github.com/ChurchCRM/CRM) (MIT license); attribution requirements must be confirmed before District endorsement

### C&MA CMS — National Compliance System
- Remains the required compliance system for the national denomination
- Goal: align District-critical identifiers and naming conventions between C&MA CMS and ChMeetings

---

## Governance

| Role | Person |
|---|---|
| Project Sponsor | Pastor Trường Xuân Hồ |
| Product Owner | Pastor Bumble Hồ |
| Lead Developer | Mr. Simon (Chi) Liêu |
| Technical Reviewer | Mr. Thanh Dang, Ph.D. (Meta systems architect) |
| Data Steward | Pastor Peter Đoàn |
| District Operations | Cô Trang |
| Pilot Church — ChurchCM | Jacksonville, FL (Pastor Phát Mạnh Lê) |
| Pilot Church — ChMeetings Diocese | Midway, FL (Pastor Peter Đoàn) |

---

## Timeline

| Milestone | Target |
|---|---|
| DEXCOM approval — Phase 1-A & 1-B | Feb 11, 2026 |
| DEXCOM approval — Phase 2-A pilot | Mar 1, 2026 |
| Pilot release | Apr 1, 2026 |
| Additional pilots | May 2026 |
| First official release | Aug 2026 |
| First District Annual Report (ChMeetings Diocese) | 2027 |
| DEXCOM decision — Phase 2-B | Oct 1, 2026 |
| District rollout | Nov 2026 – Mar 2027 |
| All churches operational with ChurchCM integration | Dec 31, 2027 |
| First District Annual Report with ChurchCM integration | 2028 |

---

## Budget

- **Year 1:** $2,000 (core infrastructure and tools)
- **Year 2+:** $1,000/year
- **Future (if Phase 2-B approved):** ~$15–$30/month/church for hosting/support

---

## Repository Structure

```
vdmansys/
├── context/                  # Background research and reference documents
│   ├── project-charter-v1.1.md      # Project charter (latest version)
│   ├── ChurchCM_com-Review.docx/.pdf # Detailed review of ChurchCM by Pastor Bumble Hồ
│   ├── ChurchCM_com-Review.pdf
│   ├── Gmail-VD-Starting-Ideas-2026-02-06.pdf  # Initial email thread
│   └── VN-District-Management-System-Charter.pdf # Earlier charter draft
├── .gitignore
└── README.md
```

> Future folders will include: `specs/` (integration API specs), `data-standards/` (naming conventions, minimum data elements), `pilots/` (pilot church runbooks).

---

## Related Repositories

| Repo | Description |
|---|---|
| [i12know/vaysf](https://github.com/i12know/vaysf) | ChMeetings ↔ WordPress integration for VAY Sports Fest (Python) |
| [ChurchCRM/CRM](https://github.com/ChurchCRM/CRM) | Upstream open-source ChMS (MIT license) — likely basis for ChurchCM |

---

## Key Risks

| Risk | Mitigation |
|---|---|
| Adoption | Start with pilots; provide templates and training |
| Data quality | Standardize minimum data elements and practices |
| ChurchCM provenance | Verify licensing/attribution before District endorsement of Phase 2-B |
| Technical | Modular design, open standards, API-gated integrations |
| Sustainability | GitHub repo, clear ownership, continuity documentation |

---

*District leadership retains strategic control and oversight. DEXCOM approval required at each phase gate.*
