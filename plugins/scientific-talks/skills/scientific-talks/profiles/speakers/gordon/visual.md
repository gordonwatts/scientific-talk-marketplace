# Gordon Watts: PowerPoint visual profile

Unless a template is supplied, use PowerPoint's plain built-in default template and layouts. Background and foreground settings come from the selected talk-type file or the talk's local style; resolve them locally if no setting is recorded. No custom binary template is required. Preserve native theme, master, layouts and placeholders, following [PowerPoint mechanics](../../../references/powerpoint.md). This file contains Gordon's reusable visual preferences across talk types.

## Shared theme settings

| Element | Default |
| --- | --- |
| Canvas | 16:9, 13 1/3 × 7 1/2 inches |
| Heading theme font | Calibri Light, normally 44 pt, regular |
| Body theme font | Calibri; master bullet levels 28/24/20/18 pt |
| Equation font | Cambria Math |
| Code font when needed | Consolas |
| Palette | Standard Office theme colors, subject to selected talk-type/local overrides |
| Primary emphasis | Office accent 2 orange, `#ED7D31` |
| Connections/caveats | Office blue, `#4472C4` |
| Hyperlinks | `#0563C1` |
| Additional diagram colors | Green `#70AD47`, yellow `#FFC000`, exceptional red `#FF0000` |
| Footer, every slide | `Gordon Watts (UW/Seattle)`, centered, 12 pt |
| Slide number, every slide | Automatic native field, bottom-right, 12 pt, continuous from 1 |

Configure these through PowerPoint theme/master styles. Newer Office defaults may use Aptos; set the selected fonts centrally rather than relying on per-object overrides. If a requested font is missing, report and resolve the substitution. Body text may use 20, 24 or 28 pt as content warrants; long headings may use 32–40 pt. Preserve clear hierarchy and consistency for corresponding slide roles. Avoid defaulting to automatic shrink.

Use orange on the important phrase or caveat rather than whole paragraphs. Supporting colors serve the diagram; do not force the entire palette onto a slide. Keep paper/plot screenshots' original white backgrounds where present. No decorative header bar, persistent sidebar or elaborate branding frame is needed. Institutional logos belong where relevant, not on every slide.

## Geometry and consistency

The source guide measured these approximate placeholder bounds; they are a useful reference, not mandatory glyph coordinates or a reason to replace native layouts:

| Element | Left | Top | Width | Height |
| --- | ---: | ---: | ---: | ---: |
| Title | 0.92 in | 0.40 in | 11.50 in | 1.45 in |
| Main content | 0.92 in | 2.00 in | 11.50 in | 4.76 in |
| Center footer | 4.42 in | 6.95 in | 4.50 in | 0.40 in |
| Slide number | 9.42 in | 6.95 in | 3.00 in | 0.40 in |

Reuse native layouts for related slides. Keep title placement, margins, font hierarchy and credit/footer positions stable so audiences can focus on the changing content. Adjust density and composition when the argument requires it, preserving the common visual grammar.

## Select a composition

- **Quiet question or section change:** sparse centered text and ample empty space. Use exceptional colored emphasis only when meaningful.
- **Roadmap:** repeat the same composition and emphasize the active item in orange; update completed items without redesigning the slide.
- **Evidence and interpretation:** dominant plot/table on the left half to two-thirds, compact commentary on the right.
- **Prompt and execution:** text/prompt beside an authentic code/log image, preserving exact evidence where needed.
- **Explanatory diagram:** large native shapes/connectors and short editable labels, with a visible main path.
- **Paper evidence:** relevant real figure, table, page or excerpt with editable commentary; credit using only the compact arXiv or DOI identifier as an active hyperlink near the evidence.
- **Overview and detail:** repeat or reversibly crop related imagery to maintain orientation.
- **Occasional conceptual artwork:** a selective metaphor with short editable thought; keep it secondary to evidence.

Authored titles, summaries, equations and explanatory labels stay in native PowerPoint objects. Source labels integral to plots can stay in their images. Never distort a picture to fill a box. Use built-in footer/number placeholders even on title/section/backup slides. Backup slides form a native **Backup** section at the end, with content-specific titles. Full citation details remain in the source index; identifiers link to arXiv abstract pages or DOI resolvers.
