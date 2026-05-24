# 🔍 Advanced Digital Forensics & Incident Response (DFIR) Lab Architecture

A comprehensive, enterprise-grade digital forensics investigation and incident response track completed over 6 intensive weeks (Weeks 7–12 of the Cyberster engineering program). This repository documents hands-on case setups, forensic artifact parsing, and multi-source evidence correlation to reconstruct complex user and attacker timelines.

---

## 💻 Forensic Lab Environment & Tooling Matrix
* **Forensic Frameworks & Suites:** Autopsy Forensic Browser, Volatility 3 Core Engine
* **Artifact Parsing Toolkits:** Registry Explorer, LECmd (LNK Parser), PECmd (Prefetch Parser)
* **Investigative Environments:** Windows Triage Hosts, Isolated Evidence Mount Points
* **Core Artifact Targets:** Windows Registry Hives (`SYSTEM`, `SOFTWARE`, `SAM`, `NTUSER.DAT`), NTFS File System Structures, Outlook PST Stores, Raw RAM Memory Dumps

---

## 📅 Chronological Forensic & Artifact Breakdowns

### 📦 Week 7: Forensic Disk Imaging & NTFS Core Elements
* **Bit-Stream Integrity:** Mastered raw forensic disk imaging workflows, establishing strict chain-of-custody protocols through MD5/SHA256 hash verification checks.
* **File System Dissection:** Conducted structural analysis of Windows NTFS volumes, mapping hidden data vectors by extracting the **MFT (Master File Table)** and hunting for data streams within **ADS (Alternate Data Streams)**.
* **Deleted Object Recovery:** Reconstructed damaged structural pointers to successfully carve out and recover deleted system file signatures.

### 💻 Week 8: Windows Core Triage & Event Log Correlations
* **Authentication Auditing:** Dissected Windows Event Logs to isolate user privilege usage patterns, distinguishing standard access actions from anomalous authentication vectors.
* **Execution Timelines:** Leveraged **Prefetch file structures** to track historical application launch events, mapping precise machine uptime calendars.
* **Hidden Artifact Recovery:** Extracted and parsed binary system caches including Thumbcache databases, browser storage nodes, and Recycle Bin metadata to establish user presence.

### 🌐 Week 9: Browser Forensics & LNK File Footprints
* **User Behavior Reconstruction:** Extracted SQLite backend databases across active browser application profiles to inventory search histories, explicit download paths, cookies, and rogue extensions.
* **Interaction Footprints:** Analyzed system **LNK shortcuts** to map the exact execution timelines of external system utilities and user file-open frequencies.
* **Timestamp Normalization:** Correlated time configurations across disparate log architectures into a unified operational timeline.

### 🗄️ Week 10: Enterprise Registry Forensics & Case Architecture
* **Case Deployment Setup:** Configured end-to-end case workflows within **Autopsy** to systematically process raw target volumes.
* **Hive Dissection:** Parsed structural Windows registry hives (`SYSTEM`, `SOFTWARE`, `SAM`, `NTUSER.DAT`) using **Registry Explorer** to uncover system telemetry.
* **Perimeter Audit Clues:** Documented historical USB storage device connection states, drive letter mapping records, MRU (Most Recently Used) tracking maps, and user shell folders.

### 📧 Week 11: Email Forensics & Corporate Data Exfiltration Audits
* **PST Data Parsing:** Investigated an insider corporate data leak scenario by conducting structured data extractions over Microsoft Outlook **PST data stores**.
* **Header Architecture Forensic Analysis:** Parsed raw email header metadata arrays to evaluate source network paths, relay routing architectures, and mail exchange signatures.
* **Cross-Artifact Triage Validation:** Combined email traffic indicators with **LNK** and **Prefetch tracking data** (`LECmd` & `PECmd`) to validate malicious data movement footprints.

### 🧠 Week 12: Memory (RAM) Forensics & Integrated Case Closing
* **Volatile Data Ingestion:** Executed deep memory space investigations using the **Volatility 3** framework over raw system RAM dumps.
* **Process Vector Auditing:** Traced operational process hierarchy trees, hidden DLL injections, and raw command-line argument hooks to isolate active threat actions.
* **Unified DFIR Reporting:** Integrated multi-source threat indicators across memory dumps, network streams, and disk artifacts into a comprehensive Forensic Incident Report.

---

## 🛠️ Complete Technical Skill Set Verified
* **Digital Forensics (DFIR):** Windows Registry Triage, Volatile Memory Investigation, Artifact Timeline Normalization, Email Header Forensics
* **Framework Compliance:** NIST SP 800-61 Incident Handling Guidelines, ISO/IEC 27037 Evidence Handling Baselines
* **Investigation Standards:** Chain of Custody Maintenance, Hash Integrity Verification, Multi-Source Event Correlation
