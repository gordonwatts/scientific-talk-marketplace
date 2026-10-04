# Origins and extraction decisions

Prepared 4 October 2026 from the Davis talk workspace. This record documents origins; none of the original files is required to use the plugin.

| Original material | Reusable destination | Treatment |
| --- | --- | --- |
| `generic-instructions.md` | Colloquium style file | Department-wide audience, first-year graduate accessibility, motivation and broader conclusion |
| `slide-style.md`: voice, text density, narrative | Gordon content profile | Speaker voice and useful composition decisions; removed historical slide numbers and scientific example claims |
| `slide-style.md`: visual foundation and compositions | Colloquium style file and Gordon visual profile | Colloquium-specific background/foreground configuration in the talk-type file; reusable palette, typography, geometry, compact credits and compositions in speaker guidance |
| `slide-style.md`: generation/editing instructions | Shared PowerPoint mechanics and graphics reference | Native objects, equation mode, aspect ratio, text-box behavior, automatic numbers, backup section, rendered review |
| Existing section outlines and asset provenance records | Outline/source/asset starter fields and lookup workflow | Separate visible content, notes, takeaway, evidence and local graphic; stable IDs replace dependence on current slide numbers |
| Existing build/revision records | Assembly and verification guidance | Preserve themes/designs and inspect numbers/images/links; temporary repair code is not packaged or prescribed |
| Speaker's instructions in this conversation | Workflow and packaging | Three reviewed outline passes, plugin-only implementation, guide-only template, native PowerPoint priority and audience consistency |

The original guide refers to `2026-08-13 - Agents and the future of HEP Analysis.pptx`. No source deck was bundled. Its scientific content, anecdotes, historical costs/rankings, exceptional cover art and particular slide numbers are not universal requirements. Figure-specific training/dimuon instructions were generalized to preserving source labels, reversible cropping, editable annotations and truthful benchmark attribution.

Source hashes at extraction (SHA-256):

```text
slide-style.md
4B1C7CF8EA70804F47464FEBCCA38A31EFBC8910A29948D3AFE2A2E7DD2108A5
generic-instructions.md
34050C8D321D8AFEA9D547E324B84A41668E011DD87DBFF107BBD4CCCC39FD25
```

Packaging follows [official OpenAI plugin/marketplace documentation](https://developers.openai.com/plugins/build/plugins), checked on 4 October 2026. The package is skills-only, with root `plugin.json` inside the plugin and a separate repository-root `.agents/plugins/marketplace.json`. Catalog paths are relative to the marketplace root. Installation is a separate user-controlled step; this source package does not modify user configuration or install itself.
