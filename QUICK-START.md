# Quick start: setting up your TV for films, step by step

> This page tells you **what to do and in what order**. The **why** behind each step is in [Settings explained](settings/settings-explained.md) (linked next to each item). Exact menu names per brand are in [Names by brand](settings/names-by-brand.md).

**Time:** level 1 ≈ 15 minutes · level 2 ≈ 45 minutes · level 3 ≈ one evening.
**You need:** the remote, a film you know well, and test patterns (free, see [Level 2](#level-2--adjustments-with-test-patterns-45-min)).

---

## Before you start (5 minutes)

1. **Update the firmware** of the TV and of any external player or streaming box. Manufacturers often fix tone mapping and picture modes in updates.
2. **Photograph your current menus** with your phone so you can always go back.
3. **Judge the TV in the conditions you actually use it in**: the same evening light, the same seat. Settings that are right for a dark room are not right for a sunny living room. This is the main reason Filmmaker Mode "looks dark" ([why](wiki/03-color.md#why-filmmaker-mode-looks-dark)).
4. Remember: **SDR, HDR10, HDR10+ and Dolby Vision have separate settings.** Whenever you adjust something, do it while content in that format is playing, or you will change the wrong memory.

---

## Level 1 — The five things that matter most (15 min)

| # | What to do | Why, in one line | Details |
|---|---|---|---|
| 1 | Choose **Filmmaker Mode** (or Cinema / Movie / Calibrated / Professional) | It is the mode closest to how the film was approved: D65 white, no added processing | [→](settings/settings-explained.md#picture-mode) |
| 2 | **Motion interpolation OFF** (TruMotion, Motionflow, Picture Clarity, MEMC, Intelligent Frame Creation…) | It invents frames that do not exist: the "soap opera effect" | [→](settings/settings-explained.md#motion-interpolation) |
| 3 | **Picture size: "Fit to screen" / Just Scan / Full pixel**, overscan OFF | Shows every pixel without cropping or rescaling | [→](settings/settings-explained.md#overscan-and-aspect) |
| 4 | **Energy saving and auto brightness OFF** (or at least check them; often outside the Picture menu, and on Samsung set per picture mode) | They change brightness unpredictably; one measured LG lost almost half its brightness | [→](settings/settings-explained.md#energy-saving-and-light-sensor) |
| 5 | **Set the panel light for your room** (Backlight / OLED Pixel Brightness / "Brightness" on recent Samsung) | The reference assumes a dark room; in a brighter one you can raise the light **without** touching white or gamma | [→](settings/settings-explained.md#panel-brightness) |

If you stop here you have already fixed most problems. If the picture still looks too dark in a bright room, go to [Level 2, step 5 (gamma)](#5-gamma).

---

## Level 1b — The source matters as much as the TV

| What to do | Why | Details |
|---|---|---|
| Connect your player/box to an HDMI port with the **enhanced format enabled** (Input Signal Plus, HDMI Ultra HD Deep Colour, HDMI Enhanced format…) | Without it, many TVs do not accept 10-bit 4K HDR | [→](settings/settings-explained.md#enhanced-hdmi-format) |
| On the external box (Apple TV, Shield, Fire TV…): **match dynamic range and frame rate to the content** ("Match Content" on Apple TV) | Stops SDR films being converted to "fake" HDR, and 24 fps films being forced to 60 Hz (judder) | [→](settings/settings-explained.md#match-frame-rate-and-dynamic-range) |
| Check that the TV's **HDMI black level** (Auto/Limited/Full) matches the source output | If they don't match: grey blacks or crushed shadows | [→](settings/settings-explained.md#hdmi-black-level-range) |
| Use the best source you have: **UHD Blu-ray > high-bitrate streaming > regular streaming** | Compression removes more quality than "4K" adds | [→](wiki/01-image-pipeline.md) |

---

## Level 2 — Adjustments with test patterns (45 min)

**Recommended patterns** (free): for black level and sharpness, the two "Untangled" check patterns shown in Slidebean's video *This TV setting is ruining your movies* (on the TV's YouTube app search **`Slidebean This TV setting is ruining your movies`**, or cast it from your phone), set to 4K and paused at the right minute ([black level at 23:17](https://youtu.be/Ki1QMLMkt0A?t=1397), [sharpness at 20:02](https://youtu.be/Ki1QMLMkt0A?t=1202); how to read them in [Calibration](wiki/08-calibration.md#the-untangled-by-eye-patterns-shown-in-v7)). For white clipping and a fuller set, AVS HD 709 (HD) or the Spears & Munsil UHD HDR Benchmark disc (paid). For white balance and colors with the phone app, Slidebean's SDR and HDR10 YouTube playlists plus HDR10+ and Dolby Vision files (all links in [Calibration](wiki/08-calibration.md#slidebean-test-patterns-free)). Alternatively, pattern files played from a USB stick (for example the AVS HD 709 set or similar), which avoid YouTube's re-compression. ⚠️ Patterns on YouTube go through YouTube's compression: fine for black, white and sharpness, less so for fine measurements.

Do the steps **in this order** (each one affects the next):

### 1. Black level ("Brightness" / "Black level" / "Shadow detail")
Pattern: near-black squares (1 %, 2 %, 3 %… on a black background), known as *PLUGE*.
Lower the control until the darkest square disappears, then raise it one step until the next one is **just** visible. If you lose squares above 3 % you are throwing away shadow detail.
[Why →](settings/settings-explained.md#brightness-black-point)

### 2. Contrast (white as a level, not as a color)
Pattern: near-white bars. Raise until the brightest bars are still distinguishable; if they merge into white, lower it. On many modern TVs the factory value is already correct.
[Why →](settings/settings-explained.md#contrast)

### 3. Sharpness
Set your **brand's neutral value** (often 0; 50 on some Sony models — check the RTINGS "settings" page for your model), or find it with the Untangled sharpness pattern: with a 4K source, lower until the 1-px bars go mushy, then raise just until they are crisp. Only then, if you wish, try raising it slightly **from your viewing distance**: stop as soon as halos appear around edges.
[Why, and why it is debated →](settings/settings-explained.md#sharpness)

### 4. Color temperature
**Warm 2 / Warm 50 / Expert 1** (depends on the brand): this is the preset that targets D65. It will look "yellowish" for the first few minutes; that is your eye adapting, not a defect ([why](wiki/03-color.md#why-the-eye-cant-judge-white)).
[Why →](settings/settings-explained.md#color-temperature)

### 5. Gamma
- **Dark** room: **BT.1886** or **2.4**.
- Room **with light**: **2.2** (or the brightest step available).
This is the "cleanest" deviation for a bright room: it opens up shadows without changing white or colors. It follows the same principle as the UHD Alliance's official ambient light compensation algorithm ([wiki](wiki/03-color.md#why-filmmaker-mode-looks-dark)).
[Why →](settings/settings-explained.md#gamma)

### 6. Local dimming (LCD/Mini-LED only)
Start high (RTINGS's approach) or at Medium: it gives much deeper blacks. If you see halos (blooming) around subtitles or bright objects on a black background, or the backlight visibly "pumping", go down one level.
[Why →](settings/settings-explained.md#local-dimming)

### 7. Picture "enhancements": all OFF, then turn back on only what you need
Noise reduction, MPEG/digital noise reduction, super resolution, dynamic contrast, dynamic color, "AI picture", skin tone, color optimizers.
To see what each one does, use the shadow ramp of the Untangled black-level pattern: if the first visible step moves right, the setting is crushing shadows; if the background turns grey, it is lifting them.
Reasonable exceptions: **banding reduction / smooth gradation at minimum** on heavily compressed sources; **low dynamic contrast** only if you watch in daylight and accept moving away from the reference.
[Why →](settings/settings-explained.md#picture-enhancements)

### 8. Repeat for HDR
Start HDR10 content (then Dolby Vision / HDR10+ if you have it) and repeat: mode, motion, sharpness, color temperature. In HDR **do not** handle brightness and contrast the same way: leave panel light and contrast at **maximum** (the HDR signal itself sets brightness), and choose a tone-mapping behavior instead ([tone mapping](settings/settings-explained.md#hdr-tone-mapping)).

---

## Level 2b — Motion: if 24p "stutters"

On OLEDs and fast Mini-LEDs, 24 fps films can look jerky in pans. Before turning on any smoothing:

1. Make sure the source really sends **24p** (see "Match frame rate" above) and that the TV shows frames evenly (LG: *Real Cinema* ON; others: "Film mode"/"Cinema" detection).
2. If it still bothers you, use **the lowest level** of de-judder (e.g. LG *Cinematic Movement*, Samsung *Judder Reduction* 1–3, Sony *CineMotion*/Motionflow "True Cinema"). Know that this **is interpolation**, so a deviation from the original ([why](wiki/02-frame-rate-and-motion.md#judder-stutter-and-what-you-can-do)).
3. For sports and native 50/60 fps content, interpolation is a legitimate choice: create a **second memory** (e.g. "Standard" or "Sport" mode) for those.

---

## Level 2c — The room

| What | Why |
|---|---|
| Remove direct **reflections** on the screen (lamps, windows opposite) | A reflection raises perceived black more than any setting can lower it |
| In the evening, a **dim light behind the TV** (bias light), as neutral white as possible (around D65, ~6500 K) | Reduces eye strain and keeps contrast perception stable; it imitates the "surround" of grading suites ([wiki](wiki/03-color.md#the-reference-viewing-environment)) |
| Distance: to see 1080p vs 4K differences you need to sit fairly close (the screen should fill roughly 30–40° of your field of view) | Further back, 4K is indistinguishable from 1080p ([wiki](wiki/01-image-pipeline.md#when-4k-is-actually-visible)) |

---

## Level 2d — Audio

| What to do | Why | Details |
|---|---|---|
| With a soundbar/AV receiver: TV set to **eARC/ARC output, format "Passthrough"/"Bitstream"/"Auto"** | Lets the audio device decode Dolby/DTS | [→](wiki/06-audio.md#practical-settings) |
| Dialogue hard to hear: raise the **center channel** by 2–3 dB (receiver) or enable **dialogue enhancement / clear voice** | Film mixes have wide dynamic range; dialogue lives in the center channel | [→](wiki/06-audio.md#why-dialogue-is-hard-to-understand) |
| At night: **night mode / DRC / dynamic compression** | Narrows the gap between dialogue and explosions | [→](wiki/06-audio.md#why-dialogue-is-hard-to-understand) |
| After placing the speakers, run the receiver's **microphone calibration** (Audyssey, Dirac, YPAO, Room EQ…) | Compensates for distances, levels and room acoustics | [→](wiki/06-audio.md#atmos-in-practice) |

---

## Level 2e — Privacy (5 min, recommended)

The most up-to-date guide is the community project [CleanYourTV](https://cleanyour.tv/) (step-by-step for Samsung, LG, Roku, Vizio, VIDAA, Fire TV; a reversible debloat for Android/Google TV). Summary:


1. In the Privacy/Terms menu, turn off **content recognition (ACR)**: *Viewing Information Services* (Samsung), *Live Plus* and "viewing information" (LG), *Samba Interactive TV* (Sony), and equivalents on Google TV/Roku/VIDAA. ⚠️ ACR also analyzes what comes in **over HDMI** ([wiki](wiki/07-privacy-acr.md)).
2. Turn off **personalized advertising** and, if you don't use voice control, the microphone.
3. Strong option: use an **external box** for streaming and keep the TV **offline**, or isolate it on a guest network/VLAN.

---

## Level 3 — Calibrating white balance with your phone (one evening)

Only after everything else. For most people the right tool is the **smartphone** ([full comparison](wiki/08-calibration.md)):

1. **Phone-camera apps** (Slidebean *TV Calibrator* on iPhone, Samsung *Smart Calibration*). The app reads the screen with the camera, using correction profiles matched to a professional colorimeter, and tells you which control to move. It gives a good approximation for free, which is a big step up from the factory picture. Note your original values, and compare before/after on a film you know.
2. **Colorimeter + free software** (e.g. HCFR or DisplayCAL with an i1Display Pro-class meter): only for enthusiasts who want measured precision.
3. **Professional calibrator** (ISF/THX): the best result, at a cost.

⚠️ Golden rule: **adjust 2-point white balance first; touch 10/20-point and the color management system (CMS) only with readings to guide you.** Adjusting them by eye usually makes things worse.

---

## Printable checklist

```
[ ] Firmware updated
[ ] Mode: Filmmaker/Cinema (SDR)   [ ] (HDR10)   [ ] (Dolby Vision)
[ ] Motion interpolation OFF (conscious exception: minimal de-judder)
[ ] Picture size: Fit to screen / overscan OFF
[ ] Energy saving / auto brightness OFF
[ ] Enhanced HDMI format ON for the port in use
[ ] Source: match dynamic range + frame rate ON
[ ] HDMI black level consistent with the source
[ ] Brightness (black point) set with PLUGE
[ ] Contrast checked with white pattern
[ ] Sharpness at the brand's neutral value
[ ] Color temperature: Warm 2 / Warm 50 / Expert 1
[ ] Gamma: 2.4/BT.1886 (dark) or 2.2 (light)
[ ] Local dimming: Low/Medium without obvious blooming
[ ] "AI/dynamic" processing OFF
[ ] Audio: eARC passthrough, center level, night mode if needed
[ ] Privacy: ACR OFF, personalized ads OFF
[ ] Optional: white balance with a phone calibration app
```
