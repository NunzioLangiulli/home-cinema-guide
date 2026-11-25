# HDR

> Main source: Slidebean, *The Brilliant Scam of "HDR"* (V3, 2026-06-25), [video](https://youtu.be/6hAVA6_Sczs), with contributions from finishing artist and colorist Paul Carlin. Additions from ITU-R BT.2100, SMPTE ST 2084, the UHD Alliance and RTINGS.

## In short

- SDR is **relative**: "100 %" means "the brightest white you have", whatever the screen.
- HDR with the **PQ** curve is **absolute**: a value means "N nits", up to 10,000. If the TV can't reach it, it must **compress** (tone mapping), and each manufacturer does that its own way.
- **HLG** is the relative, SDR-compatible alternative designed for broadcast.
- HDR10 (static metadata), HDR10+ and Dolby Vision (dynamic metadata) are different ways of telling the TV how to compress.
- HDR also brings **10-bit color and a wide gamut**, and these often make more difference than the nits.

## Why it matters: dynamic range

✅ A real scene (a sunset with rocks in shadow) can span 16–20 *stops* (doublings of light). SDR shows far fewer ([V3 04:54](https://youtu.be/6hAVA6_Sczs?t=294)).
⚠️ The video's numbers for the eye: ~24 stops with adaptation, ~14 in a single "glance". The order of magnitude is right, but estimates in the literature vary widely with method and conditions.
⚠️ Paul Carlin speaks of "six stops of SDR dynamic range" ([V3 07:03](https://youtu.be/6hAVA6_Sczs?t=423)). It depends on how it is measured: between 100 nits and a 0.1-nit black there are about 10 stops; "6" is probably the usable range of traditional SDR grading.

## The curves

| Curve | Standard | Type | Use |
|---|---|---|---|
| BT.1886 (gamma 2.4) | ITU-R BT.1886 | Relative | SDR |
| **PQ** (Perceptual Quantizer) | SMPTE ST 2084, ITU-R BT.2100 | **Absolute**, 0–10,000 nits | HDR10, HDR10+, Dolby Vision, HDR cinema |
| **HLG** (Hybrid Log-Gamma) | ITU-R BT.2100 (BBC/NHK) | Relative, SDR backward-compatible | Broadcast, some phone footage |

✅ PQ with 10 bits (1024 levels) covers up to 10,000 nits, spreading values according to the eye's sensitivity ([V3 22:21](https://youtu.be/6hAVA6_Sczs?t=1341)). ([ITU-R BT.2100](https://www.itu.int/rec/R-REC-BT.2100))
✅ Paul Carlin's critique of PQ: absolute values mean the same file looks different on every screen and in every room ([V3 21:48](https://youtu.be/6hAVA6_Sczs?t=1308)). This is the problem tone mapping, and for room light Dolby Vision IQ / HDR10+ Adaptive / the UHDA compensation, try to solve.

### How bright real material is
- ✅ Netflix requires mastering monitors of at least 1000 nits; many titles are mastered at 1000 nits, others at 4000 ([V3 31:32](https://youtu.be/6hAVA6_Sczs?t=1892)).
- ✅ The ITU's HDR production guidance puts diffuse/reference white (a white card, subtitles, graphics) at **203 cd/m²**, with everything brighter reserved for highlights ([ITU-R BT.2408](https://www.itu.int/dms_pub/itu-r/opb/rep/R-REP-BT.2408-9-2026-TOC-HTM-E.htm)). This is why a well-graded HDR film is not "brighter everywhere" than SDR.
- 💬 Carlin: "nobody uses all 1000 nits" as an average level. Reasonable: good HDR uses peaks for reflections and light sources, with an average level close to SDR.
- ✅ 10,000-nit TVs exist since 2026: the TCL X11L (CES 2026) was measured at about 10,900 nits peak ([Notebookcheck](https://www.notebookcheck.net/TCL-X11L-SQD-peaks-at-almost-11-000-nits-surpassing-HDR10-standards.1296017.0.html), [TechRadar](https://www.techradar.com/televisions/tcl-launches-next-gen-sqd-mini-led-tv-at-ces-the-best-tv-in-the-market-for-2026)). ⚠️ Peaks like that serve very little content.

## Tone mapping

The problem: the film contains a 4000-nit highlight, the TV can do 800.
1. **Clipping**: everything above 800 becomes flat white; highlight detail is lost ([V3 26:09](https://youtu.be/6hAVA6_Sczs?t=1569)).
2. **Scaling everything** proportionally: the film gets dark ([V3 26:42](https://youtu.be/6hAVA6_Sczs?t=1602)).
3. **A "knee" curve** (the real-world solution): faithful up to a point, then gradual compression of highlights. The shape of the curve is the manufacturer's choice.

✅ HDTVTest showed the trade-off side by side on three 2017 OLEDs ([HDTVTest, 2017](https://youtu.be/Lt6IflKAmWg?t=650)): one TV tracked PQ exactly and **clipped** above its ~800-nit peak (brightest picture, lost highlight detail: white shirt creases, lightning); one preserved detail up to 4000 nits by **lowering the whole curve** (all detail, darker picture); one tracked PQ up to ~100–200 nits and then **rolled off** (near-reference brightness, detail kept, some risk of posterization). There is **no standard** for tone mapping, so none of these is "wrong"; the models are old, but the three strategies still describe today's options. Also why a TV with a lower measured peak can look brighter in HDR.

✅ **HDR10** metadata (static): mastering display luminance (SMPTE ST 2086), **MaxCLL** (brightest pixel in the film), **MaxFALL** (frame with the highest average). The TV may use them to choose the curve, but many ignore them or use them only partly.
✅ Example cited: the *Mad Max: Fury Road* UHD contains a pixel at around 9000+ nits, which makes MaxCLL misleading (analysis by Vincent Teoh, HDTVTest) ([V3 27:15](https://youtu.be/6hAVA6_Sczs?t=1635)).
⚠️ V3 links this to "the whole film being too dark". That would only happen on a TV scaling linearly on MaxCLL, which almost none do. The case does show why static metadata is fragile.

**Settings**: see [HDR tone mapping](../settings/settings-explained.md#hdr-tone-mapping).

## HDR10, HDR10+, Dolby Vision

| | HDR10 | HDR10+ | Dolby Vision |
|---|---|---|---|
| Metadata | Static (whole film) | Dynamic (per scene) | Dynamic (per scene/frame) + colorist *trims* for different luminance levels |
| Licensing | Open, free | Royalty-free (Samsung-led consortium) | Proprietary (Dolby) |
| Bits | 10 | 10 | Up to 12 |
| TV support | All | Samsung, Panasonic, Philips, TCL, Hisense… | LG, Sony, Panasonic, Philips, TCL, Hisense… (not Samsung) |

✅ The video's analogy: HDR10 ≈ sRGB (simple, open, "figure it out"), Dolby Vision ≈ ColorSync (managed, closed, paid) ([V3 29:54](https://youtu.be/6hAVA6_Sczs?t=1794)). It works as an image; don't read it as literal history.
💬 Carlin: in film and episodic work "Dolby Vision is the only game in town", and he doesn't even have a tab for HDR10+ ([V3 30:27](https://youtu.be/6hAVA6_Sczs?t=1827)). A professional's testimony, not market data.
⚠️ "Dolby Vision falls back to HDR10 if the TV doesn't support it": true for discs (profile 7) and for profile 8.1, **not** for profile 5, which has no HDR10 base layer ([Emby](https://emby.media/learn/articles/video/hdr/formats/dolby-vision/profiles-and-compatibility/Dolby-Vision-Profile-5.html)). In streaming, the service chooses the version that suits the TV, so the problem mostly shows up with files and media players.

## The "HDR" label on the box

❌ V3: "with 400 nits you can write HDR on the box" ([V3 26:09](https://youtu.be/6hAVA6_Sczs?t=1569)). For TVs there is no threshold: "HDR" usually just means the TV accepts the signal. Voluntary certifications:
- **Ultra HD Premium** (UHD Alliance, 2016): >1000 nits and black <0.05 nits, **or** >540 nits and black <0.0005 nits; ≥90 % of P3; 10 bit ([What Hi-Fi](https://www.whathifi.com/advice/ultra-hd-premium-what-are-specs-which-tvs-support-it)).
- **VESA DisplayHDR 400/600/1000…** for **PC monitors**: here 400 does indicate the minimum peak.

**Choosing a TV for HDR:** look at independent measurements (peak on 10 % windows, full-screen luminance, gamut coverage, tone-mapping quality), not the logo.

## "Fake HDR" in streaming

⚠️ The video reports that the HDR versions of the original *Star Wars* trilogy on Disney+ "don't reach 10,000 nits" and are stretched SDR ([V3 24:30](https://youtu.be/6hAVA6_Sczs?t=1470)). "Doesn't reach 10,000 nits" is not a valid test: no film does. HDTVTest analyses have, however, shown titles with very low peaks, close to SDR. A **conservative** HDR grade more than a "fake" one, and it still brings 10 bits and a wide gamut. ❓ We could not locate the specific HDTVTest video cited.

## Instagram, iPhone and the web (context)

The first half of V3 is about HDR **photos** on phones and social media ([V3 08:12](https://youtu.be/6hAVA6_Sczs?t=492)): color profiles stripped by Instagram ([Engadget](https://www.engadget.com/apps/instagram-says-a-bug-turned-your-photos-black-and-white-061802389.html)), sRGB as the web's implicit default, Apple's ColorSync (1993). It is a clear explanation of why color management is hard, though it matters little for TV settings.
⚠️ "sRGB was born to give Apple the finger" is the video's caricature ([V3 16:49](https://youtu.be/6hAVA6_Sczs?t=1009)). sRGB (HP and Microsoft, 1996, later IEC 61966-2-1) was designed to give devices without color management a sensible default.
