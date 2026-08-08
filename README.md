# Hi there, I'm Prasanna Dabi 👋 


### 🛡️ Cybersecurity Practitioner | Cloud Security Architect
Specializing in cloud infrastructure hardening and advanced threat detection.

---

### 🏆 Featured Security Discovery: CVE-2026-46602
* **Project:** Go Core Image Packages (`golang.org/x/image/tiff`)
* **Vulnerability:** Unbounded Memory Allocation / Resource Exhaustion - CVSS 7.5
* **Official Advisory:** [GO-2026-5062](https://pkg.go.dev/vuln/GO-2026-5062) | [GHSA-pwfv-328h-75x9](https://github.com/advisories/GHSA-pwfv-328h-75x9)
* **Impact:** Identified a resource validation flaw where processing maliciously crafted tiled TIFF images forces immediate Out of Memory (OOM) errors and Denial of Service (DoS).

### 🏆 Featured Security Discovery: CVE-2026-12681
* **Project:** Google go-attestation Library
* **Vulnerability:** Improper Input Validation / TPM Hash Injection - CVSS 8.9
* **Official Advisory:** [GHSA-9r4w-jg96-92mv](https://github.com/google/go-attestation/security/advisories/GHSA-9r4w-jg96-92mv)
* **Impact:** Discovered a critical logic flaw in `parseEfiSignatureList()` where a crafted TPM event log can inject arbitrary SHA256 hashes into a verifier's trusted database, causing a compromised boot state to be falsely accepted.

### 🏆 Featured Security Discovery: CVE-2026-25212
* **Project:** Percona Monitoring and Management (PMM)
* **Vulnerability:** Authenticated Remote Code Execution (RCE) - CVSS 9.9
* **Official Advisory:** [GHSA-hm6f-x2ww-p497](https://github.com/advisories/GHSA-hm6f-x2ww-p497)
* **Impact:** Identified a critical flaw allowing full host compromise via reverse shell.

### 🏆 Featured Security Discovery: GHSA-3238-pp48-6m3j
* **Project:** Google Project Oak
* **Vulnerability:** Trusted Execution Environment (TEE) Attestation Bypass
* **Official Advisory:** [GHSA-3238-pp48-6m3j](https://github.com/project-oak/oak/security/advisories/GHSA-3238-pp48-6m3j)
* **Impact:** Discovered a critical validation flaw enabling a complete bypass of enclave security measurements, allowing untrusted hosts to spoof remote attestation states.

### 🏆 Featured Security Discovery: GHSA-gqvg-gmmx-x4hm
* **Project:** MLflow (`mlflow/mlflow`)
* **Vulnerability:** Path Traversal / Arbitrary File Read
* **Official Advisory:** [GHSA-gqvg-gmmx-x4hm](https://github.com/mlflow/mlflow/security/advisories/GHSA-gqvg-gmmx-x4hm)
* **Impact:** Discovered a path traversal flaw in MLflow artifact retrieval endpoints. An attacker could manipulate URI path parameters to bypass directory containment and read arbitrary files directly from the underlying server filesystem.

### 🏆 Featured Security Discovery: GHSA-pj9q-pv45-xq8g
* **Project:** Google Project Oak (`project-oak/oak`)
* **Vulnerability:** Stage0 Firmware Integer Overflow / Memory Corruption
* **Official Advisory:** [GHSA-pj9q-pv45-xq8g](https://github.com/project-oak/oak/security/advisories/GHSA-pj9q-pv45-xq8g)
* **Impact:** Discovered an integer overflow in the `setup_high_allocator` function within the stage0 bootloader firmware. An untrusted host or hypervisor could supply a maliciously crafted E820 memory map entry to trigger silent memory aliasing during heap initialization, leading to enclave memory corruption.

### 🚀 Notable Security Discovery: TensorFlow Lite Buffer Bounds Check Arithmetic Overflow
* **Project:** TensorFlow (`tensorflow/tensorflow`)
* **Vulnerability:** Arithmetic Overflow / Out-of-Bounds Memory Access
* **Official Advisory:** [Pull Request #123910](https://github.com/tensorflow/tensorflow/pull/123910)
* **Impact:** Discovered an arithmetic overflow vulnerability in TFLite buffer bounds checking logic during model deserialization (`tflite::Verify`). Processing malformed FlatBuffer models allowed boundary validation checks to be bypassed, leading to out-of-bounds memory access, heap corruption, or runtime crashes.

### 🚀 Notable Security Discovery: Google ADK JS Zip-Slip Blacklist Bypass
* **Project:** Google ADK JS (`google/adk-js`)
* **Vulnerability:** Path Traversal / Zip-Slip Blacklist Bypass
* **Official Advisory:** [Pull Request #621](https://github.com/google/adk-js/pull/621)
* **Impact:** Discovered a Zip-Slip bypass vulnerability in archive extraction routines where blacklist-based path validation was insufficient. An attacker supplying a maliciously structured archive could bypass path checks to write or overwrite arbitrary files outside the target extraction directory on the underlying host filesystem.

### 🚀 Notable Security Discovery: Go SSH Channel Stall Denial of Service
* **Project:** Go Extended Cryptography Library (`golang/go` / `x/crypto`)
* **Vulnerability:** Unhandled Protocol State Transition / Denial of Service
* **Official Advisory:** [Issue #80333](https://github.com/golang/go/issues/80333)
* **Impact:** Discovered a channel stall vulnerability in the `x/crypto/ssh` package where unhandled protocol state transitions caused concurrent SSH channel handlers to deadlock or hang indefinitely. An unauthenticated or authenticated client could exploit this to exhaust server connections and trigger a Denial of Service (DoS).

### 🚀 Notable Security Discovery: XNNPACK Space-to-Depth Integer Overflow
* **Project:** Google XNNPACK (`google/XNNPACK`)
* **Vulnerability:** Integer Overflow / Heap-based Buffer Overflow
* **Official Advisory:** [Pull Request #10907](https://github.com/google/XNNPACK/pull/10907)
* **Impact:** Discovered an integer overflow vulnerability during output buffer calculation in the space-to-depth operator. Supplying oversized or maliciously structured tensor dimensions through public API calls could bypass buffer bounds checks, leading to heap memory corruption or runtime crashes.

### 🚀 Notable Security Discovery: Google ADK JS Unsafe A2A Metadata Control Flow Redirection
* **Project:** Google ADK JS (`google/adk-js`)
* **Vulnerability:** Agent-to-Agent (A2A) Metadata Injection / Control Flow Hijacking
* **Official Advisory:** [Pull Request #596](https://github.com/google/adk-js/pull/596)
* **Impact:** Discovered a security flaw in Agent-to-Agent (A2A) communications where untrusted peer-supplied `transferToAgent` metadata was processed without sanitization. A malicious remote agent could manipulate execution metadata to force unauthorized agent redirection and hijack local control flow.

### 🚀 Notable Security Discovery: OpenXLA / TensorFlow Shape Proto Integer Overflow
* **Project:** OpenXLA & TensorFlow (`openxla/xla` / `tensorflow/tensorflow`)
* **Vulnerability:** Integer Overflow / Out-of-Bounds Memory Access
* **Official Advisory:** [OpenXLA PR #46403](https://github.com/openxla/xla/pull/46403) | [OpenXLA PR #46495](https://github.com/openxla/xla/pull/46495) | [TensorFlow PR #124350](https://github.com/tensorflow/tensorflow/pull/124350)
* **Impact:** Discovered an integer overflow vulnerability in `Shape::FromProto` shape deserialization logic. Processing malformed proto definitions with oversized array bounds could bypass shape validation, leading to out-of-bounds memory access, heap corruption, or runtime crashes across OpenXLA and TensorFlow graph compilers.

### 🚀 Notable Security Discovery: XNNPACK Batch Matrix Multiply Integer Overflow
* **Project:** Google XNNPACK (`google/XNNPACK`)
* **Vulnerability:** Integer Overflow / Heap-based Buffer Overflow
* **Official Advisory:** [Pull Request #10842](https://github.com/google/XNNPACK/pull/10842)
* **Impact:** Discovered an integer overflow vulnerability in the batch matrix multiplication operator when calculating packed weights allocation size. An attacker supplying oversized, caller-controlled tensor dimensions through public API calls could trigger heap memory corruption or runtime crashes.

### 🚀 Notable Security Discovery: OpenXLA Buffer Allocation Boundary Validation Flaw
* **Project:** OpenXLA Compiler (`openxla/xla`)
* **Vulnerability:** Out-of-Bounds Memory Access / Improper Input Validation
* **Official Advisory:** [Pull Request #46105](https://github.com/openxla/xla/pull/46105)
* **Impact:** Discovered a validation vulnerability in `BufferAssignment::FromProto` where assigned buffer allocation offsets and sizes were deserialized without verifying boundary limits. Loading malformed or untrusted HLO proto definitions allowed unvalidated offsets to trigger out-of-bounds memory access, heap corruption, or unexpected compiler crashes.

### 🚀 Notable Security Discovery: XNNPACK Deconvolution Kernel Calculation Memory Corruption
* **Project:** Google XNNPACK (`google/XNNPACK`)
* **Vulnerability:** Integer Overflow / Heap-based Buffer Overflow
* **Official Advisory:** [Pull Request #10834](https://github.com/google/XNNPACK/pull/10834)
* **Impact:** Identified an integer overflow flaw during kernel-size dimension calculations in the deconvolution operator. Processing maliciously crafted layer parameters bypassed spatial memory bounds, leading to heap buffer overflows and unexpected memory corruption.

### 🚀 Notable Security Discovery: Go SSH Private Key Parameter Validation Bypass
* **Project:** Go Extended Cryptography Library (`golang/go` / `x/crypto`)
* **Vulnerability:** Cryptographic Parameter Validation Bypass / Improper Input Validation
* **Official Advisory:** [Issue #80418](https://github.com/golang/go/issues/80418)
* **Impact:** Discovered a vulnerability in the `ssh.ParseDSAPrivateKey()` function where ASN.1 DER-encoded DSA private keys are processed without verifying the mathematical validity of their core cryptographic parameters (p, q, and g). An application parsing a maliciously structured or malformed private key could be forced into intense CPU exhaustion (Denial of Service), trigger runtime panics, or experience unpredictable cryptographic failures during signature and verification operations.

### 🚀 Notable Security Discovery: Go SSH Client Terminal Escape Sequence Injection
* **Project:** Go Extended Cryptography Library (`golang/go` / `x/crypto`)
* **Vulnerability:** Improper Input Sanitization / ANSI Escape Sequence Injection
* **Official Advisory:** [Issue #80302](https://github.com/golang/go/issues/80302)
* **Impact:** Discovered a vulnerability in the `ssh.BannerDisplayStderr()` helper function where pre-authentication SSH banners were streamed directly to `os.Stderr` without data sanitization. A malicious or compromised server could inject arbitrary ANSI escape codes to execute terminal spoofing, manipulate clipboards, or potentially exploit underlying terminal emulator vulnerabilities on the client side.

### 🚀 Notable Security Discovery: gVisor Mount Isolation Bypass
* **Project:** Google gVisor Container Sandbox (`google/gvisor`)
* **Vulnerability:** Mount Namespace Security / Container Isolation Bypass
* **Official Advisory:** [Issue #13481](https://github.com/google/gvisor/issues/13481) | [Pull Request #13482](https://github.com/google/gvisor/pull/13482)
* **Impact:** Discovered a sandbox isolation flaw where `open_tree(OPEN_TREE_CLONE)` incorrectly succeeded on `MNT_DETACH` unmounted paths (which strictly returns `EINVAL` on native Linux). This allowed a user with container root privileges to clone and re-attach an intentionally isolated filesystem via `move_mount(2)`, completely breaking container containment boundaries.

### 🚀 Notable Security Discovery: xpub Change-Index Amplification
* **Project:** Trezor Blockbook Service
* **Vulnerability:** Unauthenticated Resource Exhaustion (DoS)
* **Official Advisory:** [Trezor Security](https://trezor.io/vulnerability/unauthenticated-remote-do-s-via-xpub-change-index-amplification)
* **Impact:** Identified an amplification flaw where uncapped change indexes in xpub descriptors forced excessive database lookups and address derivations, filling a global in-memory cache and forcing a complete Out-of-Memory (OOM) server crash.

### 🚀 Notable Security Discovery: Unauthenticated Remote Memory Exhaustion
* **Project:** Trezor Blockbook Service
* **Vulnerability:** Denial of Service (DoS) via Unbounded Timestamp Array
* **Official Advisory:** [Trezor Security](https://trezor.io/vulnerability/unauthenticated-remote-do-s-via-xpub-change-index-amplification)
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
## 🛠️ Active SecOps Monitoring

![Bug Bounty Terminal Dashboard](assets/bug-bounty-terminal.svg?v=1)

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

![Bug Bounty Target Radar](https://raw.githubusercontent.com/prasanna8585/prasanna8585/master/assets/bug-bounty-radar.svg)
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
