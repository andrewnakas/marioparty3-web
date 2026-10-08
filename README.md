# marioparty3-web

Mario Party 3 in the browser, bring your own ROM. Live at
https://andrewnakas.github.io/marioparty3-web/ and listed on https://decompgames.com.

**No game data is in this repository or on the page.** You pick your own ROM; it is read
in the tab and never uploaded.

## What this is

- **Source project:** [mariopartyrd/marioparty3](https://github.com/mariopartyrd/marioparty3) at `34994c4a008552f0b56d69216e8384f0a70e08df`.
- **Matching build:** All 575 C units were compiled with GCC 2.7.2 and a period GNU as; the linked 32 MiB ROM has SHA-1 `6beb80ff822b96bcf85dcdb512e8b2b7969d8259`, zero bytes different from the USA cartridge. The decompilation is partial: much of the game is still included as assembly.
- **Browser player:** EmulatorJS 4.2.3 with the libretro Mupen64Plus-Next core (WebAssembly). This is emulation of the rebuilt ROM, not a native
  port of the game's code to WebAssembly.

## Tested

A Chilly Waters board turn, the Crazy Cogs minigame and the return to the board, a save-state restore and a cartridge-save round trip (muted). Audio has not been listened to: every test ran muted. Nothing
beyond that scope has been played.

## Layout

- `web/` — the page (published as the `gh-pages` branch).
- `web/THIRD_PARTY.md` — licences of the vendored runtime.
