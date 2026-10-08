# keel plugin: Tasks

A list of work items. Start a flow from a task with one button.

> **Status: planned.** The code still lives in [keel-v2](https://github.com/MiladNalbandi/keel-v2). It moves here step by step, as
> [the plugin plan](https://github.com/MiladNalbandi/keel-v2/tree/main/docs/plugins) says. There is nothing to install yet.

| | |
| --- | --- |
| id | `tasks` |
| needs | keel core (plugin SDK 1) |
| works with | — |
| parts | api · web · migrations |
| trust level | runs code in keel |

**What it adds to keel**

- the Tasks page (#/tasks)
- task cards in the Inbox

**Where the code is today (keel-v2)**

- `keel.api.tasks` (api)
- `web/src/pages/Tasks.tsx`
- `web/src/tasksApi.ts`

## Layout

```
keel-plugin.yml   the manifest
api/              Kotlin, a thin Spring Boot jar
web/              React pages and slots (an ES module)
migrations/       its own database tables (own Flyway history)
```

## Install

When it is released: in keel, **Control › Plugins › Marketplace › Tasks › Install**. keel checks the file's
signature, shows what the plugin may do, and asks you before it installs.

## License

MIT
