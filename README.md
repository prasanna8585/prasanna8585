# Hi there, I'm Prasanna Dabi 👋 


### 🛡️ Cybersecurity Practitioner | Cloud Security Architect
Specializing in cloud infrastructure hardening and advanced threat detection.

---

### 🏆 Featured Security Discovery: CVE-2026-25212
* **Project:** Percona Monitoring and Management (PMM)
* **Vulnerability:** Authenticated Remote Code Execution (RCE) - CVSS 9.9
* **Official Advisory:** [GHSA-hm6f-x2ww-p497](https://github.com/advisories/GHSA-hm6f-x2ww-p497)
* **Impact:** Identified a critical flaw allowing full host compromise via reverse shell.

### 🏆 Featured Security Discovery: CVE-2026-12681
* **Project:** Google go-attestation Library
* **Vulnerability:** Improper Input Validation / TPM Hash Injection - CVSS 8.9
* **Official Advisory:** [GHSA-9r4w-jg96-92mv](https://github.com/google/go-attestation/security/advisories/GHSA-9r4w-jg96-92mv)
* **Impact:** Discovered a critical logic flaw in `parseEfiSignatureList()` where a crafted TPM event log can inject arbitrary SHA256 hashes into a verifier's trusted database, causing a compromised boot state to be falsely accepted.

### 🚀 Notable Security Discovery: xpub Change-Index Amplification
* **Project:** Trezor Blockbook Service
* **Vulnerability:** Unauthenticated Resource Exhaustion (DoS)
* **Official Advisory:** [Trezor Security Advisory](https://trezor.io/vulnerability/unauthenticated-remote-do-s-via-xpub-change-index-amplification)
* **Impact:** Identified an amplification flaw where uncapped change indexes in xpub descriptors forced excessive database lookups and address derivations, filling a global in-memory cache and forcing a complete Out-of-Memory (OOM) server crash.

### 🚀 Notable Security Discovery: Unauthenticated Remote Memory Exhaustion
* **Project:** Trezor Blockbook Service
* **Vulnerability:** Denial of Service (DoS) via Unbounded Timestamp Array
* **Official Advisory:** [Trezor Security Portal](https://trezor.io/vulnerability/unauthenticated-remote-do-s-via-xpub-change-index-amplification)
* **Impact:** Found a flaw in the historical price API allowing unauthenticated remote attackers to pass massive, unbounded timestamp arrays to trigger rapid server memory exhaustion.

### 🚀 Notable Security Discovery: eBPF DDoS Mitigation Logic Failure
* **Project:** PowerDNS dnsdist
* **Vulnerability:** Logic Flaw / Denial of Service (DoS) Mitigation Bypass
* **Official Advisory:** [Pull Request #17287](https://github.com/PowerDNS/pdns/pull/17287)
* **Impact:** Discovered a critical logic error in `bpf-filter.cc` where range-based subnet evaluation queries incorrectly triggered a runtime error, completely breaking active eBPF-based blocking mechanisms and leaving the DNS infrastructure exposed during traffic spikes.

### 🚀 Notable Security Discovery: REST API Permission Boundary Bypass
* **Project:** PowerDNS dnsdist
* **Vulnerability:** Authorization Bypass / Improper Access Control
* **Official Advisory:** [Pull Request #17291](https://github.com/PowerDNS/pdns/pull/17291)
* **Impact:** Identified a security boundary issue where restricted "Read-Only" API tokens could bypass endpoint separation rules to execute unintended state-changing memory actions (such as purging the global packet cache and exploiting CORS misconfigurations), breaking the isolation between read and write access keys.

---

### 🛠️ Technical Stack
<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white" />
</p>

---

### 📫 Let's Connect
* **LinkedIn:** [Prasanna Dabi](https://www.linkedin.com/in/prasanna-dabi-27b6a513a/)

---
*"Securing the cloud, one exploit at a time."*

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=prasanna8585&label=Profile%20views&color=0e75b6&style=flat" alt="prasanna8585" />
</p>


![Bug Bounty Terminal Dashboard](assets/bug-bounty-terminal.svg?v=1)

![Bug Bounty Target Radar](assets/bug-bounty-radar.svg?v=1)
<!--
**prasanna8585/prasanna8585** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
