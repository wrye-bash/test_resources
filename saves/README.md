Saves & Cosaves
=========

These folders house saves and cosaves for each game.

For saves, the `.meta` format looks like this:

```toml
TODO
```

For xSE cosaves, the `.meta` format looks like this:

```toml
[cosave_header]
# The magic number of this cosave; 4-byte string
savefile_tag = "SKSE"
# The format version of this cosave; integer
format_version = 1
# The internal major version of the script extender that created this cosave;
# integer
se_version = 48
# The internal minor version of the script extender that created this cosave;
# integer
se_minor_version = 263
# The version of the game that this cosave was created on; integer
game_version = 0x09200000
# The number of plugin chunks denoted in the header; integer
num_plugin_chunks = 5

[cosave_body]
# The masters listed in the first chunk of the first plugin chunk (either MODS
# or PLGN)
cosave_masters = [
    "Skyrim.esm",
    "Update.esm",
    "Enderal - Forgotten Stories.esm",
    "RaceMenu.esp",
    "EHQM.esp",
    "Bashed Patch, 0.esp",
]
# Whether or not the masters listed above match the actual load order in-game
# at the time the cosave was created
masters_are_accurate = true
```

For Pluggy cosaves, the `.meta` format looks like this:

```toml
TODO
```
