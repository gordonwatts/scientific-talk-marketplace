# Native PowerPoint construction and verification

## Start with native structure

PowerPoint is the primary authoring/editing application. Use an available supported control path, such as native application automation on Windows or connected PowerPoint controls. Choose the available path without hardcoding runtime locations into the skill. Supporting tools can prepare assets or inspect the package. Do not replace native PowerPoint construction with full-slide raster images or flatten editable content.

If PowerPoint access is unavailable, continue outlining/sourcing and state what cannot yet be built or verified. Do not silently switch applications and claim native PowerPoint completion. If another application is explicitly requested, follow that request and document any differences in native behavior or verification.

A supplied template takes precedence. Otherwise create a presentation from PowerPoint's plain built-in default template and layouts. Keep its theme, slide master, layout definitions and title/body/footer placeholders. Apply the selected profiles' background, palette, typography, canvas and footer settings centrally. Talk-type-specific settings live in the selected talk-type file; do not load another talk type to obtain them. Do not bundle or require a custom binary template.

Use stock Title Slide, Title and Content, Two Content and other appropriate native layouts. For common slide patterns, reuse the same layout and corresponding object placements; extend a native layout when a recurring need warrants it. Apply shared changes at master/layout/theme level rather than restyling each slide independently. Related slides should preserve title position, margins, typography, emphasis conventions and citation/footer placement. Variation should communicate a change in purpose, not force the audience to relearn the canvas. Do not rebuild the master when only one slide needs a local change.

## Editable slide content

- Titles use title placeholders. Put body text, captions, takeaways and figure-specific commentary in editable native objects. Use native bullet levels and spacing.
- Use native equation mode (Office Math/OMML) for authored mathematics, with proper structure. Ordinary Unicode symbols are fine for simple labels; screenshots or hand-positioned superscripts are not substitutes for equations. Preserve borrowed mathematical labels inside original figures.
- Use native shapes/connectors for simple explanatory diagrams and progressive reveals. Keep required data charts/tables editable where underlying data are available; original paper figures remain valid evidence images.
- Normally set custom text boxes to **Resize shape to fit text**, with intended width and suitable margins. Keep intentional title/layout placeholders and fixed design boxes where required. Check that growing text remains in the slide's usable area. Do not use automatic text shrink as the default cure for excess content.
- Set paragraph alignment and vertical alignment explicitly. Center the object as well as the text; do not use spaces or incidental line breaks to simulate centering.
- If text needs a border, apply the line/fill to the same text box so they resize together. Use PowerPoint alignment/distribution and native connectors to preserve relationships when edited.
- Inspect existing embedded labels before adding overlays. Reversible PowerPoint cropping can remove an unwanted heading strip while native text replaces it; do not obscure required plot labels. Uniformly scale images and compare displayed proportions with originals.

## References, footer, numbers and backup

For Gordon's profile, render paper identifiers as compact editable hyperlink text near the relevant evidence. Link arXiv identifiers to the matching abstract page (`https://arxiv.org/abs/<identifier>` including the revision when relevant) and DOI identifiers to `https://doi.org/<identifier>`. Keep full bibliographic details in the source index. Do not use a paper's full title merely as credit. For other profiles, follow their attribution choices while retaining evidence access.

Enable PowerPoint's native footer and slide-number placeholders through Header and Footer, applied to all slides, including title, section and backup slides. Gordon's footer is `Gordon Watts (UW/Seattle)`, centered, 12 pt; the slide number is bottom-right, 12 pt. Turn off title-slide suppression where needed. Use an automatic `slidenum` field, never a typed number in an ordinary box. Number continuously from 1 in the complete deck. If sections are combined, verify fields, themes and designs after insertion rather than preserving section-local numbers.

Place backup slides after all main-talk slides in a native PowerPoint section named **Backup**. A divider slide alone does not create that section. Give backup slides descriptive content titles without adding "backup" to each one. Preserve any requested hidden/show behavior; backup placement does not imply slides should be hidden.

## Build and verify

Create chapter drafts for review and keep speaker notes with the slides. When assembling sections, preserve their native layouts, theme bindings, notes, equations, links and image proportions. Update stable-ID mapping in `STATE.md`. Save the editable deck at the recorded `deck/` path and exports at recorded `output/` paths. Keep intermediate experiments in `tmp/`.

Open and inspect the result in PowerPoint, export rendered slides, and inspect those images at full-slide scale and, where needed, readable detail. Check coverage, titles, notes, background, hierarchy, consistent placement, citations, image proportions, legible labels, text fit and unintended overlap. Check sparse transitions as well as evidence slides.

Verify native behavior in a disposable copy of the completed deck: edit representative title/body text, change a shared layout/style and confirm dependent slides follow, inspect an equation and connector, and insert/reorder/delete a slide to confirm automatic numbering follows its position. Do not run these destructive checks on the speaker's current deck. Discard the test copy or identify it as disposable.

Structural/package inspection may supplement these checks; passing it does not prove scientific correctness, rendering or editability. Record the actual renderer/application, review scope, issues fixed and remaining limitations in `STATE.md`. Say "checked in PowerPoint" only after doing so. A deck awaiting native checks remains a draft, even if other checks pass.
