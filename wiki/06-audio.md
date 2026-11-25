# Audio: from Dolby Stereo to Atmos

> Main source: Slidebean, *The brilliant scam of "Dolby Atmos"* (V6, 2026-09-11), [video](https://youtu.be/SNwoI6531us).

## In short

- **Channel-based audio** (2.0, 5.1, 7.1): each track goes to a specific speaker.
- **Object-based audio** (Dolby Atmos, DTS:X): sounds have a 3D position and the decoder "renders" them to the speakers you have.
- In **streaming**, Atmos is compressed (Dolby Digital Plus, up to ~768 kbps); on **disc** it is lossless (Dolby TrueHD).
- Without **height** speakers (in-ceiling, upfiring, or a good soundbar), Atmos reduces to traditional surround.
- Hard-to-hear dialogue has several causes; Atmos is at most one of them.

## From channels to objects

✅ **Cinerama** (1952) already had multichannel audio on separate magnetic film (7 tracks) ([V6 02:14](https://youtu.be/SNwoI6531us?t=134)).
✅ **5.1** = left, center, right, two surrounds + subwoofer (the ".1" band-limited LFE channel). The center carries almost all dialogue ([V6 02:48](https://youtu.be/SNwoI6531us?t=168)).
✅ Surround placement in 5.1: about **110–120°** from the listener ([V6 03:54](https://youtu.be/SNwoI6531us?t=234)). Reference: ITU-R BS.775 (100–120°) and the [Dolby speaker setup guides](https://www.dolby.com/about/support/guide/speaker-setup-guides/).
✅ **Atmos**: in cinemas up to **128 elements** (bed + objects) and up to 64 outputs; the mix describes positions in space and the processor maps them to the actual speakers ([V6 05:33](https://youtu.be/SNwoI6531us?t=333)).

⚠️ V6 attributes room adaptation to the receiver's calibration microphone ([V6 06:06](https://youtu.be/SNwoI6531us?t=366)). These are two separate things:
1. the **Atmos renderer** uses the **speaker layout** you declare (e.g. 5.1.2, 7.1.4);
2. **microphone calibration** (Audyssey, Dirac, YPAO, Room EQ) measures distances, levels and the room's frequency response. It works without Atmos too.

✅ Headphones with spatial audio (AirPods etc.) use the object/channel nature of the mix for binaural rendering with head tracking ([V6 06:40](https://youtu.be/SNwoI6531us?t=400)).

## A history of compression: Dolby vs DTS

| Format | Year | Channels | Bitrate | Notes |
|---|---|---|---|---|
| Dolby (A-type noise reduction) | 1971 (*A Clockwork Orange*) | — | analog | Reduced hiss |
| Dolby Stereo (matrix) | 1975–77 (*Star Wars*) | 4 (L, C, R, S) in 2 optical tracks | analog | Phase-based matrix encoding ✅ |
| Dolby Digital (AC-3) | 1992 (*Batman Returns*) | 5.1 | 320 kbps in cinemas; 384–448 kbps on DVD | Digital blocks between the perforations ✅ |
| DTS (cinema) | 1993 (*Jurassic Park*) | 5.1 | ~882 kbps | Audio on CD-ROM synced by timecode ✅ |
| SDDS (Sony) | 1993 | 7.1 | — | Discontinued in the 2000s ✅ |
| DTS on DVD | 1990s–2000s | 5.1 | 754 or 1509 kbps | ✅ |
| Dolby TrueHD / DTS-HD MA | 2006+ (Blu-ray) | up to 7.1 + objects | lossless; max ~18 / ~24.5 Mbps | ✅ |
| Dolby Atmos in DD+ (JOC) | streaming | objects | 448–768 kbps (Netflix) | ✅ ([What Hi-Fi](https://www.whathifi.com/news/netflix-brings-high-quality-audio-to-51-and-atmos-content)) |
| Linear PCM | cinema DCP | one channel per speaker | uncompressed | Atmos in cinemas via IAB ✅ |

✅ **Matrix encoding**: a correct, clear explanation. The center is the in-phase signal between L and R, the surround the out-of-phase one ([V6 17:04](https://youtu.be/SNwoI6531us?t=1024)). Home "Dolby Pro Logic" applies the same principle.
⚠️ "You need at least 1400 kbps for lossless audio" ([V6 20:21](https://youtu.be/SNwoI6531us?t=1221)): 1411 kbps is the CD's **uncompressed** bitrate. A lossless codec (FLAC, TrueHD, DTS-HD MA) reduces data without loss, often to half or less.
⚠️ "TrueHD wasn't backward compatible, DTS-HD MA was" ([V6 26:23](https://youtu.be/SNwoI6531us?t=1583)): DTS-HD MA contains a lossy DTS "core"; TrueHD streams on Blu-ray are also generally accompanied by a compatible Dolby Digital track ❓ (to be checked against the BD specification). The video's commercial point (DTS-HD MA widespread on early Blu-rays) is plausible.
💬 "DTS sounds punchier": often it is simply **louder** (some DTS streams don't apply dialogue normalization the way Dolby does). At matched volume the differences are much smaller. The video's own test (*Shaun of the Dead*, English Atmos vs German DTS:X, [V6 36:52](https://youtu.be/SNwoI6531us?t=2212)) concludes it can't hear a difference.

## Streaming vs disc

✅ Streaming Atmos = DD+ with JOC, ~768 kbps at most; UHD Blu-ray Atmos = lossless TrueHD ([V6 30:13](https://youtu.be/SNwoI6531us?t=1813)).
✅ Netflix calls 640 kbps "perceptually transparent" for 5.1 ([Netflix via What Hi-Fi](https://www.whathifi.com/news/netflix-brings-high-quality-audio-to-51-and-atmos-content)). 💬 The "night and day" *Blade Runner 2049* disc-vs-streaming comparison in the video is a sighted listening test, and the disc may also have a different mix and dynamics.
✅ DTS:X streaming exists on Disney+ (IMAX Enhanced), only with compatible devices ([V6 30:44](https://youtu.be/SNwoI6531us?t=1844)).
✅ Apple TV decodes TrueHD/DTS-HD from local files to **multichannel PCM**: lossless, but the Atmos object metadata is lost ([V6 31:17](https://youtu.be/SNwoI6531us?t=1877)).

## Atmos in practice

Options for height channels, from least to most effective ([V6 33:00](https://youtu.be/SNwoI6531us?t=1980)):
1. **Atmos soundbar** with upfiring drivers: depends on the ceiling (flat, reflective, not too high). 💬 "Fatmos" is the video's verdict; the best soundbars still give a perceptible height effect.
2. **"Atmos enabled" modules** on top of the front/surround speakers, firing at the ceiling.
3. **In-ceiling** or high wall speakers: the reference solution (5.1.2, 5.1.4, 7.1.4).

Key figures from the [Dolby Atmos Home Theater Installation Guidelines](https://displaydaily.com/wp-content/uploads/2014/10/dolby-atmos-home-theater-installation-guidelines.pdf) (Dec 2018, read in full):

| Item | Dolby guideline |
|---|---|
| Ear-level speakers | Same height, ~1.2 m (seated ear height, per ITU-R BS.775-3 / BS.1116); rears no higher than 1.25× the fronts |
| Front L/R | 22–30° from center |
| Surrounds | 5.1: 110–120°; 7.1: side surrounds 90–110°, rears 135–150° |
| Overhead (top front/rear) | 45° elevation, acceptable 30–55°; mounted at 2–3× ear height; about as far apart as the front L/R |
| Upfiring ("Atmos enabled") | At or slightly above ear height, never above half the wall; flat, reflective ceiling 2.3–4.3 m (ideal 2.3–3.66 m); at least 0.9 m (ideally 1.5 m) from listeners |
| Levels | Each speaker 79–82 dB SPL (C-weighted) at the main seat with −20 dBFS pink noise; check auto-calibration results for the subwoofer and upfiring speakers |
| Source | Bitstream output; secondary audio mixing off on Blu-ray players |
| Avoid | Dipole surrounds; putting all speakers in the ceiling |

⚠️ Written by the format owner: its claim that upfiring speakers can be "preferable" to ceiling speakers is promotional. More layouts: [Dolby guides](https://www.dolby.com/about/support/guide/speaker-setup-guides/).

## Why dialogue is hard to understand

The video blames "everything getting an Atmos mix" ([V6 34:39](https://youtu.be/SNwoI6531us?t=2079)). ⚠️ This is a simplification. More significant documented causes:
1. **Cinematic dynamic range**: relatively quiet dialogue, very loud explosions. Designed for cinemas with powerful systems.
2. **Downmixing** 5.1/Atmos to 2.0 on TVs: the center (dialogue) gets mixed with the other channels.
3. **TV speakers**: small, often facing down or backwards.
4. **Mixing and acting** choices (more naturalistic, whispered dialogue) and streaming services' loudness targets.

Practical fixes:
- Receiver: **center channel +2/+3 dB**.
- TV/soundbar: **dialogue enhancement / clear voice**.
- **Night mode / DRC** (dynamic range compression).
- A soundbar or speakers with a real center channel almost always beat TV speakers.

## Practical settings

| Situation | TV setting | Source setting |
|---|---|---|
| Soundbar/receiver over HDMI | Output: HDMI eARC; format: **Passthrough/Bitstream/Auto** | Audio: Auto / Dolby Digital Plus / Bitstream |
| TrueHD/DTS-HD from a player | Player connected directly to the receiver, or a TV with **eARC** (ARC is not enough for lossless) | Bitstream |
| TV speakers only | Dialogue enhancement; DRC/night if needed | PCM/Auto |
| Lip-sync off | Audio delay on TV or receiver | — |
