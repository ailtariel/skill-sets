Personal customized skill sets.

## Install

Install the general frontend entry skill from this repository:

```bash
npx skills add https://github.com/ailtariel/skill-sets --skill web-project
```

For local testing from this checkout:

```bash
npx skills add . --skill web-project
```

## Update

Use `update_skills.py` to stage or apply updates from configured git sources.

```bash
python update_skills.py --list
python update_skills.py --skill vue,pinia
python update_skills.py --skill vue,pinia --apply
python update_skills.py --apply
```

Without `--apply`, updates are staged under `tmp/update-skills/staged` and repository files are not changed.

## Sources

These paths are used by `update_skills.py`.

| Local path | Source |
| --- | --- |
| `web-project/SKILL.md` | Local aggregate entry point; maintained in this repository. |
| `web-project/vue/` | `https://github.com/antfu/skills.git` -> `skills/vue` |
| `web-project/vue/pinia/` | `https://github.com/antfu/skills.git` -> `skills/pinia` |
| `web-project/vue/vue-router/` | `https://github.com/JetBrains/skills.git` -> `vue-router-best-practices` |
| `web-project/vue/vuetify/` | `https://github.com/skilld-dev/vue-ecosystem-skills.git` -> `skills/vuetify-skilld` |
| `web-project/react/` | `https://github.com/vercel-labs/agent-skills.git` -> `skills/react-best-practices` |
| `web-project/react/ant-design/` | Local Ant Design guidance; maintained in this repository. |
| `web-project/vite/` | `https://github.com/antfu/skills.git` -> `skills/vite` |
| `web-project/pnpm/` | `https://github.com/antfu/skills.git` -> `skills/pnpm` |
| `web-project/design/` | `https://github.com/github/awesome-copilot.git` -> `skills/penpot-uiux-design` |
