# The image pipeline: from set to living room

> Main source: Slidebean, *The Biggest Mistake in the History of Hollywood* (V1, 2026-02-20), [video](https://youtu.be/yN0H_WfWOp4). Additions and corrections are marked with labels.

## In short

1. For decades a film was **film from start to finish**: a work print was cut, the negative conformed to it, color corrected at the lab with filters and chemistry, and prints made for cinemas ([V1 01:04](https://youtu.be/yN0H_WfWOp4?t=64)).
2. From around 2000 the **Digital Intermediate (DI)** took over: the negative is scanned, conformed and graded on a computer. The DI becomes **the master**; everything you will see (cinema, Blu-ray, streaming) derives from it.
3. If the DI is **2K**, any "4K" version is necessarily an **upscale**, unless someone goes back to the negative.
4. Between the master and your living room, quality is lost mainly to **compression** (bitrate), not resolution.

## The Digital Intermediate and "fake 4K"

✅ *O Brother, Where Art Thou?* (2000, shot by Roger Deakins) is the classic case of the first feature fully color-graded digitally: the negative was scanned at 2K, graded on a computer and recorded back to film ([American Cinematographer](https://theasc.com/articles/o-brother-cinematography-deakins)). ✅ 2K DIs then became the norm for years. For a widescreen film the usable resolution is around 2048×858.

**Practical consequence.** Many "4K" releases of 2000s–2010s films are upscaled 2K masters. ✅ The video cites *The Lord of the Rings*, *Mad Max: Fury Road* (shot digitally, 2K DI), *Prometheus* and *The Social Network*. To check a specific title, databases such as [4KFilmDB](https://www.4kfilmdb.com) or the *Real or Fake 4K* site exist.

⚠️ "Fake 4K" is a strong label. A good 2K upscale **with HDR and 10-bit color** can still beat the 1080p Blu-ray, because the UHD disc also brings more bitrate and more color depth. Resolution is not the only improvement.

✅ The opposite case: *Big Fish* (original 2K DI) was **rescanned from the negative in 4K** for UHD Blu-ray ([V1 26:15](https://youtu.be/yN0H_WfWOp4?t=975)). ✅ *Spider-Man 2* (2004) is often cited as the first 4K DI, with visual effects rendered at 2K ([V1 12:30](https://youtu.be/yN0H_WfWOp4?t=750)).

### How much resolution does film have?
⚠️ The video reports the "general consensus" that a 4K scan captures all the detail in a 35 mm negative ([V1 11:57](https://youtu.be/yN0H_WfWOp4?t=717)). In reality detail depends on the stock, lenses, exposure and which element is scanned (original negative vs a much softer release print). The debate is open; "4K is enough for almost all 35 mm" is a good approximation, not a law.

### IMAX 70 mm
- ❌ "IMAX 70 mm is four times 35 mm" ([V1 28:23](https://youtu.be/yN0H_WfWOp4?t=1703)). An **IMAX 15/70** frame (15 perforations, running horizontally) is roughly **10 times** the area of a standard 35 mm frame; it is 5-perf 70 mm that is about 3.5 times.
- ❌ "Nolan's films have no digital intermediate" and "only four cinemas in the world project IMAX 70 mm". For *Oppenheimer* (2023) the film prints came from a **photochemical** grade, but the digital versions (DCP and IMAX digital) were made from **8K scans** of the film elements ([technical notes via in70mm.com](https://in70mm.com/presents/1970_imax/2023_oppenheimer/format/index.htm), [8K Association](https://8kassociation.com/oppenheimer-scanned-in-8k/)). About **30** IMAX 70 mm cinemas showed it ([CNBC](https://www.cnbc.com/2023/07/19/where-to-watch-oppenheimer-in-70mm-imax-.html)).

## When 4K is actually visible

✅ Whether you can tell 1080p from 4K depends on **screen size and distance**, i.e. the angle the screen fills in your field of view. The video uses the [RTINGS](https://www.rtings.com/tv/reviews/by-size/size-to-distance-relationship) chart: a 75" TV at 2.8 m (~33°) is at the edge of visibility ([V1 13:27](https://youtu.be/yN0H_WfWOp4?t=807)).

Practical references:
- SMPTE indicates a minimum of about **30°** of field of view for cinema-like viewing; THX recommends **~36–40°** ⚠️ (widely quoted values; the original documents are not freely available).
- In practice, for a 65" TV you need to sit closer than ~2.5 m to appreciate 4K.

✅ It is also why **many films are still mastered in 2K**: at typical cinema distances most seats cannot tell 2K from 4K ([V1 14:07](https://youtu.be/yN0H_WfWOp4?t=847)).

## Compression: the real bottleneck

Orders of magnitude (✅ where marked; the rest are the video's estimates):

| Version | Size / bitrate | Notes |
|---|---|---|
| 4K DI (e.g. *Blade Runner 2049*) | ~1.7 TB (video's ProRes estimate) | The "purest" version |
| Cinema DCP | ~300–600 GB | JPEG 2000, up to 250 Mbps (DCI spec) |
| UHD Blu-ray | up to 66/100 GB; peak video bitrate above 100 Mbps | ✅ the video's "up to 144 Mbps" is the disc's maximum read rate, not the average video bitrate |
| Kaleidescape | up to ~100 Mbps (manufacturer's figure) | ⚠️ the video says "65 Mbps average"; the manufacturer states up to 100 Mbps ([Kaleidescape](https://www.kaleidescape.com/compare/)) |
| Sony Pictures Core (Pure Stream) | up to 80 Mbps | ✅ ([TweakTown](https://www.tweaktown.com/news/77290/sony-bravia-core-movie-service-near-lossless-4k-blu-ray-streaming/index.html)); only on compatible Sony devices |
| Typical 4K streaming | 15–40 Mbps | ✅ the video's ranking from 4KFilmDB: Apple TV > HBO > Netflix > Amazon ([V1 19:04](https://youtu.be/yN0H_WfWOp4?t=1144)) |

⚠️ Comparing bitrates across codecs (JPEG 2000, HEVC, AV1) is not linear: at the same Mbps, modern codecs are far more efficient. Bitrate is still the simplest indicator.

⚠️ The video says streaming is also held back by TVs' 100 Mbps Ethernet ports ([V1 19:37](https://youtu.be/yN0H_WfWOp4?t=1177)). Many TVs do have 100 Mbps Ethernet, but streaming stops at ~40 Mbps, well below that limit. The main brakes are delivery (CDN) costs and device compatibility.

## Banding is not a gamut problem

❌ The video blames the banding seen in *Blade Runner 2049* on the Rec.709 gamut: the oranges between two shades "no longer exist" ([V1 18:31](https://youtu.be/yN0H_WfWOp4?t=1111)). This is wrong. The **gamut** says *which* colors can be represented (the corners of the triangle); **banding** depends on *how many steps* there are between two nearby colors, i.e. on:
1. **bit depth** (8 bit = 256 levels per channel; 10 bit = 1024);
2. aggressive **compression**, which flattens smooth gradients into blocks.

Two nearby oranges sit comfortably inside Rec.709; quantization is what turns them into a step. Remedies: a higher-bitrate or 10-bit source (UHD Blu-ray, HDR), and the banding reduction feature at minimum ([settings](../settings/settings-explained.md#picture-enhancements)).

## Gamut: how many colors

✅ Values commonly quoted as a percentage of the CIE 1931 xy diagram: Rec.709 ≈ 36 %, DCI-P3 ≈ 45 %, Rec.2020 ≈ 76 % ([V1 17:26](https://youtu.be/yN0H_WfWOp4?t=1046)).
⚠️ The video gives 53 % for P3: almost certainly the value in CIE 1976 u′v′ space (as reported, e.g., by the [DCI-P3 Wikipedia page](https://en.wikipedia.org/wiki/DCI-P3)), while for Rec.709 it uses the xy value. Mixing the two spaces skews the comparison. These percentages are only indicative anyway: area on a diagram does not weigh colors the way the eye perceives them.
❌ The video calls DCI-P3 "a compression standard": it is a **gamut** (a set of colors), not a codec.

✅ The bottle analogy is correct: a film mastered in P3 inside a Rec.2020 container does **not** hold more colors than P3 ([V1 24:34](https://youtu.be/yN0H_WfWOp4?t=1474)). ✅ Exception cited: the *Spider-Man: Into the Spider-Verse* UHD uses colors beyond P3 ([V1 25:07](https://youtu.be/yN0H_WfWOp4?t=1507)).

## In practice

1. For films you care about: **UHD Blu-ray** (or high-bitrate services) before 4K streaming.
2. Check whether a title's "4K" is a native DI or an upscale before deciding whether it is worth buying.
3. If you sit far from the screen, a 4K streaming plan mainly gets you **HDR and a higher bitrate**, not detail; decide whether you need it.
