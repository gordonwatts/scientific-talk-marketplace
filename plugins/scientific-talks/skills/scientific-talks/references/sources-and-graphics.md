# Sources and graphics

## Ground the claim first

Start with the slide's claim and the evidence needed to support it. Prefer original papers, collaboration releases, original data/plots and supplied source material. Read the relevant passage/caption, not just a search result. Verify current or uncertain claims with primary sources. Preserve the difference between an author's claim, actual measured evidence, the speaker's interpretation and an LLM's unvalidated output.

Assign a stable source ID such as `P001` or `R001` in `references/index.md`. Record title/authors, arXiv or DOI where available, exact revision/date, source URL, downloaded PDF/HTML path, useful extract, page/section/figure, and consuming slide IDs. Non-paper sources can have an organization, date and URL rather than an invented identifier. Keep each downloaded revision distinct. If a source cannot be obtained, record that limitation; do not claim a local file exists.

Extract only useful passages or captions into `references/extracts/`, with their precise source locations. Do not treat an extracted snippet as sufficient for a question requiring broader paper context. Slides and source indexes point to the same revision. Historical screenshots or supplied benchmark output remain dated snapshots unless new evidence replaces them explicitly.

## Obtain and prepare visuals

Prefer original figure files when available. Download papers to `references/papers/` and original figures to `assets/originals/`. A PDF-page rendering is acceptable when no suitable original figure is accessible. Keep cropped/converted variants in `assets/ready/` and preserve the originals.

In `assets/index.md`, record a stable asset ID, original and ready paths, source ID and exact URL/page/figure, caption and interpretation, attribution/license if known, processing steps, consuming slide IDs, and readiness. Index originals even if no derived file is necessary. The usable file may be an original in that case; do not duplicate it merely to fill both folders.

Inspect visuals before using them. Keep axes, units, legends, panel labels and relevant evidence. Scale uniformly; crop only where scientific interpretation remains intact. Explain ambiguous colors, counts, units or model labels from the source rather than guessing. Label a reproduced result, an adapted diagram, or a generated illustration appropriately. Do not silently correct recorded experimental or model output.

For native diagrams, record their specification in the slide outline rather than inventing an image path. Reuse related diagrams and visuals when continuity serves the argument. A composite diagram from a source deck may contain native shapes; extracting one embedded picture does not reproduce the whole diagram.

For generated artwork, request components, not entire slide images. Specify desired placement/aspect ratio and no headline, slide title, takeaway or summary inside the image. Object labels integral to understanding the artwork may remain; author editable slide-specific labels and equations in PowerPoint. Generated artwork is conceptual illustration, not scientific evidence. Use an available image-generation capability only when needed; this plugin requires no particular external service.

## Credit and review

Apply the selected speaker's citation convention. Gordon uses compact native editable arXiv/DOI hyperlinks near the evidence, while the full bibliography and revision details remain in the source index. Use source/credit text for non-paper assets as appropriate and preserve any required attribution.

For each slide review the selected graphic, what it actually demonstrates, readability at presentation size, source/revision, and caveats. Prefer separate slides or progressive reveals to shrinking important evidence. Record unresolved acquisition, attribution or interpretation questions before building.
