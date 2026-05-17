---
name: web-project
description: Modern web project guidance organized from Vue, Pinia, Vue Router, Vuetify, React/Next.js performance, Vite, pnpm, and UI/UX design skills. Use when creating, modifying, reviewing, or debugging frontend web applications, build tooling, package management, state/routing/UI framework integrations, or product interface design.
---

# Web Project

Use this skill as the general frontend web project entry point. First identify the stack from repository files, then load only the relevant nested skill.

This skill provides framework and tooling references only. If it conflicts with the user's global coding specification or repository-local instructions, follow those higher-priority instructions.

## Index

- [vue](vue/SKILL.md): Vue 3 Composition API, SFCs, and Vue ecosystem routing.
  - [pinia](vue/pinia/SKILL.md): Vue state management and stores.
  - [vue-router](vue/vue-router/SKILL.md): Vue Router guards, params, lifecycle, and navigation gotchas.
  - [vuetify](vue/vuetify/SKILL.md): Vuetify components, layouts, theming, and migration notes.
- [react](react/SKILL.md): React and Next.js performance best practices.
- [vite](vite/SKILL.md): Vite config, plugin API, build, SSR, and migration work.
- [pnpm](pnpm/SKILL.md): pnpm commands, workspaces, dependency resolution, catalogs, patches, and CI usage.
- [design](design/SKILL.md): Penpot UI/UX design, design systems, accessibility, and component patterns.

## Selection Rules

1. For Vue files (`.vue`, Vue imports, Vue SFC macros), read `vue/SKILL.md`.
2. For Vue state, also read `vue/pinia/SKILL.md`.
3. For Vue routes, guards, params, or navigation bugs, also read `vue/vue-router/SKILL.md`.
4. For `vuetify` imports or Vuetify components/layout/theme work, also read `vue/vuetify/SKILL.md`.
5. For React or Next.js code, read `react/SKILL.md`. Do not load it for non-React frontend projects.
6. For `vite.config.*`, Vite plugins, build/SSR/library mode, or dev server issues, read `vite/SKILL.md`.
7. For `pnpm-lock.yaml`, `pnpm-workspace.yaml`, `.npmrc`, workspace filters, or dependency changes, read `pnpm/SKILL.md`.
8. For interface design, Penpot, accessibility design, layout design, design systems, dashboards, forms, or navigation design, read `design/SKILL.md` only when the user explicitly asks for UI/UX design work or the task is primarily a design task.
9. For Vuetify, first identify the installed Vuetify major version from project dependencies. Use Vuetify 4 migration or breaking-change guidance only when the project is on Vuetify 4 or the user explicitly asks about Vuetify 4 migration.

## Workflow

1. Detect existing framework, package manager, UI library, and build tool before changing files.
2. Prefer project-local conventions over generic framework defaults.
3. Load detailed nested references only when the current task needs them.
4. Validate with the repository's available scripts, using targeted checks before broad checks.

## Layout

```text
web-project/
+-- vue/
|   +-- pinia/
|   +-- vue-router/
|   +-- vuetify/
+-- react/
+-- vite/
+-- pnpm/
+-- design/
```
