# Cashu Card ecosystem

The architecture diagram published on [cashucard.org](https://cashucard.org/developers#overview), covering card payments, issuance and recovery.

![Cashu Card ecosystem diagram](preview.jpg)

## Files

| Asset | Use |
| --- | --- |
| [Desktop SVG](cashucard-ecosystem.svg) | Landscape architecture map, 1000 × 824 |
| [Phone SVG](cashucard-ecosystem-mobile.svg) | Portrait composition, 360 × 1168 |
| [Preview](preview.jpg) | Published diagram with its legend and hosting note |

Both SVGs are scalable, self-contained vectors with editable text, component shapes and connectors. The card and applet appear together; wallet/till/mint payments, CCP/ops-service issuance and supporting recovery tools have separate paths.

## Legend and hosting

- Green solid lines: NFC.
- Pale solid lines: online APIs.
- Dashed lines: backups and alerts.

The Atoll asterisk refers to the Workers/R2 pairing path. The standalone Docker service uses filesystem exports with operator-supplied scheduled copy and alert jobs. Keep this context with the diagram when reusing it.

## Source and updates

Imported on 2026-10-26 from [cashucard/cashucard at a8ee1e6](https://github.com/cashucard/cashucard/commit/a8ee1e64bec66e6842c2cc64394c25a9b204707e), merged in [PR #183](https://github.com/cashucard/cashucard/pull/183).

The editable generator is [website/tools/ecosystem.py](https://github.com/cashucard/cashucard/blob/a8ee1e64bec66e6842c2cc64394c25a9b204707e/website/tools/ecosystem.py). In a checkout of that repository, run `python3 website/tools/ecosystem.py` to regenerate its two SVGs, or add `--check` to verify them. Refresh both files and the preview together when the architecture changes.

## License

MIT, with the source project's copyright notice preserved in [LICENSE](LICENSE).
