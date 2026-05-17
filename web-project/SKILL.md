---
name: web-project
description: Modern web project guidance for Vue, React, Vite, pnpm, UI design, and Vue ecosystem integrations. Use when creating, modifying, reviewing, or debugging frontend web applications, especially projects involving Vue 3, Pinia, Vue Router, Vuetify, React/Next.js performance, Vite config/build tooling, pnpm workspaces/dependencies, or UI/UX design workflows.
---

# Web Project

Use this as the unified entry point for web application work. Load only the sub-skill files needed for the current task, then follow their references progressively.

## Routing

- **Vue application or component work**: read [vue/SKILL.md](vue/SKILL.md).
- **Pinia stores or Vue state management**: read [vue/pinia/SKILL.md](vue/pinia/SKILL.md) after the Vue guide.
- **Vue Router routes, params, guards, or navigation bugs**: read [vue/vue-router/SKILL.md](vue/vue-router/SKILL.md) after the Vue guide.
- **Vuetify components, layouts, theming, or imports from `vuetify`**: read [vue/vuetify/SKILL.md](vue/vuetify/SKILL.md) after the Vue guide.
- **React or Next.js implementation, review, or performance optimization**: read [react/SKILL.md](react/SKILL.md).
- **Vite config, plugins, build, SSR, library mode, or migration work**: read [vite/SKILL.md](vite/SKILL.md).
- **pnpm commands, dependency management, monorepos, catalogs, patches, or CI installs**: read [pnpm/SKILL.md](pnpm/SKILL.md).
- **UI/UX design, Penpot, design systems, accessibility, dashboard/form/navigation layout**: read [design/SKILL.md](design/SKILL.md).

## Workflow

1. Detect the project stack from files such as `package.json`, lockfiles, `vite.config.ts`, framework config, imports, and component extensions.
2. Read the smallest relevant sub-skill set from the routing list.
3. Prefer repository conventions over generic framework defaults.
4. For Vue projects, default to Vue 3 Composition API, TypeScript, and `<script setup lang="ts">` unless the existing codebase clearly uses another pattern.
5. For package operations, respect the detected package manager. If `pnpm-lock.yaml` or `pnpm-workspace.yaml` exists, use pnpm guidance.
6. For UI work, apply existing design tokens and component systems first. Use design guidance only to fill gaps or review usability.
7. Validate changes with the repo's available scripts, choosing targeted checks before broader runs.

## Structure

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
