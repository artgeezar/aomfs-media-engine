# 📡 AOMFS Media Engine

[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Domain Validation](https://img.shields.io/badge/verification-DNS%20MX%20%2B%20HTTP%20200-green.svg)](https://github.com/artgeezar/aomfs-media-engine)

A sovereign broadcast syndication and media automation engine engineered for independent record labels and artist campaigns. Features automated DNS MX routing verification, language-aware cultural localization, pre-flight HTTP verification, and lossless broadcast media muxing.

Engineered by **Art Jay Guizar** (President & Founder, AOMFS Records LLC).

---

## ⚡ Overview

Independent labels face high friction in press and radio syndication: high email bounce rates, format mismatches (pitching radio stations webzine reviews), and language/cultural blunders (pitching Brazil in Spanish or defaulting to generic PR spin).

The **AOMFS Media Engine** automates the entire verification and outreach lifecycle:
1. **Network Validation**: Verifies destination MX records via DNS and checks recipient domains for live HTTP 200 responses before any dispatch.
2. **Cultural Toast Localization**: Automatically identifies territory and enforces native drinking toasts:
   * Brazil / Portugal: `SAÚDE!`
   * LATAM / Spain: `¡SALUD!`
   * Japan: `KANPAI!`
   * Germany / Austria: `PROST!`
   * Global English: `CHEERS!`
3. **Format Alignment**: Reconciles target media types (College Radio / Terrestrial / Webzine / Podcast) to prevent sending station IDs to webzines or review requests to radio music directors.
4. **AV Muxing Suite**: Losslessly injects 24-bit 48kHz WAV master audio into 4K/ProRes video containers using Apple AVFoundation.

---

## 🚀 Key Modules

* `engine.py`: Core CLI orchestrator for contact auditing and verification.
* `dns_guard.py`: Asynchronous DNS MX validator and disposable email detector.
* `av_muxer.py`: Native AVFoundation audio-video alignment tool.

---

## 💻 CLI Usage

### Audit & Verify Contact Queue
```bash
python engine.py --input contacts.csv --verify-dns --verify-http --output verified_queue.csv
```

### Localize Dispatch Copy
```bash
python engine.py --contact "ed@rockfreaks.net" --country "Denmark" --medium "webzine" --generate-card
```

---

## 🛡️ License

MIT License. Designed and maintained by Art Jay Guizar (AOMFS Records).
