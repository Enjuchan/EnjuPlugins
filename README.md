# EnjuPlugins

Dalamud plugin repository. Add this URL in Dalamud under
*Settings → Experimental → Custom Plugin Repositories*:

```
https://raw.githubusercontent.com/Enjuchan/EnjuPlugins/main/repo.json
```

One entry covers every plugin listed below — you only ever add this repository once.

## Plugins

| Plugin | What it does |
|---|---|
| [EnDetailer](https://github.com/Enjuchan/EnDetailer) | A DPS meter showing what you are doing right now, over a rolling time window instead of the whole fight. Requires IINACT. |

## Adding a new plugin

`repo.json` is a plain array — append another object for each plugin. The download links
point at `releases/latest/download/<Name>.zip`, so they stay valid across releases and
only `AssemblyVersion` has to be bumped when a new version ships. Dalamud compares that
value against the installed one to detect updates.
