# Frame rate and motion

> Main source: Slidebean, *yeah... no wonder movies look cheap on new TVs* (V2, 2026-04-18), [video](https://youtu.be/CFol4HFxVec). De-judder sections from V7 ([video](https://youtu.be/Ki1QMLMkt0A)).

## In short

- Cinema shoots at **24 frames per second**; TV was born at **50/60 Hz** because it was tied to the mains frequency. The two worlds were never compatible.
- Converting 24 → 60 forces frames to be shown for different durations (**3:2 pulldown**), causing uneven jerkiness (**judder**).
- Modern **120 Hz** TVs can show each frame 5 times (**5:5**), removing pulldown judder. What remains is the **stutter** inherent to 24p, more visible on OLEDs.
- **Interpolation** removes the jerkiness by inventing frames: that is the "soap opera effect".

## Why 24 fps

✅ In the silent era speed was not fixed (often 16–20 fps, hand-cranked). With synchronized sound (late 1920s) a constant speed was needed, and **24 fps** became the standard ([V2 12:24](https://youtu.be/CFol4HFxVec?t=744), [V2 16:39](https://youtu.be/CFol4HFxVec?t=999)).
✅ At 24 fps, one minute of 35 mm (4-perf, 16 frames per foot) is exactly **90 feet** ([V2 17:14](https://youtu.be/CFol4HFxVec?t=1034)).
⚠️ "Persistence of vision" is, as the video admits, a simplification. Apparent motion is explained today by the *beta movement* / *phi phenomenon* and by the flicker fusion threshold ([V2 11:17](https://youtu.be/CFol4HFxVec?t=677)).
✅ Film projectors show each frame 2 or 3 times (two- or three-bladed shutter) to raise flicker to 48/72 Hz: this is the "trick" the video mentions ([V2 12:24](https://youtu.be/CFol4HFxVec?t=744)).

## Why TV is 50/60 Hz

✅ Early TV sets locked their field rate to the mains frequency (60 Hz in North America, 50 Hz in Europe) to avoid hum bars ([V2 20:58](https://youtu.be/CFol4HFxVec?t=1258)). Hence 30/60 and 25/50.
✅ With NTSC color (1953) the rate became **59.94 Hz / 29.97 fps** ([V2 22:07](https://youtu.be/CFol4HFxVec?t=1327)). The color system had to be **compatible** with existing black-and-white sets: color was added as a subcarrier on top of the black-and-white (luminance) signal. The FCC approved it on 17 December 1953, the first nationwide color broadcast followed on 1 January 1954, but most US broadcasts were in color only from 1965 and color sets outsold black-and-white ones only in 1972 ([Technology Connections, *Compatible Color*](https://youtu.be/InrDRGTPqnE?t=629); background in [*How Analog Color TV Works*](https://youtu.be/dX649lnKAU0)).
✅ In Europe, films on TV were **sped up by 4 %** (24 → 25 fps): higher voices and shorter films (*Home Alone*: ~103 → ~99 minutes, [V7 11:21](https://youtu.be/Ki1QMLMkt0A?t=681)). Pitch was sometimes corrected during transfer ([V2 23:41](https://youtu.be/CFol4HFxVec?t=1421)).
✅ Shows such as *Friends* and *Seinfeld* were shot on 35 mm film at 24 fps ([V2 24:49](https://youtu.be/CFol4HFxVec?t=1489)), which is why HD remasters exist.

## 3:2 pulldown

✅ 60 / 24 = 2.5: you cannot show each frame for a whole number of refresh cycles. Frames alternate between 3 and 2 repetitions (A A A B B C C C D D…). One frame lasts 50 ms, the next 33 ms, so pans **judder** ([V2 05:25](https://youtu.be/CFol4HFxVec?t=325)). Cinematographers limit pan speed partly for this reason (the video cites a pan-speed calculator at [phfx.com](https://phfx.com/tools/panSpeedCalc/), no longer reachable in November 2026).

## Judder, stutter and what you can do

RTINGS distinguishes ✅ ([RTINGS](https://www.rtings.com/tv/learn/research/motion-cadence)):
- **Judder**: uneven cadence caused by 3:2 pulldown. It *can be fixed* by sending 24p to a TV that shows it at a whole multiple (120 Hz → 5:5, or 48/72 Hz).
- **Stutter**: each frame is held still for 1/24 s, and panels with very fast response times (OLED) jump to the next one "abruptly", without the slight smear of slower LCDs. It is **inherent to 24p** and can only be masked.

What to do, in order:
1. **Source at 24p** (match frame rate): [settings](../settings/settings-explained.md#match-frame-rate-and-dynamic-range).
2. A **120 Hz** TV or one with an even-24p mode (e.g. LG *Real Cinema*).
3. If stutter bothers you: **de-judder at minimum**, knowing it is interpolation.

⚠️ V2 points to **VRR** with a dedicated HDMI cable as the fix ([V2 34:33](https://youtu.be/CFol4HFxVec?t=2073)). VRR is a gaming technology; for films the right feature is frame-rate matching at the source.
⚠️ V7 recommends de-judder ([V7 11:54](https://youtu.be/Ki1QMLMkt0A?t=714)) and later says to stay away from motion smoothing ([V7 33:32](https://youtu.be/Ki1QMLMkt0A?t=2012)). Both are the same technology at different strengths; a low de-judder level is a reasonable compromise on OLEDs if you treat it as a conscious deviation.

## Interpolation and the soap opera effect

✅ The TV computes in-between frames by estimating motion ([V2 07:39](https://youtu.be/CFol4HFxVec?t=459)). The name comes from soap operas, shot on video at 50/60 fields per second and so with smoother, "live" motion.
💬 The aesthetic judgement (Rian Johnson's "liquid diarrhea"; the Cruise/McQuarrie campaign) is the directors' opinion, but it is also **the criterion behind Filmmaker Mode**.
✅ The *Spider-Verse* case: Miles Morales is animated "on twos" (12 poses per second) in the first part of the film to show his inexperience ([V2 14:29](https://youtu.be/CFol4HFxVec?t=869)). Interpolation erases that narrative choice. The same applies to stop motion.

## Shutter angle: why motion blur is part of the "look"

✅ With a **180°** rotating shutter at 24 fps, each frame is exposed for **1/48 s**: cinema's natural motion blur ([V2 27:02](https://youtu.be/CFol4HFxVec?t=1622)).
✅ *Saving Private Ryan*: Janusz Kamiński used narrow shutters (45°, about **1/192 s**) for the landing, giving "frozen", nervous images ([V2 28:41](https://youtu.be/CFol4HFxVec?t=1721)). The same effect appears in *Gladiator* and *Children of Men*.
⚠️ The video says "we don't have rolling shutters in our digital cameras" ([V2 28:41](https://youtu.be/CFol4HFxVec?t=1721)); probably a slip of the tongue. Most digital cameras **do** have an electronic rolling shutter; the *shutter angle* is set as an exposure time.

## The HFR experiment

✅ *The Hobbit* (2012) was shot and released also at **48 fps** (HFR), partly to reduce 3D problems. Reception was negative because of the "video" look ([V2 18:17](https://youtu.be/CFol4HFxVec?t=1097)). Later attempts (e.g. Ang Lee at 120 fps, *Avatar: The Way of Water* with variable HFR) have not changed the standard.
💬 The video asks a fair question: if the director *wants* HFR, respecting intent means watching it that way.

## In practice

| Content | Setting |
|---|---|
| Films, series shot at 24 fps | Interpolation OFF; source at 24p; TV at 120 Hz / even 24p |
| OLED with bothersome stutter | De-judder at minimum (conscious deviation) |
| Sports, live events at 50/60 fps | Interpolation to taste (separate memory) |
| Video games | Game mode; VRR **yes** (this is where it belongs) |
