# Censys Exposed Services — Security Report

**Type:** Passive OSINT / Attack Surface Management (ASM)  
**Tool Used:** [Censys Internet Intelligence Platform](https://search.censys.io)  
**Date:** April 11, 2026  
**Analyst:** Obaidur Rahman

---

## Overview

This report identifies three exposed services discovered via passive reconnaissance using Censys. No active exploitation or login attempts were made. All findings are based solely on publicly available information returned by the Censys scanner.

---

## Findings Summary

| # | Service | Port | Severity | CVSS v3.1 Score |
|---|---------|------|----------|-----------------|
| 01 | Exposed FTP (Pure-FTPd) | 21/TCP | HIGH | 8.2 |
| 02 | Exposed MySQL (MariaDB 10.6.24) | 3306/TCP | CRITICAL | 9.8 |
| 03 | Exposed cPanel Login Page | 2083/TCP | CRITICAL | 10.0 |

---

## Key Techniques

- **Censys Queries:** `services.port`, `services.service_name` filters for FTP, MySQL, and cPanel
- **Passive Analysis:** Manual inspection only — no exploitation, no login attempts
- **CVSS v3.1 Scoring:** Each finding scored using the standard Attack Vector / Complexity / Impact model

---

## Tools & Methodology

| Tool | Purpose |
|------|---------|
| Censys (search.censys.io) | Internet-wide scan data — open ports and services |
| CVSS v3.1 Calculator | Severity scoring of findings |

---

## Disclaimer

This research was conducted purely for educational purposes. All targets were discovered passively through Censys public data. No systems were accessed, no credentials were tested, and no harm was caused to any network or system.

---

## Files

- `Report.pdf` — Full security report with finding details and remediation steps
