# How this repository was made (Solothurn (city))

This file is written by the build on 2026-11-02, the day the source data was retrieved.

## Sources

| Source | Address | Retrieved | Licence |
| --- | --- | --- | --- |
| Stadt Solothurn: SRS (LexWork) | <https://reglemente.stadt-solothurn.ch/> | 2026-11-02 | Laws and decrees are not protected by copyright (Art. 5 para. 1 let. a URG, SR 231.1). |

Every word of law in this repository comes from these sources. Lexifina reads them and records each act's dated versions, and the laws that made each change, in one corpus file. This repository is built from that file.

## What is in it

| Act | Title | Versions | Span |
| --- | --- | ---: | --- |
| `1-1-1` | Gemeindeordnung der Einwohnergemeinde der Stadt Solothurn | 1 | 2026-01-01 to 2026-01-01 |

The build made 1 commits:

| Commits | Kind |
| ---: | --- |
| 1 | first version of an act |
| 0 | one law on its in-force day |
| 0 | changes no amendment note explains, credited to the publisher |

Other counts:
- 0 commits on the branch `zukunft`: laws not yet in force on 2026-11-02.
- 0 commits dated 1 January 1970: in force before 1970, with the real day in their `In-force` trailer.
- 1 laws in the record.
- 2 tags.

## Dates

Each commit is dated at noon (Europe/Zurich) on the day the change took effect. The other dates, enacted and published, are trailers.

When a law gives no date of its own, the default rule applies: Each version is dated by the day the city's systematic collection says it took effect ("in Kraft seit / von"); municipal acts take effect on the day the act or the city sets. https://reglemente.stadt-solothurn.ch/

## How the history is built

`tools/build.py` turns the corpus into this history in one pass: one commit per law, on the day it took effect. The same corpus always gives the same commit hashes. `tools/check_repo.py` reads every version back from git and compares it with the corpus. `tools/on.py` shows the law as it stood on any date. The corpus format is described in `tools/SCHEMA.md`.

- Corpus: sha256 `1cbc4cf57c76cf03932f7618330c192c72382072341c97164ecb88cb877ad5bb` (43802 bytes).
- Builder blob hashes (`git hash-object`): `build.py` `a4faa25af85facb64b956b372f6b528aafdd7ec1`, `check.py` `3d00541d258745461ab52b1b0cb4e1716a27a95d`, `on.py` `644a6c0857fbcc72562032b58d57aa113fee0641`.
- Python 3.12.10; git version 2.46.0.windows.1.

## Checks

1 versions of 1 acts read back from git on the day each took effect and on the day before: 0 mismatches. Trailers: 0 commits whose trailers git cannot parse. Health: 0 merge commits on main, 0 commit dates that go backwards, 0 commits dated after the build.

No second build of this corpus has been compared yet.

## Decisions made by hand

- Each version is the consolidated text the city's systematic collection publishes, dated by its "in force from" day; when two versions share a day only the last is kept.
- Changes are credited to the entries of the act's own change table (decision, in-force day, element, CRS reference) whose in-force day falls after the previous version and on or before this one; a change whose element the table does not name is credited to every entry of that window.
- Section headings are kept together in one file per act (gliederung.md); the title, date and preamble in ingress.md; the signature block in schluss.md. Amendment markers (*) and the "Stand" date are left out.
- Annexes published only as separate PDF files are not included.
- An act's first version is credited to its original enactment only when the change table shows no change in force before it; otherwise it is the oldest version available.

## What AI did and did not do

The scripts that read the sources and build this repository were written by Claude Code running Claude Opus 5.5 (`claude-opus-5-5`) under Lexifina's direction.

No model wrote, translated or corrected legal text. No model runs at build time. Every word of law in this repository comes from the official sources above.

The commit messages are written by `build.py` from the source data.

Model use at data-build time:
- A model (Claude) wrote the fetch and parse code and chose which acts to include; it wrote no law text. Every word of law comes from the city's own collection.
