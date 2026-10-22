# Focused revision and source-grounded answers

Read `TALK.md` and `STATE.md`, then the requested slide/chapter, its sources and the relevant style/mechanics guidance. Inspect the current deck's actual objects, notes, equations, figures and links. Resolve references such as "the EveNet slide" by content and stable-ID mapping; if several matches remain, clarify before editing the wrong one.

For a factual question, trace the relevant claim through `references/index.md` to the precise paper revision and page/figure. Use the graphic's asset record for visual interpretation. Answer with the evidence and its caveat; do not manufacture certainty or assume an old slide accurately reports a later paper. If external lookup is needed, prefer primary sources and distinguish newly obtained evidence from what the deck currently says.

An explanatory question is not automatically a slide-edit request. For a question-only turn, answer without changing the deck unless the user also requests an edit. If the user asks to keep the explanation for their own reference, place it in notes.

For edits, preserve the existing deck as the authority for manual text and layout changes. Compare it with the outline; reconcile affected entries rather than rebuilding from a stale outline. Work on the designated deck or a clearly identified revision copy, as the user's requested workflow permits. Preserve unrelated slides, masters, notes and assets. Changing one slide does not authorize restyling the whole talk.

When the user adds another example or subpoint, retain the earlier ideas unless they replace or conflict with them. Nest supporting points under their parent idea rather than making every sentence a top-level bullet.

Use native PowerPoint objects and [mechanics](powerpoint.md). Preserve scientific labels and caveats, and keep generated output distinct from the speaker's interpretation. If requested wording changes meaning or evidence, identify the issue and resolve the scientific point before presenting the edit as supported.

Afterward, render and inspect affected slides and neighboring slides when their transitions/layout depend on the change. Verify links and native equation/text behavior as relevant. For insertion/deletion/reordering, refresh slide-ID mapping, backup placement and automatic numbering across the complete deck. For master/layout changes, inspect representative dependent slides throughout the deck.

Update the changed outline entries, source/asset records and `STATE.md`: current editable deck, review status, decisions, remaining questions and next action. If the user makes an independent manual edit later, inspect and adopt it before continuing. Do not assert validation of unchanged material that was not inspected. Answer-only work need not create a revision or alter metadata.

## Presentation notes

Write notes the presenter can use directly: talking points in their voice, relevant sources, and factual qualifications. Keep editing history, change requests, validation logs and phrases such as "requested by the speaker" in `STATE.md` or other workspace records. Replace superseded notes rather than accumulating contradictory revisions. Retain qualifications about evidence and attribution without attributing editorial responsibility to the user's request; raise an unresolved factual concern with the user directly.

## Review lessons and contribute upstream

At a natural handoff after substantial collaborative editing, ask once whether the user wants a short review of reusable lessons and a PR to the original guidance. Skip the offer if they have already requested or declined it, or deferred that work. Do not interrupt an active edit to require this review.

Present concrete proposed instructions and their appropriate home: general editing behavior in shared references, speaker preferences in that speaker's profile, and event-specific choices in `TALK.md` or local style files. Do not turn a one-off exception into a universal rule.

When the user authorizes the contribution, locate the original source repository from the skill's provenance or Git remote, inspect its current guidance and repository instructions, and make a focused change on a scoped branch. Validate the skill and affected links, then open a reviewable PR and return its link. Do not edit an installed plugin cache as a substitute for contributing to the source. Existing authorization to make the changes and open the PR is sufficient; merging remains a separate action.
