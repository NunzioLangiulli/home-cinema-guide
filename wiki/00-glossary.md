# Glossary

One line per term; the link leads to the page that explains it properly.

| Term | In one line | More |
|---|---|---|
| **ACES** | Color encoding system used in film post-production, with a gamut covering the whole visible spectrum | [01](01-image-pipeline.md) |
| **ACR** (Automatic Content Recognition) | The TV computes a "fingerprint" of what it shows (HDMI included) and matches it against a database to know what you watch | [07](07-privacy-acr.md) |
| **Anamorphic** | A lens that squeezes a wide image horizontally onto film; projection "unsqueezes" it | [05](05-aspect-ratios.md) |
| **Aspect ratio** | Width/height ratio: 1.33 (4:3), 1.78 (16:9), 1.85, 2.39… | [05](05-aspect-ratios.md) |
| **Banding** | Visible steps in smooth gradients (skies, smoke), caused by too few bits and compression | [01](01-image-pipeline.md#banding-is-not-a-gamut-problem) |
| **Bitrate** | Amount of data per second (Mbps); matters more than resolution for perceived quality | [01](01-image-pipeline.md) |
| **BT.709 / Rec.709** | ITU HDTV standard: primaries, D65 white, camera curve | [03](03-color.md) |
| **BT.1886** | ITU standard (2011) for the SDR display response curve: roughly gamma 2.4 | [03](03-color.md) |
| **BT.2020 / Rec.2020** | Very wide gamut used as the "container" for UHD/HDR | [03](03-color.md), [04](04-hdr.md) |
| **BT.2100** | ITU HDR standard: defines PQ and HLG | [04](04-hdr.md) |
| **cd/m² (nit)** | Unit of luminance; 1 nit = 1 cd/m² | [04](04-hdr.md) |
| **Chromatic adaptation** | The eye adapts to the dominant white and perceives it as "white" | [03](03-color.md#why-the-eye-cant-judge-white) |
| **D65** | Reference "average daylight" white (~6504 K) | [03](03-color.md) |
| **DCI-P3** | Digital cinema gamut, wider than Rec.709 | [03](03-color.md) |
| **DCP** | Digital Cinema Package: the film "file" delivered to cinemas | [01](01-image-pipeline.md) |
| **Delta E (ΔE)** | Distance between measured and target color; below ~1–2 it is usually invisible | [08](08-calibration.md) |
| **DI (Digital Intermediate)** | The film's digital master, where final conform and color grading happen | [01](01-image-pipeline.md) |
| **Dolby Vision** | HDR format with dynamic metadata and a proprietary ecosystem | [04](04-hdr.md) |
| **EOTF** | Function converting the signal into light on the display (e.g. BT.1886, PQ) | [03](03-color.md), [04](04-hdr.md) |
| **Filmmaker Mode** | Picture mode defined by the UHD Alliance to get close to creative intent | [settings](../settings/settings-explained.md#picture-mode) |
| **Gamma** | Curve linking signal value and brightness | [03](03-color.md#gamma-why-black-matters-more-than-white) |
| **Gamut** | The set of colors a system can reproduce | [03](03-color.md) |
| **HDR10 / HDR10+** | Open HDR formats: static / dynamic metadata | [04](04-hdr.md) |
| **HLG** | "Relative" HDR curve, SDR-compatible, designed for broadcast | [04](04-hdr.md) |
| **Judder** | Uneven jerkiness caused by frames shown for different durations (3:2 pulldown) | [02](02-frame-rate-and-motion.md) |
| **Limited / Full range** | Video coding 16–235 (video standard) vs 0–255 (PC) | [settings](../settings/settings-explained.md#hdmi-black-level-range) |
| **Local dimming** | Dimming zones of an LCD backlight | [settings](../settings/settings-explained.md#local-dimming) |
| **Matrix encoding** | Dolby Stereo technique storing 4 channels in 2 tracks using phase | [06](06-audio.md) |
| **MaxCLL / MaxFALL** | HDR10 metadata: brightest pixel / highest frame-average light level | [04](04-hdr.md) |
| **Audio objects** | Sounds with a 3D position, rendered to whatever speakers exist (Atmos, DTS:X) | [06](06-audio.md) |
| **Overscan** | Enlargement that crops the picture edges; a CRT leftover | [settings](../settings/settings-explained.md#overscan-and-aspect) |
| **PLUGE** | Test pattern for setting the black point | [settings](../settings/settings-explained.md#brightness-black-point) |
| **PQ (ST 2084)** | Absolute HDR curve: each value = a number of nits, up to 10,000 | [04](04-hdr.md) |
| **3:2 pulldown** | 24 fps → 60 Hz conversion showing frames alternately 3 and 2 times | [02](02-frame-rate-and-motion.md) |
| **sRGB** | Color standard for computers and the web (1996): same primaries and white as Rec.709 | [03](03-color.md) |
| **Shutter angle** | How long each frame is exposed; 180° at 24 fps = 1/48 s | [02](02-frame-rate-and-motion.md) |
| **Stutter** | Jerky motion typical of 24p on very fast panels (OLED) | [02](02-frame-rate-and-motion.md) |
| **Telecine** | Transfer of film to a video signal | [02](02-frame-rate-and-motion.md) |
| **Tone mapping** | Compressing HDR into what the display can actually show | [04](04-hdr.md) |
| **VRR** | Variable Refresh Rate: for video games; **not** the fix for 24p films | [settings](../settings/settings-explained.md#match-frame-rate-and-dynamic-range) |
