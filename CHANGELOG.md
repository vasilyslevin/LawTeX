# LawTeX Changelog

## v3.0 (June 11, 2026)

2026 citation-currency update. The core citation engine is unchanged; this
release adds convenience macros and one validation guard, plus version stamps.

Added:

- `\contrast` for the Indigo Book R4.9 Contrast signal (Indigo Book 2.1 update, May 9, 2026), which juxtaposes factually or legally distinguishable authorities and always takes an explanatory parenthetical. Typesets the italicized signal.
- `\cleanedup` for the Indigo Book R8.2.7 `(cleaned up)` parenthetical (Indigo Book 2.1 update), which signals minor non-substantive mechanical adjustments to a quotation. First used by the Supreme Court in Brownback v. King, 141 S. Ct. 740, 748 (2021).
- `\para{n}` and `\pararange{a}{b}` for paragraph pinpoints (the form medium-neutral jurisdictions use), producing the paragraph mark followed by the number or range.
- `\citeFfourth{vol}{page}{court}{year}` for the Federal Reporter, Fourth Series (F.4th), which began publication in 2021 and is the live reporter for the United States courts of appeals.
- `\citeFappx{...}` retains Federal Appendix formatting but emits a package warning, because the Federal Appendix was discontinued in 2021.
- `\NCneutral{...}` guarded escape hatch that raises a package error: North Carolina rescinded its universal (medium-neutral) citation system effective February 1, 2023, so North Carolina cases should use traditional N.C. / N.C. App. / S.E.2d reporter form.

Documentation:

- New self-documented "2026 Updates" section in `bluebook.sty` (visible in the built `lawtex-doc.pdf`).
- Recorded the sixteen states that maintain an active official medium-neutral case designation as of 2026: Arkansas, Colorado, Illinois, Louisiana, Maine, Mississippi, Montana, New Mexico, North Dakota, Ohio, Oklahoma, South Dakota, Utah, Vermont, Wisconsin, and Wyoming.

Version stamps:

- `bluebook.sty` bumped to `2026/06/11 v3.0`.
- `lawbrief.cls`, `lawmemo.cls`, `arbitrationbrief.cls` stamped `v3.0`; `lawbrief.cls` now requires `bluebook` dated `2026/06/11` or later.

Compatibility:

- Fully backward compatible. Reporter abbreviations and case strings are still author-supplied literal text; existing documents compile unchanged.

Provenance:

- State practice and signal/parenthetical conventions verified against the Indigo Book 2.1 update (May 9, 2026) and The Bluebook, 22nd ed. (May 2025). The Indigo Book 2.1 update adds R4.9 (Contrast signal), R8.2.7 ((cleaned up) parenthetical), expanded R33.7 (social media), a corrected T3 entry for North Carolina, and a note on the discontinuation of F. App'x; the new `\contrast` and `\cleanedup` macros and the existing `\citeFappx`/`\NCneutral` guards track those changes. North Carolina rescission confirmed against the Supreme Court of North Carolina order rescinding its universal citation system (effective Feb. 1, 2023).
- The Indigo Book is published by Public.Resource.Org under a CC-0 public domain dedication.

## Prior history

- Original LawTeX by Christopher DeCoro (2009-2013), GPLv3. Mirrored from SourceForge. `bluebook.sty` previously stamped `2011/11/11`.
