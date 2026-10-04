# Scientific Talks

A local, skills-only plugin for developing scientific talks with an LLM: chapter outline, slide outline, graphics and evidence, native PowerPoint construction, and subsequent revision. Version 0.1.1 contains one skill, a colloquium style file, and Gordon Watts's independent speaker profile. It needs no MCP server or account connection. PowerPoint work requires an available desktop PowerPoint installation and a supported means of controlling it.

## Read first

1. [Skill entry point](plugins/scientific-talks/skills/scientific-talks/SKILL.md): workflow and information lookup.
2. The selected talk-type file: [colloquium style](plugins/scientific-talks/skills/scientific-talks/profiles/talk-types/colloquium.md) holds all colloquium-specific guidance. Skip it for other talk types.
3. [Gordon's content style](plugins/scientific-talks/skills/scientific-talks/profiles/speakers/gordon/content.md) and [visual style](plugins/scientific-talks/skills/scientific-talks/profiles/speakers/gordon/visual.md): reusable speaker preferences.
4. [PowerPoint mechanics](plugins/scientific-talks/skills/scientific-talks/references/powerpoint.md): native editing and consistency requirements.
5. [Talk starter](plugins/scientific-talks/skills/scientific-talks/assets/starter/TALK.md) and [status starter](plugins/scientific-talks/skills/scientific-talks/assets/starter/STATE.md): context carried between conversations.

The remaining references are linked from the entry point. [Origins](plugins/scientific-talks/skills/scientific-talks/references/origins.md) records extraction decisions. [Acceptance scenarios](validation/scenarios.md) and [validation results](validation/results.md) describe the checks.

## Install from GitHub

Register this marketplace in a supported Codex CLI:

```powershell
codex plugin marketplace add gordonwatts/scientific-talk-marketplace
```

Then select **Scientific Talks** in the Plugins Directory and install **scientific-talks**. Private repository access requires authentication and permission to read the repository. Registration and installation are separate from publishing the repository.

## Local discovery and installation

This folder is the marketplace root. Its `.agents/plugins/marketplace.json` points to `./plugins/scientific-talks`, relative to this folder, not to `.agents/plugins/`. Open this folder as a project for local inspection. The package has not been registered or installed by its authoring process.

In a supported Codex CLI, registration can be requested with:

```powershell
codex plugin marketplace add ./scientific-talks-plugin
```

Run that command from the parent folder, or pass the absolute path to this folder. Alternatively, repo-scoped discovery can use this root's catalog. Restart the desktop app as required, choose the **Scientific Talks** marketplace in the Plugins Directory, and install **scientific-talks**. Verify that the skill is visible. Installed clients may show a namespaced invocation; select the skill from the UI if `$scientific-talks` is ambiguous.

Local installations load a cached copy. After editing the source, refresh the marketplace/local installation using the client's supported controls and restart the desktop app; confirm the updated files are loaded. Editing this folder alone does not prove an installed copy changed. See [official packaging and marketplace guidance](https://developers.openai.com/plugins/build/plugins) for current client behavior.

## Starting a talk

Ask: "Use $scientific-talks to prepare a 45-minute colloquium. Start with the chapter outline."

The skill establishes a separate talk workspace using its starter files. It uses PowerPoint's built-in default template unless a template is supplied, with appearance defined by the selected profiles. Native editable objects and shared theme/master/layout formatting apply across talk types. No binary template or completed talk is bundled.

## Repository structure

The repository root contains the marketplace catalog, `plugins/`, and this guide. Catalog and plugin paths remain relative and travel together. The marketplace's internal name is `gordon-talks`; its repository is `gordonwatts/scientific-talk-marketplace`. A local working copy can be registered using its root path as described above. No license has been selected or bundled.

To extend the guidance, follow [profile extension instructions](plugins/scientific-talks/skills/scientific-talks/references/profiles.md). Adding a talk type does not require another skill.
