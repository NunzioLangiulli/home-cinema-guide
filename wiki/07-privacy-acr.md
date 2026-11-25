# Privacy: ACR and smart TVs

> Main source: Slidebean, *yeah… this (hidden) chip pays for the whole TV* (V5, 2026-10-16), [video](https://youtu.be/t_GK06_3UY8). Not about picture quality, but it is part of the TV's initial setup and worth knowing before you accept the terms.

## In short

- Many smart TVs use **ACR (Automatic Content Recognition)**: they periodically compute a compact "fingerprint" of what is on screen and match it against a database.
- It works **with HDMI sources too** (set-top boxes, consoles, Blu-ray players).
- The data feeds advertising profiles combined with other sources (data brokers).
- You can turn it off in the menus; the most thorough option is to keep the TV offline and use an external box.

## How it works

✅ The Shazam analogy: the content itself is not sent, only a fingerprint of a few bytes, matched against a database ([V5 01:34](https://youtu.be/t_GK06_3UY8?t=94); [Wang's 2003 Shazam paper](https://www.ee.columbia.edu/~dpwe/papers/Wang03-shazam.pdf)).
⚠️ The *perceptual hashing* explanation (downsampling to 32×32 and 64 bits) is a **teaching example** of one possible technique ([V5 03:43](https://youtu.be/t_GK06_3UY8?t=223); [pHash](https://www.phash.org/docs/design.html)). Manufacturers' algorithms are not public.
✅ The traffic the video measured, about 1 KB per minute, is consistent with sending fingerprints rather than images.
✅ Samsung Ads' own document describes recognition at the "glass" level (what is on screen) regardless of source ([Samsung Ads ACR Guide](https://iabcanada.com/wp-content/uploads/2022/09/Samsung-Ads-ACR-Guide-CA.pdf)).
✅ Academic study (UCL and UC Davis, 2024): on Samsung and LG TVs, ACR sent data with antenna, HDMI and console input; **not** during screen mirroring, on the idle home screen, or in apps like Netflix/YouTube ([arXiv 2409.06203](https://arxiv.org/html/2409.06203v1)) ([V5 10:11](https://youtu.be/t_GK06_3UY8?t=611)).

## Who is behind it

- ✅ Zeev Neumeier, Cognitive Networks (later Inscape, acquired by Vizio) ([TVREV](https://www.tvrev.com/news/zeev-neumeier-inscape-vizio-tv-analytics-interview)).
- ✅ LG acquired Alphonso; Sony works with Samba TV; Samsung runs its own ACR; reference databases include Gracenote ([V5 08:03](https://youtu.be/t_GK06_3UY8?t=483)).
- ✅ The Vizio case: ProPublica (2015) revealed tracking on by default ([ProPublica](https://www.propublica.org/article/own-a-vizio-smart-tv-its-watching-you)); in 2017 Vizio paid **$2.2 million** to the FTC and New Jersey.

## Recent litigation (verified)

- ✅ **December 2025**: the Texas Attorney General sues Samsung, LG, Sony, Hisense and TCL over ACR.
- ✅ **February 2026**: settlement with Samsung (express consent for ACR data in Texas) ([Malwarebytes](https://www.malwarebytes.com/blog/news/2026/03/samsung-tvs-stop-spying-on-viewers-in-texas-heres-how-to-disable-acr-anywhere), [Texas AG release](https://www.texasattorneygeneral.gov/news/releases/attorney-general-paxton-secures-major-agreement-samsung-ensure-texans-are-protected-smart-tvs)).
- ✅ **May 2026**: settlement with LG (pop-up disclosure of data collection) ([Fox 7](https://www.fox7austin.com/news/lg-smart-tv-acr-data-collection-texas-settlement), [Texas AG release](https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-major-agreement-lg-protect-texans-privacy-and-stop-data-being)).
- ⚠️ The video says TCL had the case dismissed for lack of jurisdiction ([V5 17:16](https://youtu.be/t_GK06_3UY8?t=1036)). ❓ Not verified: May 2026 sources describe the Sony, Hisense and TCL cases as still open.
- ❓ LG's forced arbitration clause in the US: reported by [Decrypt](https://decrypt.co/377637/lg-tv-might-be-listening-even-when-off); not checked against the terms themselves.
- ⚠️ Gamers Nexus's findings on LG TVs (voice transcripts, local network scanning) ([GN video](https://www.youtube.com/watch?v=6IFVTcM28KA)) are important investigative work; read the original to understand the conditions under which they were obtained.

> **Note for readers in Europe.** The legal framework is different: the GDPR and the ePrivacy Directive generally require informed consent for this kind of processing. The cases above are American; we have not checked how each manufacturer handles ACR on European models.

## The business model

- ✅ Roku (2025 10-K): the devices segment loses money; the platform (ads and services) generates the profit ([V5 20:02](https://youtu.be/t_GK06_3UY8?t=1202), [10-K](https://image.roku.com/bWFya2V0aW5n/Roku-2025-Form10-K.pdf)).
- ✅ Fox announced its acquisition of Roku on 15 June 2026 (~$22 billion), citing direct relationships with over 100 million streaming households ([Fox Business](https://foxbusiness.com/markets/fox-corporation-announces-22b-acquisition-roku-landmark-streaming-live-tv-deal)).
- ⚠️ The estimate of LG's advertising margins ([V5 21:41](https://youtu.be/t_GK06_3UY8?t=1301)) is the video's inference ("even if it were 50 %…"), not published data.

## CleanYourTV: the community project to follow

[**CleanYourTV**](https://cleanyour.tv/) ([GitHub repository](https://github.com/Gathin23/cleanyourtv), MIT licence) is the most complete, continuously updated public resource on taking back control of a smart TV. Started in October 2026, it is updated almost daily by contributors; at the end of November 2026 it lists tested configurations for 513 TV models from 139 brands. Check it rather than relying on the menu paths in this guide, which date quickly.

It offers two paths:

| Your TV | What CleanYourTV offers |
|---|---|
| **Samsung (Tizen), LG (webOS), Roku, Vizio, Hisense VIDAA, Fire TV** | [Non-Android guide](https://cleanyour.tv/not-android): step-by-step switches with the remote, no install, every step undoable. Three levels: (1) TV settings, (2) a guest network so the TV can't see your other devices, (3) DNS blocking. It also has an online check of whether your network's DNS blocks known TV tracking domains. |
| **Android TV / Google TV** (Sony, Philips, TCL, Xiaomi, Hisense Google TV…) | A debloat over Wi-Fi via the Android debug bridge (ADB): manufacturer telemetry, ad services and preloaded apps are *disabled* (`pm disable-user`), not uninstalled; a clean launcher replaces the ad-filled home screen; a one-line restore puts everything back. Per-model lists are in the repository's `examples/` folder. |

Assessment:
- ✅ Open source and auditable, reversible by design, explicit about what it cannot do (no ADB on Tizen/webOS/Roku, so settings only there), and it warns against rooting. Its claims are sourced (e.g. the Gamers Nexus finding of an LG TV listing 38 devices on a home network, and the NSA's advice to keep guest devices on a separate network).
- ⚠️ The Android path asks you to enable developer options and USB/network debugging and, in its quick start, to let an AI coding assistant run commands against the TV on your network. Read [`PROMPT.md`](https://github.com/Gathin23/cleanyourtv/blob/main/PROMPT.md) and the scripts before running them, keep the backup it writes, and switch debugging off afterwards.
- ⚠️ Firmware updates bring the disabled packages back; the project provides a check-and-fix script, so it is an ongoing task, not a one-off.
- ⚠️ Effects on warranty and on manufacturer features (voice assistant, casting, updates) depend on what you disable; the tool asks before touching apps you might use.
- ⚠️ The project warns that look-alike domains (e.g. cleanyourtv.com, clean-your-tv.net) and app-store apps are **not** its own; use only cleanyour.tv and the GitHub repository.

## What to do

1. **Follow CleanYourTV's guide for your TV** ([non-Android](https://cleanyour.tv/not-android), or the [Android TV / Google TV path](https://github.com/Gathin23/cleanyourtv#quick-start)).
2. **Turn off ACR** and personalized advertising: paths in [names-by-brand.md](../settings/names-by-brand.md#privacy-content-recognition-acr). During first setup, accept only the **mandatory** terms.
3. **Microphone**: disable it if you don't use voice control.
4. **Network**: isolate the TV (guest network/VLAN; DNS blocking as a further step) or **don't connect it** at all and use an external box (Apple TV, Shield, etc.), which has its own data policies.
5. After every firmware update, **check the settings again**: paths and consents can change.
