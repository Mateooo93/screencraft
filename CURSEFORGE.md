# Screencraft

Watch videos and browse the web inside Minecraft, on screens you place in the world or
in a mini player that follows you while you play.

**Client-side only.** Works on any server, including Paper and Spigot, and nobody else
needs to install anything. Only you can see your screens.

## Screenshots

![YouTube on an in-world screen — address bar, back/forward/reload, and mouse/keyboard on the page](https://raw.githubusercontent.com/Mateooo93/screencraft/main/docs/curseforge/in-world-screen.png)

![Several screens at once — Cookie Clicker, YouTube, and anything else; each has its own browser](https://raw.githubusercontent.com/Mateooo93/screencraft/main/docs/curseforge/multiple-screens.png)

![Mini player (default key **K**) — keep a video in the corner while you walk around](https://raw.githubusercontent.com/Mateooo93/screencraft/main/docs/curseforge/mini-player.png)

## Required: MCEF Modern

Screencraft needs **MCEF Modern 0.3.3 or newer**, which provides the Chromium browser.
It is not on CurseForge, so download it here and put it in your `mods` folder next to
Screencraft:

- [MCEF Modern on Modrinth](https://modrinth.com/mod/mcef-modern)
- [MCEF Modern on GitHub](https://github.com/DimasKama/mcef-modern)

On first launch it downloads Chromium (about 150 MB). The older "MCEF" mod on
CurseForge is a different mod and does **not** work with Screencraft.

You also need **Fabric API**.

## Features

- **Several in-world screens** (3 by default, up to 5 in the settings, more through the
  config file). Hang them on walls, stand them on the floor or let them float in the air.
  Each one has its own browser, so they can all play something different.
- **Touchscreen controls.** Left-click a screen to click on the page. Right-click it to
  get your mouse cursor and click, drag, scroll and type right on the screen.
- **Address bar on every screen**, plus back, forward, reload and home buttons.
- **Full browser window.** `/screencraft` opens a browser with an address bar: type a
  website or anything you want to search.
- **Mini player.** Press **K** to keep the video in a corner of your screen while you
  walk, fight and build. Press **Left Alt** to click and type on it without stopping.
- **Settings menu** with performance profiles (Low, Balanced, High), sharpness
  (720p to 1440p), address bars on or off, screen sizes and keybinds.
- **Your screens are saved** per world and server, and come back when you rejoin.

## How to use

1. Hold a **stick** (you can pick another item in the settings, e.g. if you use
   Litematica) and right-click to start placing a screen. Aim at a wall, floor or
   the air and click again to place it.
2. Click the screen's address bar and type a website or a search, or run **/screencraft**.
3. Press **K** to show the mini player.

| Action | How |
|---|---|
| Move a screen | Aim at it with the stick and right-click |
| Remove a screen | Aim at it with the stick, sneak + right-click |
| Use the mouse and keyboard on a screen | Right-click it (without the stick), ESC to stop |
| Change the placement item | "Placement item" in the settings menu: search any item, modded ones included |
| Place screens without an item | Set "Placement item" to None and use the "Place / move screen" key |
| Settings | `/screencraft settings`, or the Settings button in the browser window |
| Open a page or search | `/screencraft <url or words>` |
| Remove all screens | `/screencraft remove` |
| Click/type on the mini player | **Left Alt** (you can still walk), Left Alt or ESC to go back |

All keys can be changed with the "Keybinds..." button in the settings menu, or in
Options > Controls > Screencraft.

**More than 5 screens:** open `config/screencraft/settings.json`, set `"screenHardLimit"`
to the number you want (up to 64), restart the game, then raise "Max screens" in the
settings menu. Each screen is a full browser, so many screens need a strong PC.

## Performance

Each screen is a real browser. Screens you are not looking at slow down automatically,
and the **Balanced** profile (default) keeps several screens smooth. Pick **High** in the
settings for full 60 fps everywhere and the best video quality on a strong PC, or **Low**
on a weaker one.

## Notes

- Works on Minecraft 1.21.10, 1.21.11, 26.1, 26.1.1, 26.1.2, 26.2 and 26.3. On CurseForge there is a separate
  download for each (including one file per 26.1 patch). Use the MCEF Modern file made for
  the same Minecraft version.
- On 26.3 with the Vulkan renderer, far-away screens are a little less smooth-looking
  than with OpenGL.
- Screencraft is not affiliated with or endorsed by Google or YouTube.
