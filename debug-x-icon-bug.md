[OPEN]

## Goal
Debug why the X social login icon is blank, misaligned, or sized differently from other provider icons.

## Hypotheses
- The rendered X button is still using stored custom HTML from plugin settings instead of the default output.
- The X icon selector does not match the same layout rules as the other provider icons.
- The browser is showing a cached page or a different installed copy of the plugin.
- The X SVG itself is malformed or clipped by its own viewBox/path geometry.

## Evidence To Collect
- Actual rendered HTML for the X button in the login area.
- Which CSS classes are applied to the X button container and SVG.
- Whether the X button uses the default output path or stored custom HTML.
- Whether the current page is loading this plugin directory and not a stale asset.

## Status
- [ ] Instrument the X button rendering path.
- [ ] Collect runtime evidence from the login page.
- [ ] Identify the root cause.
- [ ] Apply the minimal fix.
- [ ] Verify pre-fix vs post-fix behavior.
