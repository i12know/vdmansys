# District & Church Management System Initiative - Executive Summary (v1.1)

## Purpose

To provide churches within the District with a sustainable church management solution that improves local ministry operations while enabling accurate, consistent District-level reporting.

## Problem Statement

-   The District needs reliable data for annual reporting, planning, and oversight. Local churches don't report well because they don't track the data needed for "form-filling" with year-round operational discipline, using a system for its data (membership list and status, spiritual milestones, church attendance, group rosters, giving categories, etc.)

-   Churches vary widely in size and technical capacity. Most don't use a Church Management System (ChMS).

-   Those who use a ChMS, use a variety of products (Planning Center, Breeze, Tithe.ly, ChurchTrac, Servant Keeper, etc.) with no District support.

-   A full-featured, multi-tenant system (e.g., ChMeetings Diocese version) can be too complex for many small churches, leading to uneven adoption.

-   C&MA CMS remains the required compliance system; our goal is to align District-critical identifiers and naming conventions between CMS and ChMeetings.


## Proposed Solution (Phased Approach)

Use a phased approach at the District level and for the local churches.

### 1-A. Institutionalize ChMeetings for District Operational Backbone and System of Record

-   Centralized Annual District reports from the churches (piloted for 2024 already)
-   Official list of Pastors and workers in the Vietnamese District (piloted in 2023)
-   Official list of official churches and organizations in the District (needed in 2025)
-   Collection of other participants in the District at multi-church events such as VAY Sports Fest, camp, conference, etc. (operational in 2025)
-   Support the autonomy of any District local church's operation on the platform (RP is operational in 2024)

### 1-B. Improving ChMeetings for Sustainability

-   Review and define the District's reporting template (minimum data elements and practices)
-   Time-boxed Data Normalization Sprint for District-critical records (pastors / workers / delegates + official church names across C&MA and District systems)
-   Standardize key data elements and conventions (people names, titles, roles)
-   Provide a "Sample Church" configuration as a proof-of-concept and training environment
-   Pilot with other willing churches in the District (Midway, Jacksonville)
-   Organize a stakeholder community to charter the long-term District data governance

### 2-A. Local Church Front End Integration Evaluation - (for local churches using ChurchCM)

-   ChurchCM is proposed as an open-source, lightweight system developed by Simon Lieu (pending verification of repository access, licensing/provenance, and documentation).
-   Any church could download, install, and deploy it for their church by themselves, or through Simon Lieu's support.
-   ChurchCM focused on day-to-day ministry needs (Membership & guest tracking, Ministry groups, classes, events, Kids check-in, etc.)
-   The data in the system can be submitted as the required Annual Report to the District's ChMeetings using a Secure API-key-based sync. Only required metrics are shared.
-   Pilot with Jacksonville church.

### 2-B. Local Church Front End Adoption for ChurchCM

-   Once the open-sourced ChurchCM codebase is properly tested, it could be adopted widely for its:
    -   Lower adoption barrier for small churches
    -   Hides complexity while preserving capability
    -   Supports long-term scalability and governance
    -   Reduces technical and organizational risk, avoids vendor lock-in

-   DEXCOM will need to evaluate and approve:
    -   Will it endorse the adoption of ChurchCM?
    -   Will it subsidize the hosting of each local church running ChurchCM? (~$15–$30/month/church)
    -   What is the operating model for ChurchCM beyond having access to an open-sourced system that works well with the District data intake?


## Governance & Ownership

-   **Project Sponsor:** Pastor Trường Xuân Hồ
-   **Product Owner:** Pastor Bumble Hồ
-   **Lead Developer:** Mr. Simon (Chi) Liêu
-   **Technical Reviewer:** Mr. Thanh Dang, Ph.D. (attended GLA, currently a Meta system architect)
-   **Data Steward:** Pastor Peter Đoàn — works on District data standards and naming conventions
-   **District User:** Cô Trang — works on office operations
-   **Pilot Church for ChurchCM:** Jacksonville, FL (Pastor Phát Mạnh Lê)
-   **Pilot Church for ChMeetings Diocese tenant:** Midway, FL (Pastor Peter Doan)

District leadership retains strategic control and oversight.


## Timeline (High-Level)

| Milestone | Target Date |
|---|---|
| DEXCOM approval for Phase 1-A & 1-B | Feb 11, 2026 |
| DEXCOM approval for Phase 2-A integration pilot | Mar 1, 2026 |
| Pilot release | Apr 1, 2026 |
| Additional pilots | May 2026 |
| First official release | Aug 2026 |
| First District Annual Report (ChMeetings Diocese churches) | 2027 |
| DEXCOM decision for Phase 2-B | Oct 1, 2026 |
| District rollout | Nov 2026 – Mar 2027 |
| All churches operational with ChurchCM Integration | Dec 31, 2027 |
| First District Annual Report with ChurchCM Integration | 2028 |


## Budget (Initial Estimate)

-   $2,000 (first year) for core infrastructure and tools
-   $1,000/year starting second year
-   Future: optional per-church hosting/support model (~$15–$30/month/church, if adopted)


## Risks & Mitigation

| Risk | Mitigation |
|---|---|
| Adoption risk | Start with pilots and lead by example (District churches); provide templates and training support |
| Data quality risk | Standardize minimum data elements and practices |
| Technical risk | Use modular design and open standards; keep integrations central and adoptions gated with DEXCOM approval. API keys required for integrations |
| Sustainability risk | Clear ownership, documentation, and continuity plan for any custom components using GitHub open source repository |


## Decision Requested from DEXCOM

1.  Confirm governance roles.
2.  Approve **Phase 1 (A & B):** ChMeetings as the District operational backbone, data-elements standardization, and authorize pilot deployment (Diocese model).
3.  Approve initial budget envelope (including training/pilot support, and data cleanup support if prioritized).
4.  Authorize **Phase 2-A** evaluation of an optional local front-end integration (e.g., ChurchCM) and pilot, with the future decision of Phase 2-B on the horizon.
