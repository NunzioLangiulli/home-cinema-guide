# Contributing

The aim of this project is **accurate, verifiable** information. Every contribution should follow three rules.

## 1. Every claim has a source

- Prefer, in this order: **standards** (ITU, SMPTE, CIE, EBU) → **official documents** (UHD Alliance, Dolby, manufacturers) → **independent measurements** (RTINGS, HDTVTest, magazines with labs) → **popular explainers**.
- For videos, give the **timestamp** as a direct link: `https://youtu.be/ID?t=SECONDS`.
- If you cannot find a source, you may still add the information with the ❓ label and explain what is missing.
- When you add a new source, add it to the [bibliography](sources/bibliography.md) with a short **assessment** answering the five questions at the top of that page (type, independence, method, date and scope, what you actually read). The same critical standard applies to every source: standards, manufacturers, magazines and videos alike.

## 2. Use the labels

✅ verified · ⚠️ simplified · ❌ incorrect · ❓ unverified · 💬 opinion ([meaning](README.md#how-to-read-the-reliability-labels)).
When you correct a claim made in a video, **don't delete it**: keep it with ❌ and the correct version next to it. The comparison is part of what makes the guide useful.

## 3. Keep facts and preferences apart

"D65 is the reference white" is a fact. "I like a bit of sharpening" is a preference: it is fine to write it, with 💬.

## Most useful contributions

1. **Menu names by brand/model/year** ([names-by-brand.md](settings/names-by-brand.md)): with exact model, year, firmware and, if possible, a photo of the menu.
2. **Before/after results** with a phone calibration app, ideally cross-checked with a colorimeter if you have access to one.
3. **Corrections** to anything marked ❓.
4. **Updates** when new videos in the series or new documents appear (e.g. the Filmmaker Mode specification, or the TV Calibrator app's source code once published).

## Structure

```
README.md                 index and principles
QUICK-START.md            what to do, in order
settings/                 every setting explained + names by brand
wiki/                     concepts (one page per topic)
sources/                  bibliography, with an assessment of every source
.github/workflows/        automatic link check
```

## Automatic checks

A GitHub Action ([link-check.yml](.github/workflows/link-check.yml)) periodically checks that links still work. If a link dies, replace it with an archived copy ([Wayback Machine](https://web.archive.org/)) instead of removing the source.

## Style

- Plain English; explain technical terms on first use or link them to the [glossary](wiki/00-glossary.md).
- Short sentences, one idea per paragraph. Tables for comparisons.
- Numbers with their unit and their source.
