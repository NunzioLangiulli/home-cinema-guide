# Calibration

> Main sources: V7 *This TV setting is ruining your movies* ([video](https://youtu.be/Ki1QMLMkt0A)) and the [Slidebean TV Calibrator](https://slidebean.com/tv-calibrator) app page / [FAQ](https://slidebean.com/tv-calibrator-support).

## In short

For a normal viewer, buying a colorimeter and learning calibration software makes no sense. The realistic path is:

| Level | Tool | What it does well | Limits |
|---|---|---|---|
| 0 | Menus only (Filmmaker Mode + adjustments) | Most of the result | White stays as it left the factory |
| 1 | Test patterns + your eyes | Black, white, sharpness, overscan | **Not** the color of white, nor colors |
| 2 | **Phone-camera app** (recommended for most people) | Brings white balance and colors close to target, for free, with step-by-step guidance | An approximation, not lab precision |
| 3 | Colorimeter + software (free options exist) | 2/10/20-point white balance, gamma, CMS, verified with ΔE | Cost, learning curve; for enthusiasts |
| 4 | Professional calibrator | Everything, with reference instruments | Cost |

## What calibrating means

Measuring what the screen produces (luminance and color) for a series of known signals and adjusting the controls until:
- the **greyscale** is neutral (D65) at every level: **white balance**, first at 2 points (*gain* for highlights, *offset/bias* for low levels), then at 10 or 20 points for the levels in between;
- **gamma/EOTF** follows the target (BT.1886 or 2.2 for SDR; PQ for HDR, up to the panel's limit);
- **primary and secondary colors** (R, G, B, C, M, Y) sit where the gamut says: the **CMS** (color management system: hue, saturation, luminance).

✅ V7 explains 2-point white balance ([V7 24:57](https://youtu.be/Ki1QMLMkt0A?t=1497)) and the logic of calibration ([V7 27:36](https://youtu.be/Ki1QMLMkt0A?t=1656)) clearly.

## Why a phone camera is the right idea

Our eyes adapt to whatever white they see ([why](03-color.md#why-the-eye-cant-judge-white)), so they cannot tell whether a TV is at D65. Some measurement is needed, and the phone is the measuring device everyone already owns.

The key step, as V7 explains ([V7 28:39](https://youtu.be/Ki1QMLMkt0A?t=1719)): Slidebean **measured several iPhone models against a calibrated colorimeter** and built a correction profile for each camera. The phone does not become a lab instrument, but its readings become a **fair approximation**, which is far better than the eye and than the out-of-the-box picture. That is exactly the goal: getting most viewers most of the way there, at no cost.

## The Slidebean "TV Calibrator" app

What the developer states ✅ ([FAQ](https://slidebean.com/tv-calibrator-support)):
- **iPhone with iOS 18+**; the camera is the sensor. The app never connects to the TV: it tells you which setting to change, which way, and when you're on target; you change it with the remote.
- Supported iPhone models have a **camera profile matched in advance to a professional colorimeter**; other models use a standard profile, and the app marks their readings as approximate. New profiles are added without an app update.
- Stated clearly: iPhone readings "get you close, not lab-exact".
- Workflow: greys and white first (target D65), then optionally 10/20-point greyscale, then colors (R, G, B, C, M, Y: saturation, brightness, hue) ([V7 28:08](https://youtu.be/Ki1QMLMkt0A?t=1688)).
- Patterns: YouTube playlists for SDR and HDR10; downloadable files for HDR10+ and Dolby Vision (YouTube doesn't support them).
- Privacy: no account, no ads, no tracking; data stays on the phone.
- Brands listed: LG, Samsung, Sony, TCL, Hisense, Panasonic, Philips, Vizio, Toshiba, Sharp, Roku.

### Slidebean test patterns (free)

From the "Get the test patterns" section of the [app page](https://slidebean.com/tv-calibrator#tvc-patterns). Recommended order: SDR first, then HDR10, then HDR10+ or Dolby Vision.

| Format | Where | Contents (checked 2026-11-25) |
|---|---|---|
| SDR | [YouTube playlist](https://www.youtube.com/playlist?list=PLImwyUdmQDUg), plays in the TV's YouTube app | 15 clips, ~2 min each: quick check (00), point finder (00B), 100 % white, greys 20–80 %, red, green, blue, cyan, magenta, yellow |
| HDR10 | [YouTube playlist](https://www.youtube.com/playlist?list=PLecJgdTPOhGY) | 14 clips: quick check, point finder, greys 35–70 %, the six primary/secondary colors |
| HDR10+ | [ZIP download, ~62 MB](https://pub-ab81a5ce91624340aceebc8f8f644e48.r2.dev/TV-Calibrator-HDR10plus-Patterns.zip) | For Samsung and other HDR10+ TVs; play from USB or a media player (YouTube doesn't support HDR10+) |
| Dolby Vision | [ZIP download, ~68 MB](https://pub-ab81a5ce91624340aceebc8f8f644e48.r2.dev/TV-Calibrator-Dolby-Vision-Patterns.zip) | For LG, Sony and other Dolby Vision TVs; play from USB or a media player |

⚠️ These are measurement patterns for the app (greys and colors). For black level and sharpness, V7 itself shows two by-eye patterns (next section); for white clipping and a fuller set, use AVS HD 709 (free, HD only) or the Spears & Munsil UHD HDR Benchmark disc (paid).

### The "Untangled" by-eye patterns shown in V7

V7 shows two still patterns, branded *Untangled* (Slidebean's newsletter), meant to be played **from the video itself on the TV's YouTube app**, so you adjust against the same compression your streams have. They are not in the playlists above; play V7 at the timestamps below and pause.

**How to get the video on the TV**

| Method | Steps |
|---|---|
| **Cast from your phone** (easiest, keeps the timestamp) | Open the timestamp link below on your phone (YouTube app), tap the Cast icon and pick your TV, or open the YouTube app on the TV and use *Link with TV code* (Settings → Link with TV code) to pair the phone. The video starts at the right minute. |
| **Search on the TV's YouTube app** | Search **`Slidebean This TV setting is ruining your movies`** (channel *Slidebean*, 25 Nov 2026, 34:04). Then skip to the minute shown below with the remote and pause. |
| **Direct link** (computer or phone) | [youtu.be/Ki1QMLMkt0A](https://youtu.be/Ki1QMLMkt0A) |

Before you start, set the YouTube quality to **2160p (4K)** in the player settings, or the 1-pixel bars cannot resolve. Times below are where the patterns appear in the narration; the pattern stays on screen for a few seconds, so pause as soon as it shows.

**1. TV Sharpness Check** ([V7 20:02](https://youtu.be/Ki1QMLMkt0A?t=1202))

| Part | What it shows | How to use it |
|---|---|---|
| ① Detail | Vertical and horizontal line gratings of 1, 2, 3 and 4 pixels | **4K source**: lower sharpness until the 1-px bars turn mushy, then raise it just until they are crisp: that is your neutral. 1-px bars only resolve with a 4K signal shown pixel for pixel ("Don't chase them" below 4K). |
| ② Halos | A black and a white square, thin dark and light lines on grey | Raise sharpness until test ① looks crisp **from your seat**; stop the moment a glow or outline appears along these edges. |

Assessment: ✅ a sound, brand-independent way to find the neutral point (the same principle as the sharpness patterns on calibration discs). ⚠️ Through YouTube the finest bars are already softened by compression and chroma subsampling, so the "neutral" found this way can come out slightly above the true neutral; if your brand's documented neutral (see [settings](../settings/settings-explained.md#sharpness)) differs, trust the halo test. Set Picture size to Just Scan/Fit first, or scaling will blur the 1-px bars.

**2. TV Black Level Check** ([V7 23:17](https://youtu.be/Ki1QMLMkt0A?t=1397))

| Part | What it shows | How to use it |
|---|---|---|
| ① Black level | Patches at 1, 2, 3, 4, 5, 6, 8, 10 % on a 0 % (true black) background | Lower Brightness/Black level until 1 % disappears into the background, then raise it until 2 % is barely visible. |
| ② Shadow ramp | Two gradients from 0 to ~25 % of signal | Turn each **contrast enhancer** on in turn: if the first visible step moves right, it is crushing shadows; if the background turns grey, it is lifting them. |
| Note on the pattern | "Background still grey at every setting?" | That is the LCD backlight, not the setting; judge in your usual room light. |

Assessment: ✅ the shadow-ramp test is a useful, simple way to see what "enhancement" settings do, which calibration discs rarely explain to non-experts. ⚠️ The classic PLUGE (ITU-R BT.814) also includes bars *below* black, so you set black so that below-black is invisible and just-above-black is visible. This pattern has no below-black bars, so "1 % must vanish" sacrifices the first ~1 % above black; that is a small, conservative compromise, fine for most viewers, slightly darker shadows than the reference. ⚠️ Background "true black" relies on YouTube passing level 0 correctly (limited-range video); if 0 % and 1 % never separate at any setting, check the [HDMI black level](../settings/settings-explained.md#hdmi-black-level-range).

**Status of the source code.** V7 says the code will be published on GitHub ([V7 26:00](https://youtu.be/Ki1QMLMkt0A?t=1560)). The app came out in late November 2026; as of 25 November 2026 we have not found the repository yet, and the app page does not link one. It will probably appear soon; this note will be updated with the link.

### Getting the most out of it

1. Do the [quick start](../QUICK-START.md) settings first (mode, black level, contrast, sharpness). The app works on top of a sensible base.
2. Follow the app's setup advice: dark room, phone steady (a stand helps), at the stated distance, pointed at the center.
3. **Write down your original values** before changing anything.
4. Do the **2-point white balance** first; it gives the biggest visible improvement. Move on to 10/20 points and colors if the app shows clear errors.
5. Remember: SDR, HDR10 and Dolby Vision are separate memories; repeat for each format you use.
6. Check the result on a film you know well. If something looks clearly wrong, go back to the noted values.

### Known limits (for transparency, not a reason to avoid it)

- **Camera vs colorimeter.** Colorimeters use filters designed to match the eye's response (CIE functions); phone cameras use RGB filters designed for photos, plus image processing. The per-model profiles correct for this, and they work best on display types similar to the one used for profiling. Even professional colorimeters need per-technology corrections (WOLED, QD-OLED, quantum-dot LCD…). ❓ The app does not publish which panel types were used for profiling or its measured error; once the code is public, this can be assessed.
- **Patterns via YouTube.** YouTube's compression can slightly alter levels and colors. Fine for white balance and levels; the downloadable files avoid it.

## Other phone-based options

- ✅ **Samsung Smart Calibration** (SmartThings app): uses the camera of Galaxy phones and iPhones to adjust the TV automatically; basic mode (~15–30 s) and professional mode (a few minutes, not on all models) ([Samsung](https://www.samsung.com/uk/support/apps-services/how-to-calibrate-your-tv-screen-with-smartthings/)). Samsung TVs only; no public independent accuracy data.
- ✅ **Apple TV Color Balance** (tvOS 14.5, 2021): uses the sensors of a Face ID iPhone and corrects the **Apple TV's output**, not the TV; color only, not in Dolby Vision ([MacRumors](https://www.macrumors.com/how-to/use-apple-tv-iphone-color-balance-feature/)). Independent tests found inconsistent results, sometimes worse ([MacRumors](https://www.macrumors.com/2021/05/18/apple-tv-color-balance-quality-colors-worse), [Engadget](https://www.engadget.com/apple-tv-color-balance-calibration-tests-101007281.html)). Don't stack it on top of a TV you have already calibrated.

## For enthusiasts who want to measure

| Component | Options | Notes |
|---|---|---|
| Colorimeter | i1Display Pro / Calibrite Display Pro (HL) class | Needs corrections per panel type (EDR/CCSS files or matrices) |
| Software | **HCFR** (free, open source, designed for TVs), DisplayCAL (free), Calman (paid, consumer licenses for some brands), ColourSpace (paid) | ⚠️ V7 says the cheapest software costs about $1000 ([V7 26:00](https://youtu.be/Ki1QMLMkt0A?t=1560)); free options exist, though they take time to learn |
| Patterns | Files on USB or a software/hardware pattern generator | Avoid YouTube compression for measurements |
| Guides | [RTINGS: how to calibrate](https://www.rtings.com/tv/learn/how-to-calibrate-your-tv) and per-model "settings" pages | A practical starting point |

## Recommended order

1. Basic settings ([quick start](../QUICK-START.md)).
2. Black and white levels with patterns.
3. 2-point white balance (phone app or meter).
4. 10–20-point greyscale and gamma (if the readings show errors).
5. CMS (only with readings, and only if errors are obvious).
6. Repeat for HDR10 and Dolby Vision. For Dolby Vision, options depend on manufacturer support.
