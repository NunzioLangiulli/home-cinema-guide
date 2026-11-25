# Settings explained, one by one

Each entry has the same structure:

- **What it does**: in plain words.
- **Reference**: what would match the film "as approved".
- **Why**: the technical or historical reason.
- **What the Slidebean videos say**: and what our check found.
- **When it makes sense to deviate**: justified exceptions.

Labels: ✅ verified · ⚠️ simplified · ❌ incorrect · ❓ unverified · 💬 opinion ([details](../README.md#how-to-read-the-reliability-labels)).
Names by brand are in [names-by-brand.md](names-by-brand.md).

---

## Picture mode

**What it does.** Each mode (Vivid/Dynamic, Standard, Cinema, Filmmaker…) is a pre-packaged set of settings. "Vivid/Standard" modes are designed to stand out in a shop: exaggerated blues, high saturation and sharpness, interpolation on.

**Reference.** **Filmmaker Mode** (a UHD Alliance trademark introduced in 2019) or, where missing, Cinema / Movie / Calibrated / Professional. The specification requires ✅: motion interpolation OFF, sharpening OFF, noise reduction OFF, other "enhancement" processing OFF, overscan OFF unless signaled by the content, D65 white point, and the original frame rate and aspect ratio preserved. It applies to SDR and HDR. ([What Hi-Fi](https://www.whathifi.com/advice/what-is-filmmaker-mode-is-it-any-good-and-should-you-turn-it-on), [TechCrunch 2019](https://techcrunch.com/2019/08/29/filmmaker-mode-will-automatically-turn-off-all-the-dumb-motion-smoothing-and-noise-reduction-on-new-tvs), [Hollywood Reporter](https://www.hollywoodreporter.com/movies/movie-news/martin-scorsese-christopher-nolan-launching-filmmaker-mode-tv-setting-1234968/))

**Why.** The film is approved on a reference monitor in a dimly lit room, and Filmmaker Mode tries to reproduce *that* condition. Its limit: "turning processing off" does not mean colors are exact. Every panel leaves the factory with small deviations (see [Calibration](../wiki/08-calibration.md)).

**What video 7 says.** That Filmmaker Mode is "dark and dull" and that "we can do better" ([V7 00:00](https://youtu.be/Ki1QMLMkt0A?t=0), [V7 17:16](https://youtu.be/Ki1QMLMkt0A?t=1036)).
- ✅ That it looks dark in a bright room is **acknowledged by the UHD Alliance itself**. Its October 2025 white paper says Filmmaker Mode works well in a reference environment of 5 cd/m² surround luminance, and that elsewhere viewers lose shadow visibility, causing a "perceived loss of image detail" ([UHDA PDF](https://alliance.experienceuhd.com/wp-content/uploads/2025/10/UHDA-White-Paper-on-Ambient-Light-Compensation-for-Filmmaker-Mode-v4-clean.pdf)).
- ✅ The video's practical approach is to start from a neutral base and then adjust black level, local dimming and white balance. This guide follows the same idea: **start from Filmmaker Mode and deviate in targeted ways** (panel light, gamma) rather than starting from a mode that alters everything.
- 💬 The comparison in which a 20-year-old plasma "looks better" than all the TVs in Filmmaker Mode ([V7 16:44](https://youtu.be/Ki1QMLMkt0A?t=1004)) is a visual impression filmed by a camera, without measurements.

**When to deviate.** Bright room: raise the panel light and switch to gamma 2.2 (see below). RTINGS gives the same advice: BT.1886/2.4 for a dark room, 2.2 for a brighter one ([RTINGS, 2026](https://youtu.be/GxhZpRxB1b8?t=239)). Non-film content (sports, games, 60 fps YouTube): use another memory.

**Related modes.** Some TVs (e.g. recent Sony models) switch automatically to *Netflix Adaptive Calibrated Mode* or *Prime Video Calibrated Mode* when those apps play; they aim at the same accuracy as Filmmaker Mode, often with a light sensor that adapts brightness to the room ([Digital Trends, 2024](https://youtu.be/c5kzlI6dqyg?t=631)). Some Filmmaker Mode implementations (Caleb Denison shows a Hisense) also shift **color temperature** to the room light; that departs from D65 by design, so turn it off if you want the reference ([Digital Trends](https://youtu.be/c5kzlI6dqyg?t=487)).

---

## Motion interpolation

Names: TruMotion (LG), Picture Clarity / Auto Motion Plus (Samsung), Motionflow (Sony), Intelligent Frame Creation (Panasonic), Perfect Natural Motion (Philips), MEMC / Motion Estimation (TCL, Hisense)…

**What it does.** It calculates in-between frames that do not exist in the film, to make motion smoother.

**Reference.** OFF. ✅ It is the first Filmmaker Mode requirement and the reason the mode exists (a campaign by directors including Nolan, Scorsese and P.T. Anderson; the 2018 video by Tom Cruise and Christopher McQuarrie).

**Why.** Films are shot at 24 frames per second with a typical exposure of 1/48 s (180° shutter). Motion blur and the "stepped" cadence are part of the visual language. Inventing frames produces the **soap opera effect** (a TV-video look) and artifacts around moving objects. Details in [Frame rate and motion](../wiki/02-frame-rate-and-motion.md).

**What the videos say.**
- V2 (April 2026): ✅ a correct, very clear explanation of 3:2 pulldown and interpolation ([V2 05:25](https://youtu.be/CFol4HFxVec?t=325), [V2 07:39](https://youtu.be/CFol4HFxVec?t=459)).
- V7 (November 2026) recommends **both** "stay away from motion smoothing" ([V7 33:32](https://youtu.be/Ki1QMLMkt0A?t=2012)) **and** turning on *de-judder* in the Clarity settings ([V7 11:54](https://youtu.be/Ki1QMLMkt0A?t=714)). ⚠️ The two are the same technology at different strengths: de-judder *is* motion interpolation. It also attributes the stutter to 3:2 pulldown, but on 120 Hz TVs fed a 24p signal there is no 3:2 pulldown (each frame is repeated 5 times). What remains is the **inherent stutter** of 24p, made more visible by very fast panels such as OLED ([RTINGS: stutter vs judder](https://www.rtings.com/tv/learn/research/motion-cadence)). A low de-judder setting is a reasonable personal choice, as long as you know it is interpolation.

**When to deviate.** (1) Sports and native 50/60 fps content: interpolation is a legitimate choice (V2 says so too, [33:31](https://youtu.be/CFol4HFxVec?t=2011)). (2) If 24p stutter on an OLED bothers you: the **minimum** de-judder level, knowing it is a deviation.

---

## Overscan and aspect

**What it does.** Overscan enlarges the picture by a few percent and crops its edges. It is a leftover from CRT TVs, where the edges of the signal were "dirty". Aspect options (Zoom, 16:9, Wide…) stretch or crop the picture.

**Reference.** 1:1 pixel mapping: *Just Scan* (LG, names vary), *Fit to screen* (Samsung), *Full pixel* (Sony), "Original/Auto" aspect. ✅ A Filmmaker Mode requirement (overscan only if signaled by the content).

**Why.** With overscan, a 3840×2160 picture gets rescaled: you lose sharpness and the director's framing is cropped.

**What about black bars?** They are **correct**. A 2.39:1 film on a 16:9 (1.78:1) screen **must** have bars above and below; filling the screen means cropping the sides or distorting it. History and maths in [Aspect ratios and black bars](../wiki/05-aspect-ratios.md).

---

## Energy saving and light sensor

**What it does.** Eco modes lower brightness; the ambient light sensor (Ambient light detection, AI Brightness, Eco sensor…) changes it according to room light.

**Reference.** OFF in most cases.

**How much it matters.** HDTVTest measured an LG C1 in Filmmaker Mode: SDR peak white 170 nits with energy saving off but **92 nits** with the default "Auto" in a dark room (below the 100-nit reference), and HDR peaks of 640 vs **300 nits**, with more shadow crushing; the power saved was about 6 W ([HDTVTest, 2022](https://youtu.be/AiL6ZJXta4U?t=143)). These settings often sit outside the Picture menu (LG: General → OLED Care / Energy saving; Samsung: General → Power → Brightness optimization, **per picture mode**; Sony: ambient light sensor; Philips: Eco settings → Light sensor). Manufacturers enable them by default partly to meet energy-label rules.

**Important exception (new in 2025).** The UHD Alliance has defined **ambient light compensation for Filmmaker Mode** (the *Filmmaker Mode v1.1* specification). It measures the luminance around the TV and applies a gamma correction that makes shadows more visible **without raising black and without changing white or colors**. It was validated with Hollywood colorists and 31 members of the ASC and Colorist Society, and is present "in some displays that shipped in 2025" ✅ ([UHDA PDF](https://alliance.experienceuhd.com/wp-content/uploads/2025/10/UHDA-White-Paper-on-Ambient-Light-Compensation-for-Filmmaker-Mode-v4-clean.pdf)). If your TV offers it inside Filmmaker Mode, **leave it on**: it is the only "auto brightness" approved by the creative community. ⚠️ It is only as accurate as the TV's sensor, and the paper leaves sensor calibration to the manufacturer.

✅ V7 describes it correctly as based on the TV's light sensor ([V7 16:11](https://youtu.be/Ki1QMLMkt0A?t=971)). The reference asks for a **dimly lit** room, not a lab; the compensation exists precisely for homes that aren't.

---

## Panel brightness

Names: Backlight (LCD), OLED Light / OLED Pixel Brightness (LG), "Brightness" (recent Samsung and Sony, where it means panel light).

**What it does.** It sets how much light the screen emits, **without** changing the shape of the grey curve.

**Reference.** For SDR, reference monitors work at around 100 cd/m² (nits) in a dim room ⚠️ (established studio practice; BT.1886 defines the curve, not a fixed level). In a lit room, 150–250 nits is normal.

**Why it is the first lever for a bright room.** It raises the whole picture proportionally: it changes neither white balance nor gamma. It is the "safest" deviation.

⚠️ **Watch out for names.** On many TVs the control called **"Brightness" is not panel light but the black point** (see below). This is the most common source of confusion: check [names-by-brand.md](names-by-brand.md).

---

## Brightness (black point)

Names: Brightness (many brands), Black Level 0–100 (LG from about 2023), Shadow Detail (Samsung, similar), Black level (Sony).

**What it does.** It shifts the signal's black level: too high gives grey blacks; too low loses shadow detail ("black crush").

**Reference.** Video signal black (code 16 in 8 bit, "limited range") should match the panel's black, and the first steps above black must stay visible.

**How.** PLUGE pattern: lower until the darkest square disappears, raise until 2 % is just visible. ✅ This is the procedure shown in V7 with its "Untangled" black-level pattern ([V7 23:17](https://youtu.be/Ki1QMLMkt0A?t=1397); [how to read it](../wiki/08-calibration.md#the-untangled-by-eye-patterns-shown-in-v7)) and matches established practice. ⚠️ The ITU PLUGE (BT.814) also has bars *below* black; without them, "1 % must vanish" crushes the first ~1 % above black, a small conservative compromise.

⚠️ **Note on video 3.** V3 explains pixel values as "0 to 255" ([V3 02:12](https://youtu.be/6hAVA6_Sczs?t=132)). For **video** this is not the case: by convention black is 16 and white is 235 (limited range, BT.709). That is why the next setting exists.

---

## HDMI black level (range)

Names: HDMI Black Level (Samsung: Auto/Normal/Low), Black Level Low/High (LG, older models; on newer ones it sits in the advanced settings), RGB Range / Video Range (Sony and sources), "RGB range: Limited/Full".

**What it does.** It tells the TV how to interpret values: *limited* (16–235, the video standard) or *full* (0–255, typical of PCs).

**Reference.** **Auto** on the TV, with the source set consistently. For films and streaming the signal is almost always limited.

**Why.** If the source sends limited and the TV expects full: grey blacks and a washed-out picture. The opposite: clipped shadows and highlights. A very common mistake when connecting a PC or a console. ([BGR](https://bgr.com/2158216/what-hdmi-black-level-means-how-to-adjust-it-correctly/), [Sound & Vision, LG settings](https://www.soundandvision.com/content/lg-oled65c8pua-oled-ultra-hdtv-review-settings))

The videos don't cover this setting. It is worth knowing because on some LG models "Black level" was precisely the name of the HDMI range control.

---

## Contrast

**What it does.** On many modern TVs it sets the signal's white level (gain). On some brands it is the panel light: check the brand table.

**Reference.** Usually the factory value of the Cinema/Filmmaker mode. Check with the white pattern that the brightest bars (230–235) remain distinct from full white.

---

## Sharpness

**What it does.** It **does not add detail.** It increases edge contrast, creating a subtle light/dark halo that the eye reads as "sharper".

**Reference.** The **neutral value** (nothing added, nothing softened), which **varies by brand and year**. RTINGS gives 0 for LG, Samsung, TCL, Hisense and Vizio, and 50 for Sony ([RTINGS calibration guide](https://www.rtings.com/tv/learn/how-to-calibrate-your-tv)). On recent LG OLEDs the default of 10 adds no edge enhancement to 4K but **does** sharpen sub-4K sources, so 0 is the safe neutral for everything ([HDTVTest, 2025](https://youtu.be/YQ9E7RK0gDM?t=184)). ❓ Some users measure different neutral points on specific models (e.g. 10 on some Samsungs), so the RTINGS "settings" page for your model is the safer reference.

**What V7 says.** It suggests **raising** sharpness a little to "compensate for streaming compression" ([V7 19:28](https://youtu.be/Ki1QMLMkt0A?t=1168)), with a fine-line test pattern and a check from your normal seat.
- ✅ The test method (raise until halos appear, judged from your viewing distance) is sensible, and the video is clear that sharpening "doesn't create new detail". Its "Untangled" sharpness pattern also gives a brand-independent way to find the neutral point with a 4K source ([details](../wiki/08-calibration.md#the-untangled-by-eye-patterns-shown-in-v7)).
- ⚠️ Compression removes fine detail, and sharpening cannot bring it back; it tends to amplify compression artifacts (blocks, noise, banding). So the gain is perceptual only. Captain Disillusion's explainer on blur and deconvolution shows why: even with the exact blur function known, recovering detail is wrecked by tiny amounts of noise and compression ([CD / Blur, 2025](https://youtu.be/xDLxFGXuPEc?t=376)).
- 💬 If you like a little sharpening on soft sources (DVD, low-bitrate streaming), that is a legitimate preference. Keep it low, and leave it neutral for UHD Blu-ray.

---

## Color temperature

Names: Warm 2 (Samsung, Panasonic, LG up to 2022), Warm 50 (LG 2023–2024), Warm 40 (LG 2025, per [HDTVTest](https://youtu.be/YQ9E7RK0gDM?t=120)), Expert 1 (Sony), Warm (others).

**What it does.** It shifts white towards blue (cool) or red/yellow (warm).

**Reference.** ✅ **D65** (average-daylight white, about 6504 K), the white point of Rec.709, Rec.2020 and sRGB ([ITU-R BT.709](https://www.itu.int/rec/R-REC-BT.709)). The "warmest" preset is usually the one targeting D65.

**Why it looks yellow.** Shop modes use much cooler whites (often 8000–10,000 K or more) because they "look brighter". The eye adapts to the white it sees (chromatic adaptation); after a few minutes D65 stops looking yellow. Full story in [Color](../wiki/03-color.md).

**What V7 says.** ✅ An excellent demonstration of chromatic adaptation ([V7 09:46](https://youtu.be/Ki1QMLMkt0A?t=586)). ⚠️ On Japan's white, it says it was "bluer" and that broadcasters made content "warmer to compensate" ([V7 08:42](https://youtu.be/Ki1QMLMkt0A?t=522)). The verifiable fact is that NTSC-J used a **9300 K (D93)** reference white instead of D65 ([Wikipedia NTSC-J](https://en.wikipedia.org/wiki/NTSC-J)).

---

## Gamma

Names: Gamma (2.2 / 2.4 / BT.1886), or a numeric slider (Samsung: "Gamma BT.1886" from −3 to +3).

**What it does.** It decides how signal values become brightness, especially in the dark and mid tones. Higher gamma = darker shadows and a punchier picture; lower = more open shadows.

**Reference.** ✅ **ITU-R BT.1886** (2011): the reference curve for flat-panel HDTV displays, essentially an exponent of **2.4** ([ITU](https://www.itu.int/rec/R-REC-BT.1886)). It is meant for **grading in a dark room**.

**Why it exists.** Two coinciding reasons: (1) CRTs responded to voltage with roughly this curve; (2) the eye distinguishes differences in dark tones much better, so it pays to "spend" more values in the shadows. More in [Color](../wiki/03-color.md#gamma-why-black-matters-more-than-white).

**What V3 says.** ✅ The perceptual idea (more steps in the shadows) is well explained. ❌ It says Rec.709 introduced "the famous 2.2 gamma curve" later adopted by sRGB ([V3 15:12](https://youtu.be/6hAVA6_Sczs?t=912)). In fact BT.709 defines the **camera** curve, not the display curve. For about twenty years the display curve was not standardized, until **BT.1886 with 2.4**. sRGB has its own curve, close to 2.2, designed for lit offices. ❌ The numeric example ("1 % white = 63/255") is also wrong: with gamma 2.2, 1 % luminance corresponds to about 31/255 in full range.

**When to deviate (and this is the most useful deviation).** In a **lit** room, gamma **2.2** opens up the shadows without touching white or colors. This is the principle behind the official UHDA compensation, which applies an ever lower correcting exponent as ambient light rises ([UHDA PDF, table on p. 4](https://alliance.experienceuhd.com/wp-content/uploads/2025/10/UHDA-White-Paper-on-Ambient-Light-Compensation-for-Filmmaker-Mode-v4-clean.pdf)).

---

## Local dimming

Names: Local Dimming, Local Contrast (TCL/Hisense), XR Backlight Master Drive / Local dimming (Sony), Contrast Enhancer (Samsung, ⚠️ a different thing).

**What it does (LCD / Mini-LED only).** It turns off or dims backlight zones where the picture is dark. OLEDs don't need it: each pixel emits its own light.

**Reference.** There is no "reference" value (dual-layer or OLED professional monitors don't need it). In practice it gives much better blacks; the risk is *blooming* (a halo around bright objects) and visible "pumping" of the backlight. RTINGS's approach: start at the **highest** setting and step down one notch only if blooming or pumping distracts you ([RTINGS, 2026](https://youtu.be/GxhZpRxB1b8?t=334)); a more conservative start is Medium. Either way, judge on subtitles and starfields.

**What V7 says.** ✅ It shows the benefit clearly ([V7 23:50](https://youtu.be/Ki1QMLMkt0A?t=1430)). ⚠️ It says Filmmaker Mode "turns it off": this depends on the manufacturer and model; the UHDA specification does not explicitly forbid it.

---

## Picture enhancements

Dynamic contrast, dynamic/vivid color, super resolution, noise reduction, MPEG noise reduction, "AI Picture", skin tone optimization, gamut expansion ("Native color").

**Reference.** OFF ✅ (a Filmmaker Mode requirement).

**Why.** They change the picture depending on content: the result shifts scene by scene and moves away from what the colorist approved.

**Justified exceptions.**
- **Banding reduction / smooth gradation** at minimum: useful on heavily compressed sources (skies, smoke, gradients), where banding comes from 8-bit compression ([why](../wiki/01-image-pipeline.md#banding-is-not-a-gamut-problem)).
- **Low dynamic contrast** in a very bright room: V7 suggests trying it ([V7 24:24](https://youtu.be/Ki1QMLMkt0A?t=1464)). 💬 A matter of taste: it changes gamma in a variable way. Try panel light + gamma 2.2 first.
- **Noise reduction** at minimum on old or damaged sources (digitized VHS, DVD).

---

## Enhanced HDMI format

Names: Input Signal Plus (Samsung), HDMI Ultra HD Deep Colour (LG), HDMI signal format → Enhanced (Sony), HDMI 2.0/2.1 mode (others).

**What it does.** It enables on that HDMI port the bandwidth needed for 10-bit 4K, HDR and (on 2.1 ports) 120 Hz.

**Reference.** ON for the port the 4K/HDR source is connected to. Without it, the source may fall back to SDR or reduced chroma.

---

## Match frame rate and dynamic range

Names: on Apple TV *Match Content → Dynamic Range + Frame Rate*; on Android/Google TV "Match content frame rate"; on Nvidia Shield "Match frame rate".

**What it does.** The source changes its output to suit the content: 24p for films, SDR for SDR content, HDR for HDR content.

**Why.** If the source always outputs 60 Hz, a 24 fps film goes through 3:2 pulldown **before** reaching the TV (judder). If it always outputs HDR, SDR content gets converted, often badly.

**Example: Apple TV 4K** (Settings → Video and Audio), as recommended by Audioholics ([video, 2023](https://youtu.be/e0i52I79NaU?t=443)): Format **4K SDR** (50 Hz in 50 Hz countries, 60 Hz elsewhere), **not** "4K Dolby Vision"; HDMI Output **YCbCr**; Chroma **4:4:4** if the link allows it (otherwise 4:2:0); Match Content → **Dynamic Range ON** and **Frame Rate ON**; Audio Format → Change Format **OFF**, Dolby Atmos **ON**. Expect a second or two of black screen when the format switches (QMS removes it where supported). ⚠️ The chroma choice is debated: video is stored as 4:2:0, so 4:4:4 vs 4:2:2 makes little visible difference for films; it matters more for menus and text.

**What V2 says.** ✅ The goal is right: show 24 fps content at a refresh rate that is a whole multiple of 24 ([V2 34:02](https://youtu.be/CFol4HFxVec?t=2042)). ⚠️ The suggested feature, **VRR (Variable Refresh Rate)** with a VRR-capable HDMI cable ([V2 34:33](https://youtu.be/CFol4HFxVec?t=2073)), is a gaming technology for frame rates that change continuously. For films the right feature is the source's frame-rate matching, with a TV that accepts 24p; no special cable is needed for 24p.

**Nuance: QMS-VRR.** HDMI 2.1a/2.1b added *Quick Media Switching* (QMS), which uses the VRR mechanism so the source can change frame rate (e.g. 60 Hz menus → 24p film) **without the black screen** that usually appears ([HDMI.org](https://hdmi.org/spec2sub/quickmediaswitching), [What Hi-Fi](https://www.whathifi.com/advice/what-is-quick-media-switching-qms-the-latest-hdmi-21-feature-explained)). Both source and TV must support QMS (e.g. Apple TV 4K 2022 with recent LG and Samsung OLEDs); a switch between SDR and HDR can still blank the screen. So V2's remark points at something real, but VRR alone does not match frame rate: frame-rate matching does, and QMS only makes the switch seamless.

**Naming trap.** Some brands call their *cadence* features "de-judder" too (LG *Real Cinema*, Sony *CineMotion*): these show 24p evenly and are **not** interpolation, which is why RTINGS recommends keeping them on ([RTINGS, 2026](https://youtu.be/GxhZpRxB1b8?t=383)). Interpolation-based de-judder lives under TruMotion/Motionflow/Picture Clarity.

---

## HDR tone mapping

Names: Dynamic Tone Mapping (LG), HDR Tone Mapping Static/Active (Samsung), HDR Remaster/various (Sony), "HDR Enhancer" (others). Plus the room-adaptive variants: Dolby Vision IQ, HDR10+ Adaptive.

**What it does.** An HDR film may contain highlights at 1000, 4000 or (in theory) 10,000 nits. Tone mapping "compresses" that range into what your TV can show. Full explanation in [HDR](../wiki/04-hdr.md).

**Reference.** There is no single reference: tone mapping is by definition a manufacturer's choice. The options:
- **Static / following metadata (HDR10)**: more faithful to intent when the panel is bright; can look dark on dimmer panels.
- **Dynamic** (scene by scene, computed by the TV): a brighter picture, but the TV *reinterprets* the grade.
- **Dolby Vision / HDR10+**: dynamic metadata written at mastering; the TV gets the colorist's instructions on how to compress.
- **Dolby Vision IQ / HDR10+ Adaptive**: as above plus room-light compensation. Useful in bright rooms.

💬 Many reviewers recommend dynamic tone mapping on dimmer TVs and static (or "HGIG" for games) on brighter ones. RTINGS: dynamic tone mapping **off** is the most faithful for films, **on** is brighter and punchier but less accurate, and HGIG is the choice for HDR gaming once the console is calibrated ([RTINGS, 2026](https://youtu.be/GxhZpRxB1b8?t=621)). Try both on a scene you know.

**HDR brightness and contrast.** In HDR modes leave panel light/brightness and contrast at **maximum** (LG: OLED Pixel Brightness 100, Contrast 100): the PQ signal itself sets the brightness, and lowering them breaks PQ tracking ([RTINGS](https://youtu.be/GxhZpRxB1b8?t=574), [HDTVTest](https://youtu.be/YQ9E7RK0gDM?t=443)). Room-light adjustments belong to SDR.

**What V3 says.**
- ✅ PQ (SMPTE ST 2084) is an **absolute** curve: a value means a certain number of nits. That is the root of many problems ([V3 21:48](https://youtu.be/6hAVA6_Sczs?t=1308)).
- ⚠️ "Dolby Vision is backwards compatible with HDR10" ([V3 29:22](https://youtu.be/6hAVA6_Sczs?t=1762)): true for some profiles (8.1, and 7 on disc) but **not** for profile 5, used by several streaming services, which has no HDR10 base layer ([Emby: Dolby Vision profiles](https://emby.media/learn/articles/video/hdr/formats/dolby-vision/profiles-and-compatibility/Dolby-Vision-Profile-5.html)). In practice, streaming services detect the TV and send a suitable version.
- ❌ "400 nits is enough to put HDR on the box" ([V3 26:09](https://youtu.be/6hAVA6_Sczs?t=1569)). For TVs **there is no minimum**: the word "HDR" usually just means the TV can decode the signal. Voluntary certifications set real thresholds: *Ultra HD Premium* (UHD Alliance) requires >1000 nits with black <0.05 nits, or >540 nits with black <0.0005 nits (OLED), plus ≥90 % of P3 ([What Hi-Fi](https://www.whathifi.com/advice/ultra-hd-premium-what-are-specs-which-tvs-support-it)). "DisplayHDR 400" is a VESA certification for **PC monitors**.

---

## Summary: what is "reference" and what is "choice"

| Setting | Reference | Acceptable deviation | Avoid |
|---|---|---|---|
| Mode | Filmmaker / Cinema | — | Vivid, Dynamic |
| Motion | OFF | Minimal de-judder (OLED); ON for sports | High interpolation on films |
| Overscan / aspect | Just scan / Fit | — | Zoom, Stretch |
| Panel light | ~100 nits, dark | Higher with room light | — |
| Black point | Set with PLUGE | — | Crushed shadows |
| HDMI range | Auto / consistent | — | Mismatched with source |
| Sharpness | Brand neutral | Slight increase without halos | High values |
| Color temperature | Warm 2 / Warm 50 (LG 2025: Warm 40) / Expert 1 | — | Cool / Standard |
| Gamma | 2.4 / BT.1886 | 2.2 with room light | — |
| Local dimming | — | Low/Medium | High with blooming |
| Processing | OFF | Banding reduction at minimum | High dynamic color/contrast |
| HDR tone mapping | Follow metadata | Dynamic / IQ in bright rooms or on dimmer panels | — |
| White balance | Factory (Filmmaker) | Phone-app correction, 2-point | 10/20-point and CMS by eye |
