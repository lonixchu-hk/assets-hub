# SVG background audit

Chromium rendered all 37 saved SVGs on a dark background and decoded them to a canvas. The repository had no existing coordination files or project documentation beyond the README.

## Findings

- `images/cert-badge/aca_cc.svg` and `aca_dev.svg` have white squares inside their existing transparent margins. Preserve the shield interiors and lettering.
- `images/cert-badge/cks.svg` has a white canvas outside the blue outline. Preserve the white interior and labels. No AKS asset or reference was found in the current project or reachable Git history. CKS is independently in scope.
- `images/cert-badge/google_project_management_v3.svg` has a pure-white canvas. Preserve the almost-white title panel and other light artwork.
- `images/logo/` has white backings on `alibaba.svg`, `fimmick.svg`, `github.svg`, `lf.svg`, `ms.svg`, `mtr.svg`, `pmi.svg`, and `ztore.svg`. `isc2.svg` has white bands above and below its green artwork.
- The remaining 24 SVGs have transparent canvases or intentional colored brand backgrounds and white artwork.

## Completed cleanup

After approval, removed exterior white backing from the four badges and nine logos above. Each SVG retains its original path, dimensions, and wrapper. The cleanup preserves enclosed white artwork, including the CKS interior, the Google title panel, the GitHub Octocat, the MTR emblem, and the Ztore lettering.

Chromium rendered all 13 edited SVGs with transparent exteriors and displayed them on light and dark backgrounds. The two ACA badges and Google Project Management match their original white-background composites pixel for pixel. Differences in the other ten white-background composites are limited to cleaned backing and antialiased edges. The other 24 SVGs required no edits.

## Remaining work

The approved batch is complete. If AKS refers to another asset, obtain its source path before further edits.
