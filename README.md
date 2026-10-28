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
| [EnDetailer](https://github.com/Enjuchan/EnDetailer) | A DPS meter showing what you are doing right now as a real-time value instead of the whole-fight average. Fight graph, details on hover and a history of the last ten fights. Requires IINACT. |
| [EnCounter](https://github.com/Enjuchan/EnCounter) | Counts emotes and chat messages directed at you and shows the tally as your title. Requires Honorific. |
| [EnMotion](https://github.com/Enjuchan/EnMotion) | Shows which emotes, dances and expressions your Penumbra mods change and plays them with one click. Favourites, direct idle pose selection and a compact view to keep it open while you play. Requires Penumbra. |
| [EnGlam](https://github.com/Enjuchan/EnGlam) | Pick the glamour you want, press start, and let AutoDuty farm the duties that drop it until it's yours. Requires AutoDuty and a rotation plugin. |

## Adding a new plugin

`repo.json` is a plain array — append another object for each plugin. The download links
point at `releases/latest/download/<Name>.zip`, so they stay valid across releases and
only `AssemblyVersion` has to be bumped when a new version ships. Dalamud compares that
value against the installed one to detect updates.

**Update the table above as well.** `repo.json` is what Dalamud reads; the table is what
people read. Forgetting it leaves the repository looking like it holds one plugin.
