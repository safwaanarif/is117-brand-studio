# Career & Portfolio Research: Systems Administration & NOC Operations

- **Project:** IS117 Portfolio Research
- **Tracks Compared:** Linux Systems Administration vs. Network Operations Center (NOC) Technician
- **Desk-Review Date:** November 11, 2026 (Updated November 15, 2026 per peer review)
- **Status:** Complete — Public documentation baseline for portfolio planning.

## Employer Observations & Source Traceability

| Role & Employer                                            | Source & Verification Date                                                                                                               | Location & Availability                 | Deadline Wording            | Observed Core Responsibilities                                                                                   | Key Technical Requirements                                                    |
| :--------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------- | :-------------------------- | :--------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| **Graduate / Junior Cloud & Systems Engineer** (Canonical) | [Canonical Job Board — Cloud & Systems](https://canonical.com/careers/all) _(Verified Nov 11, 2026; individual req IDs rotate on board)_ | Remote / Hybrid (US East)               | Not stated (Rolling review) | Server provisioning, incident triage, system log analysis, shell maintenance scripting, VM/container operations. | Ubuntu/Debian environment, Bash scripting, systemd, Git version control.      |
| **NOC Technician I** (SHI International)                   | [SHI Job Search — NOC Technician](https://www.shi.com/careers/search) _(Verified Nov 11, 2026; internal portal link)_                    | Somerset, NJ (On-site / Shift rotation) | Not stated (Open posting)   | Continuous network monitoring, outage logging, alert escalation, ticket tracking, ICMP/SNMP ping checks.         | TCP/IP fundamentals, OSI model, basic network troubleshooting, SLA adherence. |

## Direction Comparison (SysAdmin vs. NOC Operations)

| Dimension           | Direction A: Junior Linux Systems Administrator (Selected Primary Track)                         | Direction B: NOC Technician I (Adjacent Operational Track)                                  |
| :------------------ | :----------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------ |
| **Core Focus**      | Server configuration, shell automation, service management, and system reliability.              | Real-time network/server alarm monitoring, Layer 2/3 triage, and ticket escalation.         |
| **Strength / Fit**  | Directly aligns with terminal workflows, Bash scripting, and Ubuntu server administration labs.  | Strong entry point for incident documentation, SLA response, and network diagnostics.       |
| **Trade-off / Gap** | Requires demonstrable scripting and infrastructure-as-code artifacts rather than just lab notes. | Shift-based on-site schedules and reliance on proprietary enterprise monitoring dashboards. |

## Research Findings to Portfolio Decisions & Checks

1. **Scripted Repetition for Systems Roles (Canonical Finding):**  
   _Finding:_ The Canonical engineering description emphasizes shell maintenance scripting and automated server provisioning.  
   _Decision:_ Build a dedicated "Terminal & Scripting" showcase featuring tested Bash utility scripts with clear exit codes and argument handling.  
   _Check:_ Run each script locally in Ubuntu Linux with both valid and invalid inputs, verifying clean `0` / non-zero exit statuses and readable `README` usage examples.

2. **Structured Incident Triage for NOC Roles (SHI Finding):**  
   _Finding:_ The SHI NOC Technician I description centers on monitoring alerts, logging outages, and escalating Layer 2/3 issues rather than writing automation scripts.  
   _Decision:_ Include a documented incident response runbook demonstrating simulated network outage triage, ICMP/SNMP checks, and escalation criteria.  
   _Check:_ Have a peer inspect the runbook markdown to verify that root-cause steps, diagnostic commands, and escalation triggers are clear without requiring live enterprise tools.

3. **Explicit Availability & Deadline Tracking:**  
   _Finding:_ Both postings omit hard cutoff dates and specify distinct work modes (Remote vs. On-site Somerset, NJ).  
   _Decision:_ Standardize all portfolio career cards to record exact availability/location and verbatim deadline wording (`Not stated`).  
   _Check:_ Cross-check table columns against the saved desk-review notes before publishing updates.

## Verification Checklist

- [x] Employer descriptions verified from original job boards with date, location/availability, and deadline wording recorded (#8, #9).
- [x] Findings separated accurately between SysAdmin scripting and NOC monitoring/escalation (#10).
- [x] Two career directions compared and concrete verification checks attached to each portfolio decision (#11).
- [x] Private personal reflections and eligibility circumstances kept strictly in Canvas.
