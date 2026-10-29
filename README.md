# Probius patch notes

Generated branch of the Probius patch-notes system. It holds no game data and shares no history
with the track branches.

- `index.json`: current pointers per track (occurrences, editions, states). Start here.
- `status.json`: pending, held and failed work for the operator.
- `ledger/observed.json`: builds seen on the patch server, used to detect missed releases.
- `occurrences/<track>/<id>.json`: one immutable record per published build.
- `comparisons/`, `editions/`, `official/`, `mappings/`, `generations/`, `budget/`: evidence, editions and bookkeeping written by later stages.

Files marked immutable are written once and never changed. Everything here is derived from the
published data branches; nothing on this branch is edited by hand except `mappings/pins.json`.
