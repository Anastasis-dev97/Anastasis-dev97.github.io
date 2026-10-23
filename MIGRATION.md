# Content migration notes

Source pages:

- https://anastasis-dev97.github.io/index.html
- https://anastasis-dev97.github.io/research.html

The conversion retains four education entries, six talks, seven conference/workshop entries, two teaching entries, seminar organization, and the single work in preparation. The homepage gives a short overview; full thesis titles are available on the research and CV pages.

## Editorial decisions

- The paper *The Lie algebra of contact vector fields is centrally closed* remains explicitly **in preparation**. No journal, publication date, DOI, arXiv identifier, or download has been invented.
- The photograph is the original `DSCF4467.jpg`, resized proportionally and encoded as WebP for faster delivery. Its complete composition is preserved.
- The contact email remains `familyname @ math dot univ-lyon1 dot fr`.
- The conference *Who is afraid of infinite dimensions?* is listed in **October 2025**. The original website placed it under 2026, but its linked official page gives 27–31 October 2025: https://www.ryvkin.eu/conferences/hs2025/. The migration uses the month rather than extending the user's stated attendance range.
- The user's listed participation dates for the Vienna programme are preserved; they are not replaced with the full programme dates.
- Spelling, punctuation, and list markup were cleaned up without adding qualifications, publications, or affiliations.

## Verification

- Built successfully with Jekyll 4.4.1 and the pinned al-folio runtime.
- Checked internal page and asset references in the generated output.
- Checked that all original content categories and entry counts were retained.
- Checked desktop rendering, page navigation, site search, and theme switching in a browser.
- Checked phone-width layout and menu navigation at a 390 px frame width; no horizontal overflow.
- The original static website is preserved on branch `backup-before-al-folio-2026-10-23` at commit `b849062ada772c0c9850058615cd632dd08160df`. This branch was created before publishing the conversion.
- The GitHub repository copy omits private-preview configuration, screenshots, source archives, and hosting metadata.
- GitHub Pages must use the GitHub Actions source for the included deployment workflow.
