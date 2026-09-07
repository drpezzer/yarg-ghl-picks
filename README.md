# GHL Picks — a YARG note theme

Guitar Hero Live style note art for YARG's six-fret highway: a guitar pick for the
single-button notes, pointing down for the white row and up for the black, and a
rounded square for the both-buttons note.

**This works on stock YARG.** It's an ordinary `.yargtheme`, so you don't need a
modified build.

<!-- screenshots go here -->

## Install

1. Download the file for your platform from
   [Releases](https://github.com/drpezzer/yarg-ghl-picks/releases):
   - **Windows** — `GHL-Picks-windows.yargtheme`
   - **Linux / Steam Deck** — `GHL-Picks-linux.yargtheme`
2. Drop it in YARG's `custom/themes` folder:
   - **Windows** — `%USERPROFILE%\AppData\LocalLow\YARC\YARG\release\custom\themes`
   - **Linux** — `~/.config/unity3d/YARC/YARG/release/custom/themes`
3. Restart YARG, then pick **GHL Picks** in your profile's theme setting.

Themes are read at startup, so it won't appear until you restart.

### Why two files

Unity asset bundles are built per platform, so the Windows file won't load on Linux
or the reverse. Both are built from the same source and share a theme id, so your
selection carries across if you play on both.

## What it changes

Only the **six-fret notes**. Frets, highway, five-fret, drums and keys are the
stock rectangular theme, untouched — so it layers onto the normal look rather than
replacing it.

Notes are drawn in flat GHL-style tones rather than the shimmering gems the
five-fret notes use. HOPOs and taps are the same shape at 85% and 72% size, and a
tap carries a purple band, following GHL's "don't strum this" convention. HOPOs
deliberately look like ordinary notes: a HOPO still needs a strum when your combo
is 0, so marking one never-strum would be a lie.

One limitation worth knowing: the inlay band is a fixed colour rather than
following your colour profile. YARG hands a single-button note one colour, so
there's nothing to read the opposite row's colour from. Under default colours it
looks as intended; heavily recoloured profiles will leave the bands as they are.

## Source

Authored by a script rather than by hand, so the shapes can be tuned and
regenerated: `Assets/Editor/Automation/GhlPickTheme.cs` and `ThemeExporter.cs` in
[drpezzer/YARG](https://github.com/drpezzer/YARG).

## Credit

Built for [YARG](https://github.com/YARC-Official/YARG) by the YARC Official team.
Guitar Hero and Guitar Hero Live are trademarks of Activision; this is unofficial
fan work with no affiliation.
