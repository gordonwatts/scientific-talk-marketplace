# Select and extend profiles

Talk type and speaker are independent choices. Record selected profile IDs and local overrides in `TALK.md`. Read only the selected talk-type file; it owns that type's audience, narrative expectations and any type-specific visual settings. Shared workflow and speaker files must not repeat those settings.

Select the talk type from the request or existing brief; clarify it if needed. The bundled type is [colloquium style](../profiles/talk-types/colloquium.md), loaded only for that type. The speaker default, when appropriate, is Gordon: [content](../profiles/speakers/gordon/content.md) for voice/narrative and [visual](../profiles/speakers/gordon/visual.md) for reusable appearance preferences. Confirm fit rather than assigning Gordon's footer to another presenter. For an unimplemented type, establish audience, objectives and visual choices locally in `TALK.md` or `style/`; do not load an unrelated talk-type file.

Explicit user instructions and supplied template/style take precedence. Recorded local choices override bundled defaults. Within bundled guidance, selected talk-type visual settings override reusable speaker defaults for that type; the speaker's remaining preferences still apply. A difference that materially affects the task should be explained and, if genuinely ambiguous, resolved with the user. A profile is a starting point, not a reason to erase manual edits.

## Add a talk type

Add one concise `profiles/talk-types/<id>.md` containing audience, assumed knowledge, purpose, accessibility/depth expectations, narrative/timing considerations, review questions, and any type-specific visual defaults. Scope speaker-specific settings by speaker ID. Link it from the bundled-profile list in `SKILL.md`, and record its ID when selected. Keep reusable speaker preferences and PowerPoint implementation in their own files. Do not create empty placeholder profiles for unimplemented types.

## Add a speaker

Add `profiles/speakers/<id>/content.md` for voice and slide-content preferences and `visual.md` for native theme/layout settings, citation/footer preferences and visual patterns. Link both from `SKILL.md`. Supply self-contained defaults rather than references to a private old deck. Keep general PowerPoint mechanics in their shared reference.

For one talk's overrides, use its local `style/` files and link them from `TALK.md`; do not modify the plugin for a one-off exception. If a preference recurs, update the relevant maintained profile deliberately.
