# ANZEN
Real-time Android phishing defense platform featuring URL interception, entropy-based threat detection, homograph analysis, and on-device security intelligence.

<div align="center">

<img src="screenshot/logo.jpeg" width="120">

# Anzen

### Enterprise-Grade Phishing Defense & Intent Firewall for Android

![Kotlin](https://img.shields.io/badge/Kotlin-1.9+-7F52FF)
![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-UI-blue)
![License](https://img.shields.io/badge/License-MIT-orange)

*Zero-knowledge. Real-time. Fully on-device.*

Anzen is a real-time security engine for Android that intercepts zero-day phishing links, calculates domain entropy, strips invisible trackers, and blocks malicious sites in milliseconds — all running 100% locally on your device.

</div>

---

## Screenshots

| Real-Time Dashboard | Deep Scanner | Threat Interception |
|---------------------|-------------|---------------------|
| ![](screenshot/dashboard.jpg) | ![](screenshot/deep%20scanner.jpg) | ![](screenshot/threat.jpg) |

---

## Why Anzen?

Traditional mobile antiviruses rely on slow cloud blacklists that routinely miss newly generated zero-day phishing links.

Attackers actively bypass them using Domain Generation Algorithms (DGA) and Homograph attacks—techniques that are invisible to signature-based scanners.

Anzen takes a different approach by analyzing the mathematical characteristics of a URL before it opens. Threat detection occurs locally on the device, eliminating cloud dependency and reducing response time.

---

## Core Features

| Feature | Description |
|----------|------------|
| 🌐 Omnipresent Interception | Scans links across SMS, WhatsApp, Telegram, and Android browsers before launch |
| 🔢 Mathematical Heuristics | Shannon Entropy & Homograph Detection |
| 🧹 Privacy Purge | Removes trackers such as `utm_source` and `fbclid` |
| 🔒 Zero-Knowledge Architecture | 100% local processing with no browsing history collection |
| 📊 Dynamic Telemetry UI | Real-time risk dashboard and threat visibility |

---

## The Heuristics Engine

```text
URL Intercepted
      │
      ▼
Stage 1: Extraction & Sanitization
      │
      ▼
Stage 2: Punycode / Homograph Analysis
      │
      ▼
Stage 3: Shannon Entropy Calculation
      │
      ▼
Stage 4: Deep Spoofing & Tunnel Detection
```

### Stage 1 — Extraction & Sanitization

- Deep extraction of URLs from text
- URL normalization and cleaning
- Removal of obfuscation techniques

### Stage 2 — Punycode & Homograph Analysis

- Detects Unicode spoofing attacks
- Converts internationalized domains for inspection
- Identifies lookalike brand domains

### Stage 3 — Entropy Analysis

- Calculates Shannon Entropy
- Detects algorithmically generated domains
- Flags suspicious randomness patterns

### Stage 4 — Spoofing & Tunnel Detection

- Detects phishing kits
- Identifies brand impersonation attempts
- Flags suspicious tunnel services and redirect chains

---

## Tech Stack

| Layer | Technology |
|---------|------------|
| Language | Kotlin 1.9+ |
| UI | Jetpack Compose |
| Architecture | MVVM + Clean Architecture |
| Dependency Injection | Dagger-Hilt |
| Async | Kotlin Coroutines & Flow |
| Local Storage | Room (SQLite) |

---

## Security & Privacy

- 100% on-device threat analysis
- No cloud dependency
- No browsing history collection
- No keystroke logging
- Privacy-first architecture
- Minimal accessibility event usage

---

## Installation

### Option A — Direct APK

1. Download the latest APK from Releases
2. Allow installation from unknown sources
3. Install Anzen
4. Complete the onboarding process

### Option B — Build From Source

#### Requirements

- Android Studio Iguana or newer
- Min SDK: API 26
- Target SDK: API 34

```bash
git clone https://github.com/fahim-stepsup/ANZEN.git
```

---

## Future Roadmap

- Machine Learning–based phishing classification
- Threat intelligence integration
- Browser extension support
- Enhanced telemetry dashboard
- Community threat feeds

---

## License

Distributed under the MIT License.

See the LICENSE file for details.

---

## Author

**Fahim Akthar**

Security Coordinator & Incident Coordinator @ Zoho

Top Internal Bug Hunter 2025

Cybersecurity Researcher | Penetration Tester | Android Security Enthusiast
