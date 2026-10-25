<div align="center">

<img src="bilder/icon.png" width="112" alt="BeyondCab">

# BeyondCab

**Step out of the cab.**<br>
Get out, walk around your truck, couple by hand, sign your papers, refuel and take a break – on foot and in first person in **Euro Truck Simulator 2** and **American Truck Simulator**.

[![Version](https://img.shields.io/github/v/release/Ku3rb1s/BeyondCab?label=Version&color=ff9500)](../../releases/latest)
![Windows 10/11](https://img.shields.io/badge/Windows-10%20%7C%2011-1f6feb)
![ETS2 and ATS](https://img.shields.io/badge/Games-ETS2%20%7C%20ATS-34c759)
![Free](https://img.shields.io/badge/free-no%20account-ff9f0a)

### [⬇&nbsp; Download BeyondCab](../../releases/latest)

[Deutsch](README.md) · English

<img src="bilder/einstellungen-en.png" alt="BeyondCab in the game: settings menu" width="900">

</div>

## What you get

🚶 **On foot** – Get out once the parking brake is on, then walk, run, jump and crouch. The ground comes from the game's physics, footsteps sound different on every surface, traffic brakes for you and gates open when you stand in front of them.

🔗 **Couple your trailer by hand** – Disconnect the lines, place the chocks, crank the landing gear (or drive it hydraulically), pull the kingpin release – and everything back again. With a checklist, a tug test and a walk-around inspection.

📄 **Real paperwork** – In ETS2 the CMR consignment note from the warehouse worker, in ATS the Bill of Lading. Sign and stamp it yourself and get it back signed at the destination. Plus seals, weighing tickets, dangerous goods papers, driver card or ELD, and police or DOT inspections.

⛽ **Pay at the pump** – Open the fuel cap, card into the terminal, PIN, watch amount and litres (gallons and dollars in ATS) count up, and get a receipt.

📦 **Road Trip (ATS)** – On courier jobs you pick up the parcel from the sender, put it on the passenger seat and hand it over to the recipient at the destination – with a delivery note.

🔦 **And more** – Remote key with windows and truck finder, flashlight, warning lights and chocks from the storage box, benches for a break, sleeping in the cab, controller support.

## Ready in 3 steps

1. **[Download](../../releases/latest)** and run `BeyondCab-Setup-….exe` – it finds ETS2 and ATS by itself and installs into both.
2. **Start the game** and confirm once that it may load SDK plugins.
3. **Stop, apply the parking brake, press E** – you're standing next to your truck. Ctrl + F7 opens the menu.

Nothing in the game is changed: no mods in the game files, no changes to `config.cfg`.

## Pictures

| | |
|---|---|
| ![Consignment note](bilder/frachtbrief-en.png) | ![Bill of Lading](bilder/bill-of-lading.png) |
| CMR consignment note (ETS2), signed | Bill of Lading with HAZMAT (ATS) |
| ![Paper folder](bilder/papiermappe-en.png) | ![Quick menu](bilder/schnellwahl-en.png) |
| Paper folder (P) | Quick menu (hold Tab) |
| ![Refuelling](bilder/tanken-en.png) | ![Refuelling in the US](bilder/tanken-us.png) |
| Fuel receipt, card terminal and pump | The same in ATS: gallons and dollars |
| ![Instructions in writing](bilder/weisungen-en.png) | ![ELD](bilder/eld.png) |
| ADR instructions in writing | ELD record (ATS) |

## Requirements

- Windows 10 or 11 (64-bit)
- Euro Truck Simulator 2 **1.61** and/or American Truck Simulator **1.61** on Steam, single player
- After a game update some features may stop working until a new version comes out. The plugin checks at start-up whether everything still fits and only switches off the affected part

---

## All the details

<details>
<summary><b>Walking</b></summary>

- Get out with the action key once the parking brake is on. The door opens and you're standing next to the truck – on the passenger side too
- Walk, run, jump, crouch. Slower uphill, slight head bob, adjustable body height
- The ground comes from the game's physics: pavements, ramps, stairs, loading docks. Crash barriers, fences and vehicles stop you
- Footsteps sound different on asphalt, gravel, grass, metal, snow and wood
- AI traffic brakes for you and honks if you stand on the road too long
- Gates and barriers at company yards open when you stand in front of them (ETS2)
- Optional arrows at the top of the screen show where your truck, trailer and the warehouse worker are

</details>

<details>
<summary><b>In the truck</b></summary>

- Switch to the passenger seat or lie down on the bed in a sleeper cab. The plugin finds out by itself whether your truck has a bed
- On the bed: hold the key to sleep (using the game's sleep dialog)
- On the passenger seat and on the bed it sounds like the cab, not like outside
- Driving time (optional): in ETS2 you insert your driver card into the tachograph at the start of your shift, in ATS you log in to the ELD. Driving and rest time show at the top right, and the device prints the daily printout or ELD record

</details>

<details>
<summary><b>Coupling by hand</b></summary>

- Uncoupling: disconnect air and electric lines, place the chocks, crank the landing gear down, pull the kingpin release
- Coupling: back under, check the fifth wheel, connect the lines, crank the landing gear up, remove the chocks. Then a tug test
- Hydraulic landing gear (car transporters, for example) works with a button instead of a crank – with its own steps and sounds
- Optional extra steps: safety catch on the coupling handle, trailer parking brake (red button), light check
- A checklist shows what comes next. If something ever gets stuck, “Coupling stuck?” in the menu resets the steps
- After coupling, walk around truck and trailer once: tyres, lights, load and doors, and the reefer unit on refrigerated trailers

</details>

<details>
<summary><b>Jobs and papers</b></summary>

- On every job a warehouse worker stands next to the trailer and hands you the papers: in ETS2 the multi-part CMR consignment note, in ATS the Bill of Lading – with companies, cities, cargo, weight and plates from the job
- You sign with the mouse and stamp it yourself. Set your name and town in the menu
- At the destination you hand them to the worker and get them back signed after unloading. “Skip parking” counts as the hand-over
- Sealed trailers, your own trailer with a loading sheet, pallet exchange (ETS2), weighing tickets for tank, silo and bulk loads
- Dangerous goods: in ETS2 per ADR with instructions in writing, in ATS per 49 CFR with HAZMAT marking and the ERG guide
- Police or DOT inspections: when the police stop you, they check your papers, driver card or ELD and, for dangerous goods, your equipment. Anything missing costs a fine
- Refrigerated trailers: print the temperature record at the reefer unit
- Everything is in the paper folder (P); your latest papers are kept in the menu under Papers

</details>

<details>
<summary><b>American Truck Simulator</b></summary>

BeyondCab notices by itself which game is running – there's nothing to choose.

- Bill of Lading instead of CMR, states instead of countries, dates in US format
- Refuelling in gallons and dollars, odometer in miles
- ELD instead of a driver card, a break after 8 hours of driving (Hours of Service), DOT inspections with three warning triangles and a fire extinguisher
- Own models for the warning light, warning triangle and flare
- **Road Trip**: on courier jobs by car you pick up the envelope, briefcase or parcel from the sender and sign the delivery note, put it on the passenger seat and hand it over to the recipient at the destination. The job then completes by itself. The parcel only shows up in the car once you've put it there

</details>

<details>
<summary><b>Refuelling</b></summary>

- Like the real thing: open the fuel cap, go to the pump, insert your fuel card, type your PIN (set in the menu), optionally the odometer, then refuel at the cap. With large tanks on both sides
- The pump display counts amount and volume, and you get a receipt with the local price, plates and odometer

</details>

<details>
<summary><b>Remote key, equipment and more</b></summary>

- Remote key: lock and unlock with indicators and an optional short honk, hold at the truck for the windows, hold far away to find it. Follow-me-home and automatic locking
- In the storage box behind the cab: warning lights, cones, warning triangle, chocks, fire extinguisher and a camping chair. Take them out, place them, pick them up again
- Quick menu (hold Tab), benches at rest areas to take a break
- Flashlight in your hand or on your head, with several modes
- Controller with Xbox or PlayStation symbols, all buttons can be remapped
- An introduction on first start, export and import of settings, German and English

</details>

<details>
<summary><b>Controls</b></summary>

| Key | Controller | What |
|---|---|---|
| E | X | Action: get out, get in, refuel, couple, papers … (hold where shown) |
| W A S D | left stick | walk |
| Shift | RT | run |
| Space | A | jump |
| Ctrl | B | crouch |
| T | LB | flashlight (hold: change mode) |
| K | RB | remote key: tap to lock/unlock, hold at the truck: windows, hold further away: find the truck |
| P | Y | paper folder; 1–4 (controller: D-pad) opens a sheet |
| Tab (hold) | D-pad up | quick menu |
| right mouse button | LT | zoom, magnifier on papers |
| Ctrl + F7 | – | menu |
| Ctrl + Alt + Z | Back (hold) | back to the truck |

All keys and buttons can be changed in the menu under **Keyboard** and **Controller**.

</details>

<details>
<summary><b>Settings and data</b></summary>

Sounds and lists (benches, fuel stations, parking) are built into the DLL. `Documents\<game>\BeyondCab\` only holds your settings (`beyondcab.ini`), what you've placed, your papers and the plugin's own models (`models\`, created by the plugin).

Your own sounds: a file with the same name in `BeyondCab\sounds\` replaces the built-in sound (for example `truck_lock.wav`).

The game log (`Documents\<game>\game.log.txt`) lists every message of the plugin, prefixed with `[BeyondCab]`. It helps when something goes wrong.

</details>

<details>
<summary><b>FAQ</b></summary>

**Windows warns when starting the setup (“Windows protected your PC”).**
The file isn't digitally signed. Click “More info” and “Run anyway”. To be sure, compare the checksum with `SHA256SUMS.txt` from the release:

```powershell
Get-FileHash .\BeyondCab-Setup-*.exe -Algorithm SHA256
```

**I can't get out.** Stop first and apply the parking brake. You can turn this off in the menu under **Truck**.

**The menu doesn't appear.** Check the game log for `[BeyondCab]`. If it's not there, the DLL is in the wrong folder or the SDK message at start-up was declined.

**I don't want paperwork.** Shipping papers, fuel card, chocks on jobs and driver card or ELD can each be turned off in the menu.

**I still have “ETS2 Walk” (1.0.x).** Just run the new setup. It removes the old `ets2_walk.dll`, and your settings and papers move to the `BeyondCab` folder.

**Does it work with TruckersMP?** No, single player only.

**Does it work alongside CabPlay?** Yes, both plugins run together.

</details>

<details>
<summary><b>Uninstall</b></summary>

Windows Settings → **Apps** → BeyondCab → Uninstall, or run the setup again and choose **Remove**. The game must be closed. The plugin is removed from both games; if you like, settings and papers go to the recycle bin.

</details>

<details>
<summary><b>Licenses and thanks</b></summary>

- Parts for reading game memory come from the [ETS2LA game plugin](https://github.com/ETS2LA/plugin) (MIT)
- [Dear ImGui](https://github.com/ocornut/imgui) (MIT), [MinHook](https://github.com/TsudaKageyu/minhook) (BSD-2), SCS Telemetry SDK, NVIDIA PhysX 3.4 (headers, BSD-3)
- Reading the game archives follows the map parser of [truckermudgeon/maps](https://github.com/truckermudgeon/maps), CityHash by Google (MIT)
- Hazard labels: public domain drawings from [Wikimedia Commons](https://commons.wikimedia.org/wiki/Category:Diagrams_of_ADR_markings)
- Sounds: [Kenney](https://kenney.nl) (CC0) and recordings from [Pixabay](https://pixabay.com) (Pixabay license, only redistributed together with the plugin)
- Built with [Claude Code](https://claude.com/claude-code) (Anthropic): Claude wrote the code, from ideas, requirements and in-game testing by Ku3rb1s

</details>

---

<sub>Fan project, not affiliated with SCS Software. Trademarks belong to their owners. Formerly “ETS2 Walk”. All changes: [CHANGELOG](CHANGELOG.md)</sub>
