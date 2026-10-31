# Licence draft: not in effect

This folder holds a draft of a permissive licence and the reasons it cannot yet
replace the repository's licence. Nothing here changes `LICENSE`, `LICENSING.md`
or any file header. The repo stays GPL-3.0-only.

## Chosen path: A, MIT on files Hung alone holds

MIT (`MIT.txt` here) is the licence for the files Hung alone holds copyright to. It
keeps the copyright notice with copies, so anyone who reuses the code credits the author.
The rest of the repo stays GPL-3.0-only.

Open items before this is final:
- **Copyright holder name.** `MIT.txt` has a placeholder. The name must come from Hung.
- **Which files qualify.** Git authorship is not the same as copyright. A file qualifies only
  if no one else's code is in it. See the list below.
- **File headers.** A file moved to MIT needs its `SPDX-License-Identifier` header changed.
  That change is not made yet.

## Candidate files (git history by Hung only, no other copyright line)

These have no Felucca or JIANT copyright line in their header. Hung still needs to confirm
they are not built on other people's code:
- `docs/BUILD-SHRUB.md`
- `docs/GUI-REVAMP-GARDEN.md`
- `docs/STEMS-10-BUILD.md`
- `docs/gui-garden-mockup.html`
- `tools/glitch_watch.py` (its header has the GPL SPDX line but no copyright line)

## Not candidates (GPL-3.0-only headers name other copyright holders)

Git history shows only Hung's commits, but these headers credit Leo Kuroshita and/or
Juan Ignacio Antonucci. Hung cannot relicense them alone, so they stay GPL-3.0-only:
- `firmware/src/eng_shrub.c`, `firmware/src/ui_goobers.c` (both credit Leo and Juan)
- `firmware/src/shrub_tables.c`, `tests/shrub_test.c`, `tools/gen_shrub_waves.py` (credit Leo)
- `tests/tracks8_test.c` (Leo, with Juan's "Portions" line)

## Third-party parts that stay under their own licences

Unchanged by this draft; see LICENSING.md: msfa (Apache-2.0), Fukiai and fm1-clk320 (MIT),
CMU dictionary (BSD-2-Clause), the OFL fonts, and the JieLi SDK files shipped only in packages.

## Other paths, not chosen

- **B. Relicense the whole repo.** Needs written consent from Leo Kuroshita, Juan Antonucci,
  charlesvestal (`web/emu/`) and illuminus5 (Skiff), and possibly a rewrite of the GPL parts.
- **C. Keep GPL-3.0-only.** The current state.

## Before publishing

Get the copyright name, confirm the candidate list, change the headers of the confirmed files,
add the MIT text at the top of each (or a LICENSE-MIT file), and update the README "License"
section. Repo visibility is not changed by any of this.
