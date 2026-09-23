# Awesome-AI-Watermark-Detection

# Top AI Watermark Detection Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on AI-Generated Content Detection, Invisible Watermarks, C2PA / Content Credentials Verification, Deepfake & Synthetic Media Provenance*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Watermark Detection** and related provenance verification. These tools help determine whether images, video, audio, or text were generated or edited by AI—via invisible watermarks (e.g. SynthID), signed C2PA / Content Credentials manifests, metadata analysis, and forensic classifiers.

**Examples** include Truepic, Reality Defender, Sensity AI, Optic, GetReal Security, Attestiv, C2PA Verify / Content Credentials tools, Hive AI, Adobe Content Credentials Verify, and DeepMedia (the category leaders and adjacent platforms).

**Open-source emphasis**: The open ecosystem is strong around **C2PA** (Content Authenticity Initiative SDKs and `c2patool`), offline watermark/metadata detectors (**AICheck**, **AI Watermark Detector**), research deepfake classifiers, and local-first verification apps. Commercial platforms still lead in multi-signal fusion, scale, and managed threat intelligence. This section lists every significant relevant project found.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Truepic](https://www.truepic.com/)**  
  Content authenticity and verification platform using cryptographic provenance and related signals to establish trust in photos and media.

- **[Reality Defender](https://www.realitydefender.com/)**  
  Multi-modal deepfake and AI-generated content detection platform for images, video, audio, and text used by enterprises and platforms.

- **[Sensity AI](https://sensity.ai/)**  
  Visual threat intelligence and synthetic media detection focused on deepfakes, face manipulation, and AI-generated imagery at scale.

- **[Optic, GetReal Security, Attestiv, DeepMedia](https://www.getrealsecurity.com/)**  
  Platforms and tools for detecting synthetic media, verifying authenticity, and supporting investigations into manipulated or AI-generated content.

- **[Hive AI](https://thehive.ai/)**  
  AI moderation and detection suite including capabilities for identifying AI-generated or manipulated visual content.

- **[Adobe Content Credentials / C2PA Verify](https://contentauthenticity.org/)**  
  Industry Content Credentials (C2PA) verification experiences and tools that surface signed provenance manifests when present in media.

- **[Other commercial AI detection & provenance platforms](https://www.realitydefender.com/)**  
  Additional solutions combining watermark detection, forensic analysis, and authenticity scoring for media platforms and enterprises.

## Open-Source GitHub Projects

- **[Content Authenticity Initiative / contentauth (C2PA)](https://github.com/contentauth)**  
  Official open-source C2PA stack: `c2patool` (CLI), `c2pa-rs` (Rust SDK), JavaScript/Swift/Android bindings, and related libraries for reading, validating, and writing Content Credentials manifests.

- **[AICheck](https://github.com/MatrixA/aicheck)**  
  Offline CLI that detects AI-generated images, video, and audio by analyzing metadata and invisible watermarks—no API keys or network required; supports many formats and generators.

- **[AI Watermark Detector](https://github.com/cpeoples/ai-watermark-detector)**  
  Research-oriented Rust CLI for detecting known text watermark schemes (SynthID-style, KGW/green-list, Gumbel, Unigram, SWEET, etc.) and verifying C2PA provenance on images, video, audio, and PDFs.

- **[Local-first C2PA / Watermark inspector](https://github.com/kylosarc/watermark)**  
  Browser-based, local-first app for inspecting C2PA credentials and media provenance without uploading assets—validates signatures and displays manifest lineage.

- **[Open AI image detectors (research)](https://github.com/lynote-ai/ai-image-detector)**  
  Open-source CLI/API/UI and benchmarks for probabilistic AI-generated image detection (e.g. UniversalFakeDetect / CLIP-based approaches).

- **[Deepfake detection research code](https://github.com/search?q=deepfake+detection+OR+synthetic+image+detection)**  
  Academic and community models (CLIP-based, frequency-domain, etc.) for classifying real vs. AI-generated or manipulated media.

- **[SynthID text & related open watermarking](https://github.com/search?q=SynthID+OR+text+watermarking+open+source)**  
  Open implementations and research code around text watermarking schemes that detectors can check for (Google has open-sourced aspects of SynthID text watermarking).

- **[C2PA web & client SDKs](https://github.com/contentauth/c2pa-js)**  
  JavaScript and other language bindings for embedding C2PA verification directly into applications and local tools.

### Additional Strong Open-Source Options

- **C2PA core**: `c2patool` + contentauth SDKs as the standard way to read and validate Content Credentials.
- **Offline multi-signal CLIs**: AICheck and AI Watermark Detector for metadata, watermarks, and C2PA in one place.
- **Local-first UIs**: Browser apps that never upload media.
- **Research classifiers**: Open deepfake / synthetic-image models for probabilistic detection when watermarks or manifests are absent.
- **Composable stacks**: C2PA verification + open classifier + metadata inspection for defense-in-depth.
- Full commercial platforms still lead in continuous model updates, multi-modal fusion, and enterprise workflows.

**Frameworks for building custom systems**:  
The strongest open foundations are the **Content Authenticity Initiative (C2PA) SDKs and c2patool**, plus offline detectors like **AICheck** and **AI Watermark Detector**.  
Research classifiers fill gaps when provenance signals are missing.  
Commercial platforms (Reality Defender, Sensity, Truepic, Hive, Adobe Content Credentials experiences, etc.) combine multiple signals, scale, and managed updates.  
Many teams use open C2PA tools for cryptographic provenance checks and open or research detectors for residual risk, while relying on commercial services for high-volume or high-stakes moderation. Fully open stacks work well for privacy-sensitive or air-gapped verification.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- AI watermark and synthetic-media detection is probabilistic. Absence of a watermark or C2PA manifest does **not** prove content is human-made; presence of a valid manifest proves provenance claims were signed, not that every claim is true. Detectors can produce false positives and false negatives, especially after re-encoding, screenshots, or adversarial edits.
- Open-source tools offer transparency and local operation but may lag commercial systems in coverage of the latest generators. Use multiple signals and human review for high-stakes decisions (journalism, legal, platform enforcement).

---

**Made for journalists, trust & safety teams, researchers, and developers building media authenticity workflows.**  
Let's expand open, verifiable tools for content provenance while recognizing the multi-signal depth and operational scale that leading commercial AI watermark and deepfake detection platforms deliver.
