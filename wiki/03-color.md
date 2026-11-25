# Color: white point, gamma, gamut

> Main sources: V7 *This TV setting is ruining your movies* ([video](https://youtu.be/Ki1QMLMkt0A)) and V3 *The Brilliant Scam of "HDR"* ([video](https://youtu.be/6hAVA6_Sczs)), complemented by ITU standards and the 2025 UHD Alliance white paper.

## In short

- A video system needs three agreements: **which white** (D65), **which primary colors** (the gamut: Rec.709, P3, Rec.2020), and **which curve between signal and light** (gamma/EOTF: BT.1886 for SDR, PQ/HLG for HDR).
- The eye **cannot judge white in absolute terms**: it adapts. That is why we need a standard and, to check it, a measuring device (even a phone camera).
- Shop modes use cool whites because they look brighter; D65 looks "yellow" at first.

## White: why D65

✅ Daylight changes with time, season and place. The CIE defined a standard "average day", illuminant **D65** (correlated color temperature ~6504 K) ([CIE D65](https://en.wikipedia.org/wiki/CIE_Standard_Illuminant_D65)). It is the white of **Rec.709**, **sRGB**, **Rec.2020** and of HDR mastering for the home ([ITU-R BT.709](https://www.itu.int/rec/R-REC-BT.709)) ([V7 12:57](https://youtu.be/Ki1QMLMkt0A?t=777)).
⚠️ Theatrical cinema (DCI) uses a slightly different white (about 6300 K, "DCI white"), converted to D65 for home versions.

### History: one white per country
- ✅ Original NTSC (1953) used illuminant **C**; the move to D65 came later.
- ✅ In Japan, NTSC-J used a **9300 K** (bluish) reference white ([NTSC-J](https://en.wikipedia.org/wiki/NTSC-J)).
- ⚠️ V7 says Japanese broadcasters "made content warmer to compensate" ([V7 08:42](https://youtu.be/Ki1QMLMkt0A?t=522)): we found no source confirming this (❓). The documented fact is the 9300 K white.
- ⚠️ The video attributes the preference for blue to "blue being the easiest color for CRTs to make bright" ❓. The more commonly cited explanation is perceptual and commercial: cool whites look brighter.

## How we see color, in one paragraph

✅ Color is not in the light itself: the eye has three kinds of cones (long, medium, short wavelengths) with overlapping sensitivities, and every color we see is a ratio of their responses. Different spectra can therefore look identical (metamerism), and magenta exists only in our heads, as a mix of the two ends of the spectrum. Displays exploit this: three primaries are enough to reproduce most colors inside their gamut ([Captain Disillusion, *CD / Color*, 2020](https://youtu.be/FTKP0Y9MVus?t=64)). The visual system is also far more sensitive to brightness detail than to color detail, which is why video can store color at reduced resolution (4:2:0 chroma subsampling) without visible loss. ⚠️ The video attributes this to the rods outnumbering the cones; in daylight vision rods hardly contribute, and the usual explanation is the lower spatial resolution of the eye's color-opponent channels.

## Why the eye can't judge white

✅ **Chromatic adaptation**: the visual system "re-centers" white on the dominant light. A sheet of paper looks white under a warm lamp and in daylight, even though it physically reflects very different light. V7 demonstrates this by slowly shifting the white point of the video without the viewer noticing ([V7 09:14](https://youtu.be/Ki1QMLMkt0A?t=554)).
Practical consequences:
1. Adjusting white balance **by eye** is unreliable; even an approximate measurement (a phone camera profiled against a colorimeter) beats it.
2. After switching to D65, wait a few minutes (better, one evening) before judging.
3. Room lighting affects what you perceive as white on the screen; one more reason for a neutral bias light.

## Why identical TVs in Filmmaker Mode don't match

✅ Every panel leaves the factory with tolerances: Filmmaker Mode *aims* at D65, but without calibration the result can be a few **ΔE** away ([V7 14:34](https://youtu.be/Ki1QMLMkt0A?t=874)). This is exactly the gap a calibration app is meant to close.
- ⚠️ The video attributes the variation to "LEDs and the crystals LCD panels are grown in": the explanation is loose, but the phenomenon (manufacturing variability of LEDs, phosphors/quantum dots, OLED materials) is real.
- ⚠️ "ΔE 2 → about 6200 K" is inconsistent: 6200 K is a noticeable shift from D65, usually well above ΔE 2. The video probably mixes an average greyscale error with a single point.
- **Reading ΔE (2000)**: < 1 imperceptible; 1–3 noticeable to trained eyes side by side; > 3 visible. Reviewers consider a greyscale with average ΔE < 2–3 good.

## Gamut: which colors

| Standard | Use | CIE 1931 xy area (indicative) |
|---|---|---|
| Rec.709 / sRGB | HDTV, SDR, web | ~36 % |
| DCI-P3 | Digital cinema; HDR mastering (inside a Rec.2020 container) | ~45 % |
| Rec.2020 | UHD/HDR container; no consumer TV fully covers it | ~76 % |

✅ V3 rightly notes that Rec.709 was a snapshot of what displays could do at the time ([V3 12:27](https://youtu.be/6hAVA6_Sczs?t=747)). ⚠️ Date: the first version (CCIR Rec.709) is from **1990**; the BT.709-1 revision from 1993.
**Related setting.** "Color space: Auto" is almost always right: the TV uses Rec.709 for SDR and P3/Rec.2020 for HDR. "Native/Wide" stretches SDR colors over the panel's wide gamut: more saturated but wrong colors (orange skin, fluorescent lawns).

## Gamma: why black matters more than white

✅ The eye perceives brightness non-linearly: it distinguishes small differences in dark tones far better than in bright ones. V3 shows this well: 0 % vs 5 % is visible, 100 % vs 95 % barely ([V3 12:58](https://youtu.be/6hAVA6_Sczs?t=778)). Encoding light **non-linearly** lets us devote more values to the shadows.

✅ Historical coincidence: **CRTs** also responded to voltage with a similar power curve (exponent ~2.2–2.5). "Gamma" was both a physical limit and a perceptual advantage.

### What the standards say (and where V3 slips)
- **BT.709** defines the **camera** curve (OETF), not the display's.
- **BT.1886** (2011) finally defines the SDR **display** curve: an exponent of **2.4**, formulated to account for the display's black level ([ITU](https://www.itu.int/rec/R-REC-BT.1886)).
- **sRGB** (HP and Microsoft, 1996) uses a piecewise curve close to 2.2, designed for lit offices.
- ❌ V3: "Rec.709 introduced the famous 2.2 curve copied by sRGB" ([V3 15:12](https://youtu.be/6hAVA6_Sczs?t=912)). The facts are as above.
- ❌ V3: "1 % white = 63/255" ([V3 14:37](https://youtu.be/6hAVA6_Sczs?t=877)). With gamma 2.2: 0.01^(1/2.2) ≈ 0.123 → **~31/255**. With 2.4 → ~37/255. The concept (more steps for shadows) is right, the number is not.
- ⚠️ V3 treats values as 0–255; in video, nominal values are **16–235** (limited range).

### Gamma 2.4 or 2.2?
- 2.4 / BT.1886 = **dark room**, as in the grading suite.
- 2.2 = **room with light**: more open shadows. This is the recommended deviation (see below).

## The reference viewing environment

✅ Films are approved in a room with controlled, low lighting. The standards describing it are [ITU-R BT.2035](https://www.itu.int/rec/R-REC-BT.2035) (2013) and [SMPTE ST 2080-3](https://pub.smpte.org/doc/st2080-3/) (2017). The UHD Alliance summarizes the reference condition as "a dim-surround color grading suite at 5 cd/m²" ([UHDA PDF](https://alliance.experienceuhd.com/wp-content/uploads/2025/10/UHDA-White-Paper-on-Ambient-Light-Compensation-for-Filmmaker-Mode-v4-clean.pdf)).
✅ BT.2035 (read in full) specifies: room illumination **10 lux**; background behind the monitor at **D65** and **≈10 % ±2 %** of the reference white; reference white **100 cd/m²**, black below 0.01 cd/m²; display gamma per BT.1886; for 1080p an optimal viewing angle of **31°** (3.2 × picture height); and no added ringing (sharpening) or motion artefacts ([ITU-R BT.2035 PDF](https://www.itu.int/dms_pubrec/itu-r/rec/bt/R-REC-BT.2035-0-201307-I!!PDF-E.pdf)). It also states that consumer displays should not be used for professional evaluation, a reminder that home viewing can only approximate this.

**Bias light.** In grading suites the wall behind the monitor is neutral grey, lit by a dim D65 light (V7 mentions the "special paint" in Paul Carlin's studio, [V7 03:12](https://youtu.be/Ki1QMLMkt0A?t=192)). At home the equivalent is an **LED strip behind the TV**, as neutral as possible (high CRI, ~6500 K) and dim: about **10 %** of the screen's white luminance ✅ (BT.2035 above; the older SMPTE RP 166 gave the same ratio).

## Why Filmmaker Mode looks dark

✅ Primary source: [UHD Alliance, *Ambient Light Compensation for Filmmaker Mode*, October 2025](https://alliance.experienceuhd.com/wp-content/uploads/2025/10/UHDA-White-Paper-on-Ambient-Light-Compensation-for-Filmmaker-Mode-v4-clean.pdf).

1. Filmmaker Mode reproduces the picture for a **5 cd/m²** surround.
2. In a brighter room the eye adapts to the surround and loses contrast sensitivity in the shadows, so dark detail falls below the visibility threshold. The paper calls this the **primary source of negative feedback** on Filmmaker Mode. V7 is right to raise it.
3. The UHDA solution (part of the **Filmmaker Mode v1.1** specification, in some 2025 TVs):
   - works **after** tone mapping, on the PQ signal;
   - normalizes between the **display's** black and white, applies a **gamma exponent < 1**, and re-normalizes;
   - therefore it **does not raise black, does not clip highlights, and does not change white or colors**: it only opens up dark and mid tones;
   - the exponents were chosen by Hollywood colorists in a visual matching test and validated with 31 members of the ASC and Colorist Society.

| Luminance around the TV (cd/m²) | 5 | 10 | 20 | 40 | 80 | 160 | 320 | 500 |
|---|---|---|---|---|---|---|---|---|
| Correcting exponent | 1.0 | 0.980 | 0.954 | 0.913 | 0.859 | 0.794 | 0.715 | 0.668 |

**What this means if your TV lacks the feature.** The colorists themselves approved a **gamma-only** correction for bright rooms. Moving from 2.4 to 2.2 in a lit room is therefore a deviation consistent with creative intent. Raising saturation or turning on dynamic contrast is not.

## Why recent films "look dull"

💬/⚠️ V7 offers an explanation (post-production time, more versions to grade: HDR, SDR, Dolby Vision) backed by trade articles ([V7 30:49](https://youtu.be/Ki1QMLMkt0A?t=1849)):
- ✅ Netflix asks for the HDR (Dolby Vision) grade first, then an SDR *trim pass* ([Netflix guidelines](https://partnerhelp.netflixstudios.com/hc/en-us/articles/360000599948-Dolby-Vision-HDR-Mastering-Guidelines)).
- ✅ Examples cited: the corrections to the HBO *Harry Potter* teaser ([Collider](https://collider.com/hbo-harry-potter-series-footage-change/)), and Jon M. Chu's comments on *Wicked*'s color ([Variety](https://variety.com/2024/film/news/wicked-color-grading-desaturated-director-jon-m-chu-1236222065/)).
- 💬 That Hollywood desaturates "so as not to look like a TV ad" is the video's hypothesis, not a fact.
- For viewers: a "dull" picture in Filmmaker Mode may be **intentional**. Before "fixing" it with saturation, try the same scene in another version (UHD vs streaming) or read what the cinematographer or colorist has said.
