# Zacism Global Scanner data contract

The Zacism app publishes all scanner data from one canonical source: `ZacismGlobalScanner`.

Current files:

- `global.json` — ranked cross-instrument opportunities for the main public scanner view.
- `investment.json` — long-term research reports, high-conviction global scanner ideas, theme universe, and funnel results.
- `options.json`, `swing.json`, `earnings.json`, `new_floats.json`, `unusual_volume.json`, `short_squeeze.json` — focused slices from the same scanner state.

Every scanner row should include `instrumentKind` (`Stock`, `ETF`, `Option`, `Future`, etc.) so public consumers can compare short-term and long-term performance by instrument type without needing separate scanner implementations.
