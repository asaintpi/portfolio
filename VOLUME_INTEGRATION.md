# VOLUME BUTTON — CLAUDE CODE INTEGRATION

## Step 1: Drop the file first

Before giving Claude Code the prompt below, manually create the file:

```
mkdir -p volume
# Then paste the volume-v2.html contents into volume/index.html
# (Use the downloaded volume-v2.html file from Claude chat)
```

Or just drag the downloaded `volume-v2.html` into your repo as `volume/index.html`.

-----

## Step 2: Copy-paste this entire block into Claude Code:

-----

Read CLAUDE.md first. Then do the following:

A new interactive experience called "The Volume Button" has been added at `volume/index.html`. It's a standalone art piece — a volume knob that goes past 100 and evolves through psychological phases (commentary, glitching, pleas, poetic ending). Like VOID and Resonance, it's something visitors interact with.

**Your tasks:**

1. **Read `volume/index.html`** to understand what it is. Do not modify the core experience — the commentary text, phase thresholds, knob physics, and ending lines are all final and intentional.
1. **Add a back-navigation link** to the top-left of the Volume page. Ghost opacity, mono font, small — same pattern as back-nav on LUMIN or Resonance pages. Text: "← Arnaud Saint-Pierre" linking back to the site root. Should be barely visible until hover.
1. **Add meta tags** to the Volume page head: `og:title` = "VOLUME", `og:description` = "How far will you go?", plus the site's standard favicon link. Match the meta tag pattern from index.html.
1. **Add "Volume" to the site navigation** on index.html. Place it in the interactive/experimental section — same group as VOID, Resonance, LUMIN. It should appear ABOVE LUMIN in the nav order. Link to `/volume/`. Match existing nav item casing and styling.
1. **If the main site has a shared font loading strategy** (self-hosted fonts, different CDN, etc.), update the Volume page's font imports to match. Currently it uses Google Fonts CDN for Space Mono, Libre Caslon Display, and Inter.
1. **Verify**: Load the page, turn the knob to 1000, confirm the ending plays and the "again" button works. Check for console errors.
1. **Commit**: `feat: add Volume — interactive experience`

Do NOT add analytics, loading screens, localStorage, social sharing, or any UI beyond what's already in the file. The page is intentionally minimal and self-contained.
