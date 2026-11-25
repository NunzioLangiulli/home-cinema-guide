# Bibliography

Every source used in this guide, ordered by type, each with a short **assessment**. No source is taken at face value, whether it is a standard, a manufacturer, a magazine or a video. Accessed November 2026.

## How sources are assessed

Each assessment answers five questions:

1. **Type**: primary (standard, official document, original measurement) or secondary (report, summary, explainer)?
2. **Independence**: does the author have an interest in the conclusion (selling a product, a trademark, a lawsuit, a sponsor)?
3. **Method**: is it measured, documented and reproducible, or an impression or claim?
4. **Date and scope**: is it current, and does it apply to consumer TVs, or to studios, one brand, one country?
5. **What we checked**: did we read the full text, only a summary, or only a page's metadata?

Where a source made a claim we found wrong or simplified, the correction is in the wiki page linked in the *Used in* column, with the reliability labels explained in the [README](../README.md#how-to-read-the-reliability-labels).

---

## 1. Standards and normative documents

| Source | Used in | Assessment |
|---|---|---|
| [ITU-R BT.709](https://www.itu.int/rec/R-REC-BT.709) | [03](../wiki/03-color.md) | Primary and authoritative for HDTV primaries and D65. Defines the *camera* curve, not the display curve, which is a common source of confusion (including in V3). |
| [ITU-R BT.1886](https://www.itu.int/rec/R-REC-BT.1886) (2011) | [03](../wiki/03-color.md), [settings](../settings/settings-explained.md#gamma) | Primary. The reference display EOTF for studio production. It assumes a dark grading environment; it says nothing about bright living rooms. |
| [ITU-R BT.2020](https://www.itu.int/rec/R-REC-BT.2020) | [03](../wiki/03-color.md) | Primary. A container gamut; no consumer display covers it fully, and most content is mastered inside P3. |
| [ITU-R BT.2100](https://www.itu.int/rec/R-REC-BT.2100) | [04](../wiki/04-hdr.md) | Primary for PQ and HLG. Production standard; consumer tone mapping is outside its scope. |
| [ITU-R BT.2035](https://www.itu.int/rec/R-REC-BT.2035) (2013) | [03](../wiki/03-color.md) | Primary, read in full. Room 10 lux; background D65 at ≈10 % ±2 % of reference white (this confirms the bias-light figure); reference white 100 cd/m², black <0.01 cd/m²; BT.1886 gamma; 1080p viewing angle 31° (3.2 × screen height); no added ringing/sharpening or motion artefacts. Studio scope: it says consumer displays should not be used for professional evaluation. |
| [SMPTE ST 2080-3](https://pub.smpte.org/doc/st2080-3/) (2017) | [03](../wiki/03-color.md) | Primary, but we only verified title, scope and date; the "10 % bias light" figure often attributed to such standards remains ❓. |
| SMPTE ST 2084 | [04](../wiki/04-hdr.md) | Primary for PQ; paywalled. We rely on its reproduction in BT.2100. |
| [CIE D65](https://en.wikipedia.org/wiki/CIE_Standard_Illuminant_D65) | [03](../wiki/03-color.md) | Linked via Wikipedia (secondary). Fine for the definition; the CIE publication is the primary source. |
| [HDMI.org — Quick Media Switching](https://hdmi.org/spec2sub/quickmediaswitching) | [settings](../settings/settings-explained.md#match-frame-rate-and-dynamic-range) | Primary (HDMI licensing body): QMS uses VRR to change frame rate without a blackout. Marketing-level detail; real-world support varies by device. |
| [ITU-R BT.2408](https://www.itu.int/dms_pub/itu-r/opb/rep/R-REP-BT.2408-9-2026-TOC-HTM-E.htm) (report, current edition 2026) | [04](../wiki/04-hdr.md) | Primary operational guidance for HDR production: reference/graphics white at 203 cd/m². We read the table and contents only. |
| ITU-R BS.775 | [06](../wiki/06-audio.md) | Primary for multichannel speaker angles. Cited from established knowledge; not re-read for this draft. |

## 2. Industry bodies and manufacturers

Primary for *what they say about themselves*, but never independent: each has a product, trademark or business model at stake.

| Source | Used in | Assessment |
|---|---|---|
| [UHD Alliance — Ambient Light Compensation for Filmmaker Mode (Oct 2025, PDF)](https://alliance.experienceuhd.com/wp-content/uploads/2025/10/UHDA-White-Paper-on-Ambient-Light-Compensation-for-Filmmaker-Mode-v4-clean.pdf) | [03](../wiki/03-color.md#why-filmmaker-mode-looks-dark), [settings](../settings/settings-explained.md#energy-saving-and-light-sensor) | Read in full. Technically specific (algorithm, exponent table) and candid about Filmmaker Mode's main weakness. Limits: the UHDA promotes its own trademark; the colorist test and the 31-person demo are described without sample sizes, statistics or blind conditions; accuracy depends on each TV's light sensor, which the paper leaves to manufacturers. |
| [Netflix — Dolby Vision HDR Mastering Guidelines](https://partnerhelp.netflixstudios.com/hc/en-us/articles/360000599948-Dolby-Vision-HDR-Mastering-Guidelines) | [03](../wiki/03-color.md) | Primary for Netflix's delivery workflow. Applies to Netflix productions only. |
| [Dolby Atmos Home Theater Installation Guidelines (Dec 2018, PDF)](https://displaydaily.com/wp-content/uploads/2014/10/dolby-atmos-home-theater-installation-guidelines.pdf) | [06](../wiki/06-audio.md) | Read in full. Ear-level speakers at ~1.2 m (BS.775-3); overhead speakers at 45° elevation (30–55°), 2–3× ear height; upfiring speakers need a flat reflective ceiling 2.3–4.3 m; levels 79–82 dB SPL(C) with −20 dBFS pink noise; bitstream output. Written by the format owner (claims about upfiring speakers being "preferable" are promotional). |
| [Dolby — speaker setup guides](https://www.dolby.com/about/support/guide/speaker-setup-guides/) | [06](../wiki/06-audio.md) | Practical and detailed. Dolby sells the format, so it does not discuss the limits of virtual or upfiring height. |
| [Samsung Ads — ACR Guide (PDF)](https://iabcanada.com/wp-content/uploads/2022/09/Samsung-Ads-ACR-Guide-CA.pdf) | [07](../wiki/07-privacy-acr.md) | A marketing document for advertisers (Canada, 2022). Strong evidence of what ACR captures ("glass level"), precisely because it was written to sell it; silent on privacy safeguards. |
| [Samsung — Smart Calibration](https://www.samsung.com/uk/support/apps-services/how-to-calibrate-your-tv-screen-with-smartthings/) | [08](../wiki/08-calibration.md) | Support page. Describes how the feature works; gives no accuracy data. |
| [Slidebean — TV Calibrator](https://slidebean.com/tv-calibrator) · [FAQ](https://slidebean.com/tv-calibrator-support) · [test patterns](https://slidebean.com/tv-calibrator#tvc-patterns) | [08](../wiki/08-calibration.md) | Developer's own description. Pattern playlists and HDR10+/Dolby Vision files checked 2026-11-25; the by-eye "Untangled" black-level and sharpness patterns appear only inside V7. Clear and honest about being an approximation. No published error measurements and no list of panel types used for the camera profiles yet; source code announced but not yet published (⏳). |
| [Kaleidescape — compare players](https://www.kaleidescape.com/compare/) | [01](../wiki/01-image-pipeline.md) | Vendor claims ("up to" bitrates); no independent measurements found. |
| [Roku — 2025 10-K (PDF)](https://image.roku.com/bWFya2V0aW5n/Roku-2025-Form10-K.pdf) | [07](../wiki/07-privacy-acr.md) | A legal filing, so reliable for segment figures. Interpretation (e.g. "hardware is a way to acquire accounts") is management's framing. |
| Texas AG releases: [Samsung](https://www.texasattorneygeneral.gov/news/releases/attorney-general-paxton-secures-major-agreement-samsung-ensure-texans-are-protected-smart-tvs), [LG](https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-major-agreement-lg-protect-texans-privacy-and-stop-data-being) | [07](../wiki/07-privacy-acr.md) | Primary for the fact and date of each settlement. Written by a party to the litigation, with political framing; we rely on them for facts, not characterizations. |

## 3. Research and independent measurements

| Source | Used in | Assessment |
|---|---|---|
| [RTINGS — How to calibrate your TV](https://www.rtings.com/tv/learn/how-to-calibrate-your-tv) and per-model settings pages | [settings](../settings/settings-explained.md#sharpness), [08](../wiki/08-calibration.md) | Independent lab with published methodology; the best practical reference for settings. Limits: one unit per model; some suggested neutral values are disputed by users; methodology changes between test-bench versions. |
| [RTINGS — Stutter vs Judder vs Micro-Judder](https://www.rtings.com/tv/learn/research/motion-cadence) | [02](../wiki/02-frame-rate-and-motion.md) | Clear and well-reasoned; the stutter/judder distinction is partly RTINGS's own terminology. |
| [RTINGS — size to distance](https://www.rtings.com/tv/reviews/by-size/size-to-distance-relationship) | [01](../wiki/01-image-pipeline.md#when-4k-is-actually-visible) | Based on visual-acuity models (about 1 arcminute); real visibility also depends on content, eyesight and contrast. |
| [UCL & UC Davis — Watching the Watchers (arXiv 2409.06203)](https://arxiv.org/html/2409.06203v1) | [07](../wiki/07-privacy-acr.md) | Measured, documented network traffic; the strongest independent evidence on ACR. Limits: preprint, two brands (Samsung, LG), 2024 firmware, UK and US settings. |
| [ProPublica — Vizio (2015)](https://www.propublica.org/article/own-a-vizio-smart-tv-its-watching-you) | [07](../wiki/07-privacy-acr.md) | High-quality investigative journalism; confirmed by the later FTC settlement. Dated: describes 2015 practices. |
| [Wang 2003 — Shazam (PDF)](https://www.ee.columbia.edu/~dpwe/papers/Wang03-shazam.pdf) | [07](../wiki/07-privacy-acr.md) | Peer-reviewed conference paper on audio fingerprinting; used only as an analogy for video ACR. |
| [Notebookcheck — TCL X11L](https://www.notebookcheck.net/TCL-X11L-SQD-peaks-at-almost-11-000-nits-surpassing-HDR10-standards.1296017.0.html) | [04](../wiki/04-hdr.md) | Reports a single reviewer's measurement (~10,900 nits); not reproduced elsewhere in our search. |
| [TechRadar — TCL at CES 2026](https://www.techradar.com/televisions/tcl-launches-next-gen-sqd-mini-led-tv-at-ces-the-best-tv-in-the-market-for-2026) | [04](../wiki/04-hdr.md) | Trade-show preview under manufacturer-controlled conditions; useful for specs, not for performance. |
| [in70mm.com — Oppenheimer](https://in70mm.com/presents/1970_imax/2023_oppenheimer/format/index.htm) | [01](../wiki/01-image-pipeline.md#imax-70-mm) | Enthusiast site, but it reproduces the official technical notes; reliable for format facts. |
| [8K Association — Oppenheimer scanned in 8K](https://8kassociation.com/oppenheimer-scanned-in-8k/) | [01](../wiki/01-image-pipeline.md#imax-70-mm) | Industry advocacy group for 8K; used only to corroborate the scan resolution. |
| [Emby — Dolby Vision profiles](https://emby.media/learn/articles/video/hdr/formats/dolby-vision/profiles-and-compatibility/Dolby-Vision-Profile-5.html) | [04](../wiki/04-hdr.md) | Media-server documentation; technically accurate but secondary. Which streaming service uses which profile is not confirmed by the services. |
| [MacRumors](https://www.macrumors.com/2021/05/18/apple-tv-color-balance-quality-colors-worse) / [Engadget](https://www.engadget.com/apple-tv-color-balance-calibration-tests-101007281.html) | [08](../wiki/08-calibration.md) | Reports of one professional calibrator's tests (2021); a small sample, but measured. |

## 4. Video explainers

Referred to in the wiki as **V1–V7**. These videos are the starting point of this guide: they explain complex topics clearly, show problems visually and give practical fixes, with interviews (Paul Carlin, finishing and color) and source lists in their descriptions. Typical limits: narrative framing ("the brilliant scam of…"), sponsored segments, deliberate simplification, and some technical slips. Each slip is corrected, with sources, in the linked wiki page; the most significant are listed below.

| Video | Used in | Assessment |
|---|---|---|
| **V1** — Slidebean, [*The Biggest Mistake in the History of Hollywood*](https://youtu.be/yN0H_WfWOp4) (2026-02-20, 30:19) | [01](../wiki/01-image-pipeline.md) | Excellent on the digital intermediate, upscaled "4K" and why bitrate matters. Corrected: banding blamed on gamut (it is bit depth and compression); P3 called a compression standard; IMAX 70 mm size and number of IMAX cinemas; "Nolan has no DI". |
| **V2** — Slidebean, [*yeah... no wonder movies look cheap on new TVs*](https://youtu.be/CFol4HFxVec) (2026-04-18, 36:16) | [02](../wiki/02-frame-rate-and-motion.md) | The clearest explanation of pulldown, interpolation and shutter angle in the series (manual captions). Corrected: VRR suggested as the fix for 24p (frame-rate matching is). |
| **V3** — Slidebean, [*The Brilliant Scam of "HDR"*](https://youtu.be/6hAVA6_Sczs) (2026-06-25, 32:28) | [03](../wiki/03-color.md), [04](../wiki/04-hdr.md) | Strong on relative vs absolute brightness and tone mapping, with a colorist's view. Corrected: gamma history (BT.709 vs BT.1886) and the "63/255" example; 0–255 vs 16–235; "400 nits for HDR"; Dolby Vision fallback; "fake HDR" criterion. |
| **V4** — Slidebean, [*The brilliant scam of cinematic "black bars"*](https://youtu.be/JYg0rBfAz6U) (2026-07-07, 39:04) | [05](../wiki/05-aspect-ratios.md) | Rich and largely accurate history of aspect ratios; percentages correct. Corrected: Univisium credited to Netflix (Storaro); "IMAX can't be edited digitally"; "widest format ever". |
| **V5** — Slidebean, [*yeah… this (hidden) chip pays for the whole TV*](https://youtu.be/t_GK06_3UY8) (2026-10-16, 24:26) | [07](../wiki/07-privacy-acr.md) | Well sourced (academic paper, filings, settlements) with its own network tests on Latin American TV models. Unverified: TCL case dismissal; margin estimates are the video's inference. |
| **V6** — Slidebean, [*The brilliant scam of "Dolby Atmos"*](https://youtu.be/SNwoI6531us) (2026-09-11, 38:26) | [06](../wiki/06-audio.md) | Clear on channels vs objects and matrix encoding; listening comparisons are sighted, not blind. Corrected: room EQ vs Atmos rendering; "1400 kbps for lossless"; dialogue problems blamed mainly on Atmos. |
| **V7** — Slidebean, [*This TV setting is ruining your movies*](https://youtu.be/Ki1QMLMkt0A) (2026-11-25, 34:04) | [03](../wiki/03-color.md), [08](../wiki/08-calibration.md), [settings](../settings/settings-explained.md) | The most practical video: why Filmmaker Mode looks dark, chromatic adaptation, an adjustment sequence, and a free phone-based calibration app. Nuanced: de-judder is interpolation; sharpening can't recover compressed detail; free calibration software exists; Filmmaker Mode's effect on local dimming varies by brand. |

Captions were automatic for six of the seven videos; misheard proper names were corrected (Janusz Kamiński, Robert Eggers, Xavier Dolan, Cinerama, telecine). Suggested viewing order for newcomers: V7 → V2 → V1 → V3 → V4 → V6 → V5.

## 5. Specialist press and general news

Secondary sources: useful for facts and context, but they usually report claims rather than measure them.

| Source | Used in | Assessment |
|---|---|---|
| [What Hi-Fi — Filmmaker Mode](https://www.whathifi.com/advice/what-is-filmmaker-mode-is-it-any-good-and-should-you-turn-it-on) · [Ultra HD Premium](https://www.whathifi.com/advice/ultra-hd-premium-what-are-specs-which-tvs-support-it) · [Netflix audio](https://www.whathifi.com/news/netflix-brings-high-quality-audio-to-51-and-atmos-content) | settings, [04](../wiki/04-hdr.md), [06](../wiki/06-audio.md) | Reputable specialist press relaying UHDA and Netflix specs. The Ultra HD Premium figures date from 2016 and we could not confirm a newer version. |
| [TechCrunch — Filmmaker Mode (2019)](https://techcrunch.com/2019/08/29/filmmaker-mode-will-automatically-turn-off-all-the-dumb-motion-smoothing-and-noise-reduction-on-new-tvs) · [Hollywood Reporter](https://www.hollywoodreporter.com/movies/movie-news/martin-scorsese-christopher-nolan-launching-filmmaker-mode-tv-setting-1234968/) | settings | Launch coverage based on UHDA announcements; good for history and the list of requirements. |
| [American Cinematographer — O Brother, Where Art Thou?](https://theasc.com/articles/o-brother-cinematography-deakins) | [01](../wiki/01-image-pipeline.md) | The ASC's own magazine: authoritative on production practice, close to its subjects. |
| [BGR — HDMI black level](https://bgr.com/2158216/what-hdmi-black-level-means-how-to-adjust-it-correctly/) · [Sound & Vision — LG settings](https://www.soundandvision.com/content/lg-oled65c8pua-oled-ultra-hdtv-review-settings) | settings | BGR is general tech press; Sound & Vision publishes measured reviews. Menu names refer to specific model years. |
| [TweakTown — Sony Bravia Core](https://www.tweaktown.com/news/77290/sony-bravia-core-movie-service-near-lossless-4k-blu-ray-streaming/index.html) | [01](../wiki/01-image-pipeline.md) | Relays Sony's launch claims (2020); no independent bitrate measurement. |
| [CNBC — Oppenheimer in 70mm IMAX](https://www.cnbc.com/2023/07/19/where-to-watch-oppenheimer-in-70mm-imax-.html) | [01](../wiki/01-image-pipeline.md) | General news, consistent with other reports (~30 cinemas). |
| [Fox Business — Fox to acquire Roku](https://foxbusiness.com/markets/fox-corporation-announces-22b-acquisition-roku-landmark-streaming-live-tv-deal) | [07](../wiki/07-privacy-acr.md) | ⚠️ Conflict of interest: owned by the acquirer. Used only for the deal's announced facts, which other outlets (AP, Bloomberg) also reported. |
| [Fox 7 Austin — LG settlement](https://www.fox7austin.com/news/lg-smart-tv-acr-data-collection-texas-settlement) | [07](../wiki/07-privacy-acr.md) | Local news relaying the AG's release. |
| [Malwarebytes — Samsung ACR](https://www.malwarebytes.com/blog/news/2026/03/samsung-tvs-stop-spying-on-viewers-in-texas-heres-how-to-disable-acr-anywhere) | [07](../wiki/07-privacy-acr.md), [names by brand](../settings/names-by-brand.md) | Security vendor blog; accurate summary and useful menu paths, with a privacy-advocacy angle. |
| [Decrypt — LG](https://decrypt.co/377637/lg-tv-might-be-listening-even-when-off) | [07](../wiki/07-privacy-acr.md) | Crypto/tech news site; the arbitration-clause claim is ❓ until checked against LG's terms. |
| [Collider — HBO Harry Potter teaser](https://collider.com/hbo-harry-potter-series-footage-change/) · [Variety — Wicked](https://variety.com/2024/film/news/wicked-color-grading-desaturated-director-jon-m-chu-1236222065/) | [03](../wiki/03-color.md) | Entertainment press; good for what filmmakers said, not for technical analysis. |
| Gamers Nexus — [LG smart TV investigation](https://www.youtube.com/watch?v=6IFVTcM28KA) | [07](../wiki/07-privacy-acr.md) | Detailed independent investigation; long and technical. We relied on V5's summary; read the original for the test conditions. |
| HDTVTest (Vincent Teoh) | [04](../wiki/04-hdr.md) | Respected measurement-based channel, cited through V3; the specific *Star Wars* analysis was not located (❓). |

## 6. Other video explainers (assessed)

Watched in full (transcripts) and used in the guide. All candidate videos found in November 2026 have now been assessed.

| Video | Used in | Assessment |
|---|---|---|
| HDTVTest (Vincent Teoh) — [5 TV Settings That Should be ILLEGAL](https://youtu.be/uGFt746TJu0) (2021) | [settings](../settings/settings-explained.md) | A certified calibrator showing sharpening halos, noise reduction erasing grain, overscan, interpolation artifacts and D65 with real footage. ⚠️ **Sponsored by the UHD Alliance**, which owns Filmmaker Mode; the advice matches independent sources, but the closing promotion is not neutral. |
| HDTVTest — [WARNING: This Sneaky TV Setting Will RUIN Your Picture Quality](https://youtu.be/AiL6ZJXta4U) (2022) | [settings](../settings/settings-explained.md#energy-saving-and-light-sensor) | Measured: energy saving on an LG C1 cut SDR peak from 170 to 92 nits and HDR from 640 to 300 nits, for ~6 W saved. One model and firmware (2022); menu paths dated. VPN sponsorship segment. |
| HDTVTest — [LG OLED TV Settings The Pros Use: SDR, HDR & Dolby Vision](https://youtu.be/YQ9E7RK0gDM) (2025) | [settings](../settings/settings-explained.md#sharpness), [names by brand](../settings/names-by-brand.md) | Current, model-specific (LG 2024–2025): Warm 50/Warm 40, sharpness 0 (default 10 still sharpens sub-4K), HDR brightness/contrast at 100, bright-room mode with gamma 2.2. LG only. VPN sponsorship segment. |
| RTINGS — [The 12 Settings We Change On Every TV](https://youtu.be/GxhZpRxB1b8) (2026) | [settings](../settings/settings-explained.md) | Lab's own baseline: Filmmaker Mode, energy saving off, BT.1886 dark / 2.2 bright, warm color temperature, local dimming high then step down, cadence "de-judder" on, HDR brightness at max, dynamic tone mapping off for accuracy, HGIG for games. Explicit that it is not a calibration. |
| Digital Trends (Caleb Denison) — [Filmmaker Mode in HDR Explained](https://youtu.be/c5kzlI6dqyg) (2024) | [settings](../settings/settings-explained.md#picture-mode) | A useful counterpoint: Filmmaker Mode assumes a dark room, and he suggests raising backlight and using minimal de-judder. Mentions Netflix/Prime Video calibrated modes and room-adaptive Filmmaker Mode. Opinionated; some terms loose ("judder" covers both cadence and stutter). |
| HDTVTest — [HDR Tone-Mapping Explained: Sony A1, LG C7 vs Panasonic OLED](https://youtu.be/Lt6IflKAmWg) (2017) | [04](../wiki/04-hdr.md#tone-mapping) | Clear side-by-side demonstration of three tone-mapping strategies (clip, lower the whole curve, track then roll off) with a pattern and real content; states that no tone-mapping standard exists. ⚠️ 2017 models and firmware; the camera exposure was lowered for the demo, as he explains. |
| Audioholics (Gene DellaSala) — [How To Set Up Your Apple TV 4K](https://youtu.be/e0i52I79NaU) (2023) | [settings](../settings/settings-explained.md#match-frame-rate-and-dynamic-range) | Practical, correct Apple TV settings (SDR default, Match Content on, Atmos on, receiver info button to verify). ⚠️ Contains affiliate links; some claims are opinions (4:4:4 chroma, "at least 100 Mbps" connection, nine-channel AVR). |
| Captain Disillusion — [CD / Color](https://youtu.be/FTKP0Y9MVus) (2020) | [03](../wiki/03-color.md#how-we-see-color-in-one-paragraph) | Accessible explanation of trichromatic vision, chromaticity and why luminance matters most when grading. ⚠️ Attributes chroma subsampling to rods outnumbering cones, an oversimplification. |
| Captain Disillusion — [CD / Blur](https://youtu.be/xDLxFGXuPEc) (2025) | [settings](../settings/settings-explained.md#sharpness) | Convolution, kernels (blur and sharpen) and why deblurring fails with noise or compression. Entertaining, technically sound at the explainer level. |
| Technology Connections — [How Analog Color TV Works](https://youtu.be/dX649lnKAU0), [Compatible Color](https://youtu.be/InrDRGTPqnE) (2017) | [02](../wiki/02-frame-rate-and-motion.md#why-tv-is-5060-hz) | Well-researched history of US color TV (CBS field-sequential vs NTSC compatible color, dates). Background only: it does not change any setting. |

## 7. Community projects

| Source | Used in | Assessment |
|---|---|---|
| [CleanYourTV](https://cleanyour.tv/) · [GitHub](https://github.com/Gathin23/cleanyourtv) (MIT) · [non-Android guide](https://cleanyour.tv/not-android) | [07](../wiki/07-privacy-acr.md#cleanyourtv-the-community-project-to-follow), [quick start](../QUICK-START.md) | The reference for smart-TV privacy and debloating: open source, updated almost daily, 513 TV models / 139 brands tested by contributors (Nov 2026), reversible by design, sourced claims. ⚠️ Young (Oct 2026) and fast-moving; the Android path needs developer mode and lets a coding assistant run commands, so read the scripts first; firmware updates undo the changes; beware of look-alike domains it warns about. |

## 8. Sources cited by the videos, not checked by us

Listed in the video descriptions and not re-checked one by one: Reddit threads, YouTube comparison videos, [4KFilmDB](https://www.4kfilmdb.com) (community database of bitrates and masters), [pan-speed calculator](https://phfx.com/tools/panSpeedCalc/) (404 in November 2026).
