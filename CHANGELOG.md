# Änderungen · Changelog

## 1.3.2

### Verbessert (aus 1.3.1)

- Log und Prüfbericht sind jetzt auf Englisch – so lassen sich Meldungen aus aller Welt leichter auswerten. Das Menü bleibt deutsch bzw. englisch wie eingestellt
- Controller-Diagnose im Log: über welchen Weg das Spiel den Controller liest (XInput, DirectInput, HID), wann BeyondCab ihn sperrt (nur beim Laufen und im Menü) und eine Warnung, falls ein gedrückter Trigger oder Knopf im Truck beim Spiel nicht ankommt

### Behoben

- Controller über DirectInput (aus 1.3.1): Legt das Spiel ein Eingabegerät neu an, konnte BeyondCab einen Controller für eine Maus halten. Das wird jetzt alle 2 Sekunden neu geprüft, und Controller-Daten werden von der Maus-Sperre nie mehr verändert (Issue #1)
- Tieflader und Pritschen mit Ladung: Die Prüfung der Anhänger-Beleuchtung (und Plombe/Ladungssicherung) lag mitten auf dem Deck, weil die Messung des Hecks die Ladung traf. Jetzt wird in Deckhöhe nachgemessen
- Taschenlampe mit 3D-Modell: Die Lampe in der Hand leuchtete grell weiß, weil ihr eigenes Licht sie anstrahlte
- Abgeben: „Vor der Abfahrt – Unterlegkeile entfernen“ erschien am Ziel und beim Abkoppeln, obwohl die Keile am Auflieger bleiben

Danke an STyx2909 für das Video!

---

### Improved (from 1.3.1)

- Log and check report are now in English, which makes reports from around the world easier to read. The menu stays German or English as set
- Controller diagnostics in the log: how the game reads your controller (XInput, DirectInput, HID), when BeyondCab blocks it (only while walking and in the menu), and a warning if a pressed trigger or button doesn't reach the game while you're in the cab

### Fixed

- Controller via DirectInput (from 1.3.1): when the game re-created an input device, BeyondCab could take a controller for a mouse. This is now re-checked every 2 seconds, and controller data is never changed by the mouse block (issue #1)
- Lowbeds and flatbeds with cargo: the trailer light check (and seal/load securing) sat in the middle of the deck because the rear measurement hit the cargo. The rear is now measured again at deck height
- Flashlight with 3D model: the lamp in your hand glowed bright white because its own light lit it up
- Delivery: "Before driving off – remove wheel chocks" showed up at the destination and while uncoupling, although the chocks stay at the trailer

Thanks to STyx2909 for the video!

---

## 1.3.1

### Verbessert

- Log und Prüfbericht sind jetzt auf Englisch – so lassen sich Meldungen aus aller Welt leichter auswerten. Das Menü bleibt deutsch bzw. englisch wie eingestellt
- Controller-Diagnose im Log: über welchen Weg das Spiel den Controller liest (XInput, DirectInput, HID), wann BeyondCab ihn sperrt (nur beim Laufen und im Menü) und eine Warnung, falls ein gedrückter Trigger oder Knopf im Truck beim Spiel nicht ankommt

### Behoben

- Controller über DirectInput: Legt das Spiel ein Eingabegerät neu an, konnte BeyondCab einen Controller für eine Maus halten. Das wird jetzt alle 2 Sekunden neu geprüft, und Controller-Daten werden von der Maus-Sperre nie mehr verändert (Issue #1)

---

### Improved

- Log and check report are now in English, which makes reports from around the world easier to read. The menu stays German or English as set
- Controller diagnostics in the log: how the game reads your controller (XInput, DirectInput, HID), when BeyondCab blocks it (only while walking and in the menu), and a warning if a pressed trigger or button doesn't reach the game while you're in the cab

### Fixed

- Controller via DirectInput: when the game re-created an input device, BeyondCab could take a controller for a mouse. This is now re-checked every 2 seconds, and controller data is never changed by the mouse block (issue #1)

---

## 1.3.0

### Neu

- Reisebusse (Coach-DLC für ETS2): MAN Lion's Coach, Scania Touring und Volvo 9700 werden erkannt. Nötig ist der Führerschein Klasse D, mit Anhänger DE
- Ein- und Aussteigen an der vorderen Einstiegstür rechts. Die Türen gehen dabei auf. An der Tür kurz drücken = einsteigen, halten = Türen auf bzw. zu
- Im Bus laufen: vom Fahrersitz aufstehen, durch den Gang bis zur letzten Reihe, über die Stufen der Vorder- oder Mitteltür hinaus und wieder hinein. Stufen und Böden stammen aus den Modellen der Busse
- Volvo-Doppeldecker: Treppe zum Oberdeck. Im niedrigen Unterdeck bleibt die Augenhöhe unter der Decke
- Bus: Staukasten am Gepäckraum zwischen den Achsen, Tankdeckel auf der Seite des Tanks, keine Liege
- Einstellung „Im Bus mit der Innenansicht laufen“ (standardmäßig aus): Innenklang des Busses, das Innenmodell des Spiels ist aber nicht überall vollständig

### Hinweise

- Getestet ist vor allem der Scania Touring. Wenn bei MAN oder Volvo Stufen oder Höhen nicht passen, bitte als Issue melden
- Deine eigene Türtaste des Spiels wird mitgezählt, solange du am Fahrersitz bist. Eine Belegung auf dem Controller sieht BeyondCab nicht

---

### New

- Coaches (Coach DLC for ETS2): MAN Lion's Coach, Scania Touring and Volvo 9700 are recognised. They need a class D licence, DE with a trailer
- Get in and out at the front entrance door on the right. The doors open for you. At the door tap = get in, hold = open or close the doors
- Walk inside the coach: stand up from the driver's seat, walk the aisle to the last row, leave and enter by the steps of the front or middle door. Steps and floors are taken from the coach models
- Volvo double-decker: stairs to the upper deck. On the low lower deck your eye height stays below the ceiling
- Coach: storage box at the luggage hold between the axles, fuel cap on the tank's side, no bunk
- Setting "Walk the bus in interior view" (off by default): the coach's cabin sound, but the game's interior model is not complete everywhere

### Notes

- Mostly tested with the Scania Touring. If steps or heights don't fit on the MAN or Volvo, please open an issue
- Your own door key of the game is counted while you're in the driver's seat. A controller binding is not seen by BeyondCab

---

## 1.2.6

### Behoben

- Leistung: Der Fahrtenschreiber speichert im Hintergrund, das konnte vorher kurz stocken
- Kuppeln: Bei manchen Aufliegern ließ sich die Anhänger-Beleuchtung nicht prüfen. Der Punkt lag hinter dem Heck, dort kam nur „Plombe prüfen“. Die Prüfung sitzt jetzt am Heck und hat Vorrang, solange sie dran ist

---

### Fixed

- Performance: the tachograph now saves in the background, which could cause a brief stutter before
- Coupling: on some trailers the trailer light check could not be reached. Its point sat behind the rear, where only "Check seal" came up. It now sits at the rear and takes priority while it is due

---

## 1.2.5

### Neu

- Fahrtenschreiber: 90 Stunden Lenkzeit in zwei Wochen werden geprüft. Bleibt von den 90 h weniger als 56 h übrig, sinkt die Wochengrenze entsprechend (abschaltbar unter Lenkzeit)
- Fahren ohne Karte bzw. ohne ELD-Anmeldung wird jetzt mitgeschrieben und steht auf Ausdruck und Wochenübersicht
- Fährhafen-Check (ETS2, abschaltbar): Führt die Navi-Route über einen Hafen nach Großbritannien oder von Griechenland und Albanien nach Italien, oder stehst du dort, erinnert BeyondCab daran, den Auflieger auf blinde Passagiere zu prüfen – vier Punkte im Rundgang. Wer es auslässt, riskiert bei der Ankunft eine Strafe
- Frachtbrief: Der Empfänger vermerkt Verspätungen, und Schäden je nach Ausmaß (leichte Schäden, Vorbehalt, Schadensmeldung)
- Nasse Schritte: Bei Regen und nassem Boden mischen sich echte Wasser-Aufnahmen unter die Schritte, je nach Nässe im Spiel mehr oder weniger, ab und zu mit Pfütze (abschaltbar, Lautstärke einstellbar unter Klänge)

### Geändert

- Ruhezeit, Warnung, Anzeige, Ausdruck, Wochenübersicht und Kontrolle rechnen jetzt alle nach dem Fahrtenschreiber. Vorher kam die Ruhezeit aus dem Müdigkeits-Zähler des Spiels und konnte der Wochenübersicht widersprechen
- ETS2: Die 56 h gelten wie im Gesetz je Kalenderwoche (Montag bis Sonntag). Gezählt wird je Schicht statt je Kalendertag, auch über Mitternacht. Geteilte Ruhe (3 + 9 h) zählt als volle Ruhe
- Menü: Seiten neu gegliedert (Bewegung und Blick, Kuppeln und Kontrollen, Auftrag und deine Angaben, Lenkzeit, Lautstärken nach Ort), und es ist mehr auf einmal sichtbar
- Der dritte 10-h-Tag einer Woche und die vierte verkürzte Ruhe zwischen zwei Wochenruhen gelten als Verstoß
- Kontrolle: Es kostet nur noch, wer ohne Karte gefahren ist – nicht schon, wer ohne Karte steht. Zu lange Lenkzeit und zu kurze Ruhe seit der letzten Kontrolle werden geahndet

### Behoben

- Prüfbericht und Log zeigten Adressen als „FEHLT“, die in der laufenden Spielversion durch eine andere ersetzt sind
- Fahrtenschreiber: Auf Fähre und Zug blieb die Fahrerkarte nicht gesteckt, danach drohte ein Bußgeld wegen Fahrens ohne Karte
- Fahrtenschreiber: Nach zu kurzer Ruhe zeigte die Anzeige wieder die volle Restzeit. Lenkzeit und Dienstfenster laufen jetzt weiter, bis eine gültige Ruhe kommt, und die Kontrolle berechnet das nicht doppelt
- Doppel- und Dreifachzüge: Das Heck kommt jetzt aus den Spieldaten statt aus einer Schätzung. ATS-Dreifachzüge mit Dollys werden bis zum letzten Anhänger erkannt, vorher lagen Plombe, Ladungs- und Lichtkontrolle am mittleren
- Tieflader: Das Heck stimmt jetzt auch ohne Messung
- Motorwagen mit Anhänger (nur Mods): Es kuppelt das Spiel, statt nicht vorhandene Stützen zu verlangen
- Fahrtenschreiber: Im Hauptmenü stand beim Spielstart oben die Ruhezeit-Warnung, obwohl noch gar kein Profil geladen war
- Frachtpapiere: An Firmen weit außerhalb der Stadt kam kein Mitarbeiter mit den Papieren
- Doppelzüge: Mitarbeiter und Empfänger standen manchmal im zweiten oder dritten Anhänger
- Gefahrgut: Ethanol, Lösungsmittel und Altbatterien fehlten in der Liste
- Frachtbrief: Maschinen, Tank- und Schüttgut standen als „Euro-Paletten“ da. Jetzt lose, Stück, Container oder Tiere je nach Aufbau
- Palettentausch: Container auf Pritsche tauschten keine Paletten mehr
- Frachtbrief: Das Kennzeichen des Aufliegers fehlte, wenn er erst nach dem Unterschreiben gekuppelt wurde
- Doppelzüge: Plombe und Rückleuchten liegen jetzt am letzten Anhänger
- ATS: Kühlgerät, Temperatur-Ausdruck in °F, Wiegeschein in lb
- Abfahrtskontrolle: Der Balken läuft nach dem Loslassen wieder von vorn, die Rückleuchten gehen beim zweiten Anlauf wieder an
- Fährhafen-Check: Die Prüfpunkte verteilen sich jetzt über den ganzen Auflieger
- Kontrolle: Eine zu lange Schicht kostete doppelt (Ruhezeit überzogen und Lenkzeit überschritten)
- Bescheide und Belege: Auf Deutsch stehen jetzt deutsche Ortsnamen (München statt Munich)
- Bescheide: Sachbearbeitung und Beamte wechseln und passen zum Land, statt immer Frau Becker und zufälliger Namen. Anschrift und Telefon der Behörde passen zur Stadt, im Ausland mit Ortsnamen und Postfach der Landessprache. Eigene Anschrift (Straße, PLZ) lässt sich freiwillig eintragen

---

### New

- Tachograph: 90 hours of driving in two weeks are checked. If fewer than 56 h remain of the 90, the weekly limit drops accordingly (can be turned off under Driving time)
- Driving without a card or ELD login is now recorded and shows on the printout and the weekly summary
- Ferry port check (ETS2, optional): if your route uses a port to Britain, or from Greece and Albania to Italy, or you stand at one, BeyondCab reminds you to check the trailer for stowaways – four points on a walk-around. Skip it and you risk a penalty on arrival
- Consignment note: the receiver notes late deliveries, and damage by extent (minor, with reservation, claim to follow)
- Wet footsteps: in rain and on wet ground real water recordings mix into your steps, more or less depending on how wet the game says it is, with the odd puddle (can be turned off, volume under Sounds)

### Changed

- Rest time, warning, display, printout, weekly summary and inspections now all use the tachograph. Rest time used to come from the game's fatigue counter and could contradict the weekly summary
- ETS2: the 56 h apply per calendar week (Monday to Sunday) as in the law. Driving is counted per shift instead of per calendar day, also across midnight. A split rest (3 + 9 h) counts as a full rest
- Menu: pages reorganised (movement and view, coupling and checks, job and your details, driving time, volumes by place), and more fits on screen
- The third 10-hour day of a week and the fourth reduced rest between two weekly rests count as violations
- Inspections: only driving without a card costs money, not standing without one. Driving too long and resting too little since the last inspection are fined

### Fixed

- The check report and log showed addresses as "FEHLT" that another one replaces in the running game version
- Tachograph: the driver card was pulled on ferries and trains, risking a fine for driving without it afterwards
- Tachograph: after too short a rest the display went back to the full remaining time. Driving time and the duty window now carry on until a valid rest, and inspections don't charge for it twice
- Doubles and triples: the rear end now comes from the game data instead of an estimate. ATS triples with dollies are recognised up to the last trailer; the seal, load and light checks used to sit at the middle one
- Lowboys: the rear end is now right even without a measurement
- Rigid trucks with a drawbar trailer (mods only): the game does the coupling instead of asking for landing gear that isn't there
- Tachograph: the rest time warning showed at the top of the main menu at game start, before any profile was loaded
- Shipping papers: at companies far outside town no worker came with the papers
- Double trailers: workers and receivers sometimes stood inside the second or third trailer
- Hazmat: ethanol, solvents and used batteries were missing from the list
- Consignment note: machinery, tank and bulk goods were listed as “Euro pallets”. Now bulk, pieces, container or head depending on the trailer
- Pallet exchange: containers on flatbeds no longer swap pallets
- Consignment note: the trailer plate was missing if the trailer was coupled after signing
- Double trailers: seal and tail lights are now at the last trailer
- ATS: refrigeration unit and temperature printout in °F, scale ticket in lb
- Walk-around check: the bar restarts after letting go, and the tail lights come on again on the second try
- Ferry port check: the check points now cover the whole trailer
- Inspections: an overlong shift was fined twice (rest overdue and driving time exceeded)
- Fine notices: clerks and officers now vary and fit the country instead of always Frau Becker and random names. The authority's address and phone fit the city, abroad with local place names and PO box wording. You can optionally enter your own address (street, postcode)

## 1.2.4

### Neu

- Erste Schritte: beim ersten Aussteigen, zu Fuß, am Truck, beim Kuppeln, Tanken und bei den Papieren zeigt eine Karte rechts, welche Tasten du brauchst – jede einmal, genau dann, wenn es so weit ist. Abschaltbar und von vorn unter Menü › Allgemein › Hilfe
- Prüfung beim Start: nach einem Spiel-Update sagt BeyondCab einmal, ob alles passt. Der Prüfbericht (BeyondCab\pruefbericht.txt, im Menü unter Spielversion › Öffnen) listet jede geprüfte Spiel-Funktion – hilfreich für eine Fehlermeldung
- Pausen-Tagebuch: in der Papiermappe liegt die Wochenübersicht des Fahrtenschreibers – je Tag ein 24-Stunden-Streifen mit Lenken, Arbeit, Pause und Ruhe, dazu die Summen, die Woche gegen 56 h und was zu lang oder zu kurz war (ATS: 8 Tage, Hours of Service)

### Behoben

- Fahrtenschreiber: Laufen zählte immer als Arbeit (auch die Pause auf der Bank), wurde aber trotzdem als Pause angerechnet. Jetzt ist nur Kuppeln, Tanken und Unterschreiben Arbeit – und Arbeit unterbricht in der EU die 45-Minuten-Pause (USA: zählt für die 30-Minuten-Pause mit)
- Physik ging nach einem Spielstand- oder Profilwechsel bis zum Neustart des Spiels ganz aus (kein Boden, keine Kollision) – jetzt wird sie neu gesucht
- Tasten auf Pfeilen, rechter Strg, Alt Gr usw.: die Aktionstaste ging trotz Hinweis auch ans Spiel, durchgelassene Spieltasten wurden geschluckt
- Englische Tastatur: Hinweise zeigten „Z“ statt „Y“ (Tastennamen jetzt nach der eingestellten Belegung)
- Menü › Tastatur: „Aktionstaste ist im Spiel belegt“ prüfte auf QWERTZ die falsche Taste (Y/Z) und Ziffern/F-Tasten gar nicht
- Controller: das Ausblenden einzelner Knöpfe (z. B. Aussteigen) wirkte nicht, wenn das Spiel die erweiterte XInput-Abfrage nutzt
- Abfahrtskontrolle ohne SCS-Eingabegerät: das Standlicht blieb nach der Lichtprüfung an
- Ohne „Verkehr hält an“ lief man durch fahrende Autos, wenn die Verkehrslisten des Spiels nicht gefunden wurden
- ATS-Kontrolle: Pylonen und Warnleuchten zählten als Warndreiecke – verlangt sind drei Dreiecke
- ATS: Tankbelege standen in Menü › Papiere als „l · €“, Bußgelder auf Frachtpapieren in €
- „Auf Standard“ unter Allgemein setzte Updates und Erste Schritte nicht zurück
- Fahrtenschreiber: beim Beenden des Spiels oder Wechsel des Profils fehlten bis zu 10 Spielminuten
- Profil kurz nicht lesbar: Belege, Aufgestelltes und Fahrtenschreiber wechselten auf ein leeres Profil
- Nach einer Pause ruckelte die Maus beim Laufen (die Eingabesperre wurde jedes Bild neu gesetzt)
- Wochenübersicht: der Blick drehte beim Lesen mit, und sie blieb offen, wenn die Mappe weg war
- Aktionsrad: „Papiere“ fehlte, obwohl Ausdrucke, Bescheide oder Führerschein dabei waren
- „Zahlung abgebrochen“ kam auch nach erfolgreicher Kartenzahlung
- „Spieltasten durchlassen“: die Tasten für Papiere und Gurt gingen zusätzlich ans Spiel
- Englisch: Ergebnisse der Abfahrtskontrolle, Tanken, Pause und Road-Trip-Hinweise standen auf Deutsch
- Seltener Absturz beim Auslesen von Spieldaten am Rand eines Speicherbereichs

---

### New

- First steps: the first time you get out, walk, stand at the truck, couple, refuel or handle papers, a card on the right shows the keys you need – each once, right when you need it. Turn it off or start over under menu › General › Help
- Start-up check: after a game update BeyondCab tells you once whether everything works. The check report (BeyondCab\pruefbericht.txt, menu › Game version › Open) lists every game function it checked – handy for a bug report
- Break diary: the folder now holds the tachograph weekly summary – a 24-hour strip per day with driving, work, breaks and rest, the totals, the week against 56 h and anything too long or too short (ATS: 8 days, Hours of Service)

### Fixed

- Tachograph: walking always counted as work (even a break on a bench) and was still credited as a break. Now only coupling, refuelling and signing are work – and in the EU work interrupts the 45-minute break (USA: it counts towards the 30-minute break)
- After loading another save or profile, physics stayed off until the game restarted (no ground, no collision) – it is now searched again
- Keys on arrows, right Ctrl, AltGr etc.: the action key also reached the game despite a hint, passed-through game keys were swallowed
- English keyboards: hints showed "Z" instead of "Y" (key names now follow the active layout)
- Menu › Keyboard: "Action key is bound in the game" checked the wrong key on QWERTZ (Y/Z) and never checked digits or F keys
- Controller: hiding single buttons (e.g. getting out) did not work when the game uses the extended XInput query
- Walk-around check without the SCS input device: the parking lights stayed on after the light check
- With "Traffic stops" off you walked through moving cars when the game's traffic lists were not found
- ATS inspection: cones and beacon lights counted as warning triangles – three triangles are required
- ATS: receipts showed as "l · €" in menu › Papers, fines on shipping papers in €
- "Default" under General did not reset updates and first steps
- Tachograph: up to 10 game minutes were lost when quitting the game or switching profiles
- Profile briefly unreadable: receipts, placed equipment and the tachograph switched to an empty profile
- After a break the mouse stuttered while walking (the input lock was set again every frame)
- Weekly summary: the view turned while reading, and it stayed open when the folder was gone
- Action wheel: "Papers" was missing although printouts, notices or the licence were on you
- "Payment cancelled" also appeared after a successful card payment
- "Pass game keys": the keys for papers and seat belt also reached the game
- English: walk-around check results, refuelling, break and Road Trip hints were in German
- Rare crash when reading game data at the edge of a memory region

## 1.2.3

### Neu

- Update-Schutz: BeyondCab liest die Fahrzeug-Daten von Truck und Anhänger direkt aus dem Spiel ab – verschieben sie sich bei einem Spiel-Update, passt es ohne neue Version. Was nicht mehr passt, schaltet sich gezielt ab, statt falsch zu laufen
- Menü › Allgemein › Spielversion: welche Teile in deiner Spielversion laufen, eingeschränkt oder aus sind – und einmal ein Hinweis nach einem Spiel-Update, wenn etwas aus ist
- Tankbeleg mit dem Preis, den das Spiel an der Säule zeigt, und der Nummer der Säule, an der du stehst
- Einstellungen aufgeräumt: Wegweiser jetzt unter Anzeige, Checkliste beim Kuppeln unter Anhänger
- Klänge aufeinander abgestimmt: Tankdeckel hörbar, Staukasten leiser, Tür innen wie außen, Schritte auf jedem Untergrund gleich laut
- Jeder Klang einzeln einstellbar (Geräusche): Anschnallen, Funkschlüssel, Staukasten und Ausrüstung, Taschenlampe, Kupplungs-Riegel, Papiere – 0 % schaltet ihn aus

### Behoben

- Tanken in 1.62: Säule wieder erkannt, Tankdeckel und Tanken wieder angeboten, das Fenster des Spiels mit Dieselpreis und Kontostand wird beim Laufen ausgeblendet
- Kartenterminal saß an der Dachstütze oder frei auf dem Platz statt an der Zapfsäule
- Plombe saß bei langen Aufliegern im Aufbau statt an den Türen – das Heck kommt jetzt aus der Messung und, wo die nicht geht, aus der Länge des Aufliegers in den Spieldaten
- Plombe musste nach jedem Neustart erneut geprüft werden
- Vier Warnleuchten und die Arbeitsleuchte: das fünfte Licht blieb dunkel
- Mit etwas anderem in der Hand ließ sich ein Gegenstand nicht aufnehmen, ohne Hinweis warum – jetzt „Hände frei machen“
- ATS: Tank-Hinweise zeigten Liter statt Gallonen
- Führerschein: Datum wie der 31.02. wurde angenommen
- „Auf Standard“ setzte nicht alles der Seite zurück (Anschnallen, Papier-Größen, Gurt-Lautstärke, Fahrername)

---

### New

- Update protection: BeyondCab reads the truck and trailer data straight from the game – if a game update moves it, it keeps working without a new version. Anything that no longer fits is switched off on its own instead of misbehaving
- Menu › General › Game version: which parts work, are limited or are off in your game version – plus a one-time note after a game update if something is off
- Fuel receipt with the price the game shows at the pump and the number of the pump you're at
- Settings tidied up: guide arrows now under Display, coupling checklist under Trailer
- Sounds balanced against each other: fuel cap audible, storage box quieter, door the same inside and outside, footsteps equally loud on every surface
- Every sound has its own volume (Sounds): seatbelt, remote key, storage box and equipment, flashlight, coupling catch, papers – 0 % turns it off

### Fixed

- Refuelling in 1.62: the pump is recognised again, fuel cap and refuelling are offered again, the game's window with diesel price and balance is hidden while walking
- The card terminal sat at the canopy pillar or out on the forecourt instead of at the pump
- The seal sat inside the body of long trailers instead of at the doors – the rear now comes from measuring and, where that fails, from the trailer length in the game data
- The seal had to be checked again after every restart
- Four warning beacons and the work light: the fifth light stayed dark
- With something else in your hands an item couldn't be picked up, with no hint why – now "Free your hands"
- ATS: refuelling hints showed litres instead of gallons
- Licence: dates like 31 February were accepted
- "Default" didn't reset everything on the page (seatbelt, paper sizes, seatbelt chime volume, driver name)

## 1.2.2

**Angepasst an ETS2 und ATS 1.62** – 1.61 wird weiter unterstützt.

### Behoben

- Spielversion 1.62: Ankoppeln und Abkoppeln, Stützen kurbeln, Spiralkabel, Anhänger-Licht, aufgestellte Ausrüstung, Lager-Mitarbeiter, Verkehr und das Ausblenden der Ringe am Anhänger funktionieren wieder – SCS hat Fahrzeug-Daten und die Modell-Funktionen umgebaut
- Bett: wurde nicht angeboten, wenn man nach dem Laden im Truck blieb, ohne vorher auszusteigen
- Controller im Truck: der Aktionsknopf ging nur zum Aussteigen – jetzt auch für Fahrerkarte, Beifahrersitz und Bett (und das Spiel sieht ihn dann nicht, z. B. als Warnblinker)

### Hinweis

- In 1.62 hat SCS die Tankstellen-Anzeige umgebaut: der Tankdeckel richtet sich dort wieder nach der Entfernung zur Säule

---

**Updated for ETS2 and ATS 1.62** – 1.61 is still supported.

### Fixed

- Game version 1.62: coupling and uncoupling, cranking the landing gear, coiled cables, trailer lights, placed equipment, the warehouse worker, traffic and hiding the rings at the trailer work again – SCS changed vehicle data and the model functions
- Bunk: wasn't offered if you stayed in the truck after loading without getting out first
- Controller in the truck: the action button only worked for getting out – now also for the driver card, passenger seat and bunk (and the game no longer sees it, e.g. as the hazard lights)

### Note

- In 1.62 SCS rebuilt the gas station display: the fuel cap there follows the distance to the pump again

## 1.2.1

**Echte Schatten für die Ausrüstung, Suche im Menü und Lenkzeiten über das Spielende hinaus.**

### Neu

- Aufgestellte Ausrüstung wirft echte Sonnenschatten wie die Objekte des Spiels – jedes Stuhlbein, jede Strebe der Arbeitsleuchte, mit Schatten auf sich selbst (ETS2 und ATS)
- Suchfeld im Menü: Begriff eingeben (z. B. „Gurt“), Treffer aus allen Seiten, ein Klick führt direkt zur Zeile
- Lenkzeit: Fahrtenschreiber bzw. ELD werden je Profil gespeichert – die Karte bleibt nach einem Neustart gesteckt. Neu auf dem Ausdruck der Wochenwert (ETS2: 56 h Lenkzeit in 7 Tagen, ATS: 70 h Dienst in 8 Tagen), nach 45 bzw. 34 Stunden Ruhe beginnt er neu
- Führerschein: Erwerbsdatum optional selbst eintragen (ETS2 Pkw und Lkw, ATS „CDL seit“), leer bleibt es automatisch
- Probeton: Nach dem Verstellen einer Lautstärke ist sie einmal zu hören

### Verbessert

- Lautstärken einheitlich: 100 % ist die Standard-Lautstärke
- Geburtsdatum in jeder üblichen Schreibweise (z. B. 07.07.2000 auch in ATS)
- Einstellungen, Papiere, Ausrüstung und Fahrtenschreiber werden so gespeichert, dass ein Absturz beim Speichern nichts mehr kaputt macht
- Verkehr: Hupen, die es im Spiel nicht gibt, werden übersprungen – Autos hupen nicht mehr stumm

### Behoben

- Ein- und Aussteigen mit offener Konsole oder einem anderen Fenster vorne: Die Kamera blieb hängen, man steckte in der freien Kamera fest. Jetzt wartet BeyondCab, versucht es erneut und läuft notfalls zu Fuß weiter
- Getipptes in der Konsole zählte als Laufen und Aktionstaste
- Zacken an Tankbeleg, Tacho-Ausdruck und den anderen Zetteln ragten über das Papier
- ATS: beim ELD-Protokoll stand „Polizei“ statt „DOT“

---

**Real shadows for your equipment, search in the menu and driving times that survive a restart.**

### New

- Placed equipment casts real sun shadows like the game's own objects – every chair leg and every strut of the work light, including shadows on itself (ETS2 and ATS)
- Search box in the menu: type a word (e.g. "belt"), results from all pages, one click takes you straight to the row
- Driving time: tachograph and ELD are saved per profile – the card stays inserted after a restart. The printout now shows the weekly total (ETS2: 56 h driving in 7 days, ATS: 70 h on duty in 8 days), which starts over after 45 or 34 hours of rest
- Driving licence: optionally enter when you got it (ETS2 car and truck, ATS "CDL since"); left empty it stays automatic
- Preview sound: after changing a volume you hear it once

### Improved

- Volumes are consistent: 100 % is the default volume
- Date of birth in any common format (e.g. 07.07.2000 in ATS too)
- Settings, papers, equipment and tachograph are saved so that a crash while saving no longer breaks anything
- Traffic: horns that don't exist in the game are skipped – cars no longer honk silently

### Fixed

- Getting in and out with the console or another window open: the camera got stuck and you were left in the free camera. BeyondCab now waits, tries again and if needed lets you keep walking
- Typing in the console counted as walking and the action key
- The torn edges of fuel receipts, tacho printouts and other slips stuck out past the paper
- ATS: the ELD record said "police" instead of "DOT"

## 1.2.0

**Führerschein, Bußgeldbescheide, Gurt und neue Ausrüstung** – dazu eine neue Papiermappe und Modelle, die aussehen wie die Deko des Spiels.

### Neu

- Führerschein (ETS2) bzw. CDL (ATS) mit eigenen Daten und Foto (Profilbild des Spielprofils oder eigenes Bild): Klassen, ADR-Bescheinigung mit Tankkurs, Code 95; in ATS CDL-Klasse, Endorsements und DOT Medical Card – einstellbar unter Papiere › Führerschein
- Prüfungen: Die Polizei prüft bei jeder Kontrolle Klasse und Nachweise, der Blitzer meldet eine fehlende Fahrerlaubnis per Brief, der Verlader gibt ohne gültige ADR-Bescheinigung bzw. Hazmat-Endorsement keine Gefahrgut-Papiere heraus, an Wiegestationen in ATS prüft der DOT-Beamte CDL und Medical Card
- Prüfkarte oben rechts: beim Annehmen eines Auftrags (bei Gefahrgut immer) und wenn der Verlader prüft – was der Auftrag verlangt, mit Haken, Ausrufezeichen oder Kreuz
- Ablaufdaten: ADR-Bescheinigung, Code 95 und Medical Card laufen ab – Erinnerung eine Woche vorher, Verlängern im Menü
- Bußgeldbescheide nach jeder Kontrolle und einige Stunden nach dem Blitzer: in Deutschland nach OWiG mit Gebühr und Auslagen, im Ausland mit Titel in der Landessprache, in ATS als Traffic Citation – die letzten 20 bleiben gespeichert, im Menü unter Papiere und als PDF
- Anschnallen (abschaltbar): Gurt mit J; ohne Gurt ab 25 km/h Warnleuchte und Gong in Intervallen wie im Auto (Lautstärke einstellbar), die Polizei kassiert 30 € bzw. 50 $
- Papiermappe mit Fächern (Auftrag, Unterwegs, Ausweis und Bescheide): Zahl öffnet ein Fach, dann ein Blatt, P geht zurück
- Papiere auch im stehenden Truck bzw. Auto ansehen (P blättert durch); Größe der Papiere einstellbar, zu Fuß und im Fahrzeug getrennt
- Führerschein-Seite im Menü mit Unterseiten (Übersicht, Daten, Klassen, Nachweise): Vorschau der Karte, per Klick groß; Klassen als Kacheln mit Sinnbild; Land bzw. Bundesstaat aus einer Liste; Nachweise mit Gültigkeit und Verlängern in einer Zeile; in ATS erklärt die CDL-Seite jede Klasse und jedes Endorsement
- Frachtbrief bzw. Bill of Lading: deine Firma aus dem Spielprofil (oder ein eigener Name) als Frachtführer, dazu der Fahrername (abschaltbar) – unterschrieben wird als Fahrer
- Papiere als PDF speichern: Frachtbriefe, Tankbelege und Bescheide (Menü › Papiere)
- Erste-Hilfe-Kasten im Staukasten – in ETS2 bei Kontrollen Pflicht
- Arbeitsleuchte: LED-Strahler mit Akku auf einem Dreibein, leuchtet wirklich, an- und ausschaltbar
- Taschenlampe: SOS-Modus (blinkt im Morsetakt), und du wählst, welche Modi beim Halten durchgeschaltet werden
- Ladungssicherung bei der Abfahrtskontrolle je nach Aufbau: Spanngurte, Ketten, Radgurte, Rungen, Twistlocks, Plane, Domdeckel
- Automatische Updates: BeyondCab sucht beim Start nach einer neuen Version und installiert sie auf Wunsch (Menü › Allgemein › Updates)
- Einführung: neue Schritte, in denen du Führerschein bzw. CDL gleich einstellst und Kontrollen, Bescheide und Gurt an- oder abschaltest

### Verbessert

- Staukasten neu: Kacheln mit Symbol, wie viele im Kasten und wie viele draußen stehen
- Eigene Modelle wie die Deko des Spiels: weiche Schattierung in Ecken und Kanten, kaum noch Plastik-Glanz, ruhigere Texturen
- Road Trip: statt eines Klemmbretts liegt die echte Sendung (Umschlag, Aktenkoffer, Paket) neben Absender bzw. Empfänger
- ATS: Begriffe wie in den USA (Bill of Lading, Scale Ticket, Citation, ELD) auch in den Meldungen
- Menü: Pfeile zu Truck, Auflieger und Mitarbeiter als eigener Abschnitt „Wegweiser“, alle Lautstärken unter Geräusche, Auswahllisten mit Kürzel und Namen

### Behoben

- Tasten (Aktion, Taschenlampe, Funkschlüssel, Schnellwahl, Zahlen, PIN am Terminal) reagierten auch, wenn ein anderes Fenster vorne war; Alt+Tab öffnete das Schnellwahl-Rad
- Nach dem Laden eines Spielstands galt der Truck teils noch als abgeschlossen
- Abkoppeln ohne Feststellbremse: Die Bremse, die BeyondCab gezogen hatte, wurde gelöst, während man noch draußen stand
- Road Trip im Auto: Meldung „nicht am ELD angemeldet“, Lkw-Ausrüstung bei der Kontrolle verlangt, Meldungen auf Englisch teils deutsch
- ATS: Hinweis auf schriftliche Weisungen (ADR), die es dort nicht gibt
- Taschenlampe: Lichtkegel schwenkte nach dem Einschalten aus der alten Richtung heran
- Plombe lag bei manchen Aufliegern im Aufbau statt an den Türen
- An Wiegestationen bzw. Kontrollstellen wurde man bei längerem Stehen alle 2 Spielstunden erneut kontrolliert
- Feuerlöscher: Spalt zwischen Standring und Behälter

---

**Driving licence, fine notices, seatbelt and new equipment** – plus a new paper folder and models that look like the game's own decorations.

### New

- Driving licence (ETS2) or CDL (ATS) with your own data and photo (your game profile picture or your own image): classes, ADR certificate with tank course, code 95; in ATS CDL class, endorsements and DOT medical card – set under Papers › Licence
- Checks: police check your class and certificates at every stop, speed cameras report a missing licence by letter, the shipper hands out no dangerous goods papers without a valid ADR certificate or hazmat endorsement, at ATS weigh stations the DOT officer checks CDL and medical card
- Check card at the top right: when you accept a job (always with dangerous goods) and when the shipper checks – what the job requires, with tick, exclamation mark or cross
- Expiry dates: ADR certificate, code 95 and medical card expire – reminder a week before, renew in the menu
- Notices of fine after every check and a few hours after a speed camera: in Germany under the OWiG with fee and expenses, abroad with the title in the local language, in ATS as a traffic citation – the last 20 are kept, in the menu under Papers and as PDF
- Seatbelt (optional): buckle up with J; without it, above 25 km/h a warning light and a chime in intervals like in a car (volume adjustable), the police charge €30 or $50
- Paper folder with sections (Job, On the road, Licence and fines): a number opens a section, then a sheet, P goes back
- View papers while the truck or car is standing (P pages through); paper size adjustable, separately on foot and in the vehicle
- Licence page in the menu with sub-pages (overview, details, classes, certificates): card preview, click to view it large; classes as tiles with symbols; country or state from a list; certificates with validity and renewal in one row; in ATS the CDL page explains every class and endorsement
- Consignment note or bill of lading: your company from the game profile (or a name of your own) as the carrier, plus the driver's name (optional) – you sign as the driver
- Save papers as PDF: consignment notes, fuel receipts and notices (menu › Papers)
- First aid kit in the storage box – required at checks in ETS2
- Work light: battery LED floodlight on a tripod, really lights up, can be switched on and off
- Flashlight: SOS mode (blinks in Morse rhythm), and you choose which modes holding the key cycles through
- Load securing at the departure check depending on the body: straps, chains, wheel straps, stakes, twistlocks, tarp, dome lids
- Automatic updates: BeyondCab checks for a new version at start and installs it if you want (menu › General › Updates)
- Introduction: new steps to set up your licence or CDL right away and to switch checks, notices and seatbelt on or off

### Improved

- New storage box: tiles with icon, how many are in the box and how many are out
- Own models like the game's decorations: soft shading in corners and edges, hardly any plastic shine, calmer textures
- Road Trip: instead of a clipboard the real parcel (envelope, briefcase, box) lies next to the sender or recipient
- ATS: US terms (bill of lading, scale ticket, citation, ELD) in the messages too
- Menu: pointers to truck, trailer and worker in their own "Pointers" section, all volumes under Sounds, pick lists with code and name

### Fixed

- Keys (action, flashlight, remote key, quick menu, numbers, PIN at the terminal) also reacted while another window was in front; Alt+Tab opened the quick menu
- After loading a save the truck sometimes still counted as locked
- Uncoupling without the parking brake: the brake BeyondCab had applied was released while you were still outside
- Road Trip in a car: "not logged in to the ELD" message, truck equipment demanded at checks, some English messages partly German
- ATS: hint about instructions in writing (ADR), which don't exist there
- Flashlight: the beam swung in from the old direction after switching on
- On some trailers the seal sat inside the body instead of at the doors
- At weigh stations and inspection points you were checked again every 2 game hours if you stayed there
- Fire extinguisher: gap between the base ring and the cylinder


## 1.1.0

**ETS2 Walk heißt jetzt BeyondCab** und läuft auch in American Truck Simulator. Das Setup löst die alte Installation ab, Einstellungen und Papiere werden übernommen.

### Neu

- American Truck Simulator 1.61: alles, was es in ETS2 gibt – Aussteigen, Laufen, Kuppeln, Tanken, Papiere, Ausrüstung
- US-Papiere in ATS: Bill of Lading (mit HAZMAT-Kennzeichnung nach 49 CFR), Tankbeleg in Gallonen und Dollar, ELD statt Fahrerkarte, DOT-Kontrolle mit drei Warndreiecken und Feuerlöscher, Pause nach 8 h (Hours of Service)
- Road Trip (ATS): Sendung beim Absender abholen und den Lieferschein unterschreiben, auf den Beifahrersitz legen, am Ziel dem Empfänger übergeben – der Auftrag wird danach automatisch abgeschlossen. Die Sendung ist erst sichtbar, wenn sie im Auto liegt
- Hydraulische Stützen (z. B. Autotransporter): eigene Schritte und Geräusche statt Kurbeln
- Tore und Schranken öffnen sich, wenn du zu Fuß davor stehst (ETS2)
- Neues Logo und neue Symbole im Menü

### Verbessert

- Eigene Figuren (Mitarbeiter, Absender, Empfänger) und aufgestellte Gegenstände werfen jetzt auch zu Fuß Schatten
- Meldungen ersetzen sich sofort, statt sich anzustellen; im Auto steht „Auto“ statt „Truck“
- Funkschlüssel: Fenster fahren beim Abschließen ganz hoch bzw. runter
- „Kuppeln hängt fest?“: Knopf in den Einstellungen setzt den Ablauf am Anhänger zurück

---

**ETS2 Walk is now called BeyondCab** and also runs in American Truck Simulator. The setup replaces the old installation; settings and papers are kept.

### New

- American Truck Simulator 1.61: everything ETS2 has – getting out, walking, coupling, refuelling, papers, equipment
- US papers in ATS: Bill of Lading (with HAZMAT marking per 49 CFR), fuel receipt in gallons and dollars, ELD instead of a driver card, DOT inspection with three warning triangles and a fire extinguisher, break after 8 h (Hours of Service)
- Road Trip (ATS): pick up the parcel from the sender and sign the delivery note, put it on the passenger seat, hand it over to the recipient at the destination – the job then completes by itself. The parcel only shows up once it is in the car
- Hydraulic landing gear (e.g. car transporters): own steps and sounds instead of cranking
- Gates and barriers open when you stand in front of them on foot (ETS2)
- New logo and new icons in the menu

### Improved

- Own figures (worker, sender, recipient) and placed items now cast shadows while you walk
- Messages replace each other at once instead of queueing; in a car it says “car” instead of “truck”
- Remote key: windows now go fully up or down when locking
- “Coupling stuck?”: a button in the settings resets the trailer steps

## 1.0.3

### Neu

- Feuerlöscher im Staukasten: eigenes 3D-Modell (6-kg-Pulverlöscher mit Etikett, Manometer und Schlauch), Pflicht bei Gefahrgut
- Temperaturprotokoll am Kühlaggregat ausdrucken: Messwerte und Kurve seit dem Abholen, liegt in der Papiermappe
- Tagesausdruck am Fahrtenschreiber (oben in der Dachkonsole): Lenk-, Pausen-, Arbeits- und Ruhezeiten der letzten 24 Stunden
- Polizeikontrollen wie im Spiel: Hält dich die Polizei an (zu schnell, Rotlicht, ohne Licht …), prüft sie Frachtbrief, Fahrerkarte und bei Gefahrgut Keil, Warnzeichen und Feuerlöscher und druckt den Tagesausdruck. Blitzer prüfen nichts. Die zufälligen Straßenkontrollen gibt es nicht mehr

### Verbessert

- Taschenlampe in der Hand: neues, genaueres Modell mit Kühlrippen, Reflektor und gerändeltem Griff

---

### New

- Fire extinguisher in the storage box: own 3D model (6 kg powder extinguisher with label, gauge and hose), required for dangerous goods
- Print the temperature record at the reefer unit: readings and curve since pickup, kept in the paper folder
- Daily printout at the tachograph (overhead console): driving, break, work and rest times of the last 24 hours
- Police checks like in the game: when the police stops you (speeding, red light, no lights …), they check the consignment note, driver card and, with dangerous goods, chock, warning signs and fire extinguisher, and print the daily printout. Speed cameras check nothing. The random roadside checks are gone

### Improved

- Flashlight in your hand: new, more detailed model with cooling fins, reflector and knurled grip

## 1.0.2

### Aufträge und Papiere

- Lager-Mitarbeiter mit Warnweste neben dem Auflieger: gibt dir den CMR-Frachtbrief beim Abholen, nimmt ihn am Ziel entgegen und gibt ihn nach dem Entladen quittiert zurück
- Frachtbrief wie der echte: Durchschreibesatz in den echten Farben, Feld 23 selbst mit der Maus unterschreiben und stempeln, Lupe mit der rechten Maustaste; „Parken überspringen“ zählt wie die Übergabe
- Plombe am Heck prüfen (beim Absender und am Ziel), Nummer steht auf dem Frachtbrief
- Eigener Auflieger: Keile an der Rampe, Beladung abwarten, Verladeschein mit Ladungssicherung unterschreiben, danach wird verplombt
- Palettentausch auf dem Frachtbrief: leere Paletten zurück oder Palettenschein
- Wiegeschein bei Tank, Silo und Schüttgut
- Gefahrgut (ADR): UN-Nummer mit Menge auf dem Frachtbrief, Schriftliche Weisungen als echter 4-Seiten-Vordruck mit den echten Gefahrzetteln (Klick blättert)
- Papiermappe auf P: alle Blätter auf einen Blick, Zahl öffnet
- Straßenkontrollen mit Bußgeld: ohne Frachtbrief, bei Gefahrgut ohne Keil und Warnzeichen an Bord, ohne Fahrerkarte
- Menü → Papiere: die letzten 20 Frachtbriefe und 30 Tankbelege, je Profil gespeichert
- Pfeile zum Auflieger und zum Mitarbeiter (abschaltbar)

### Truck und Unterwegs

- Fahrerkarte und Lenkzeit (optional): Karte im Fahrtenschreiber oben in der Dachkonsole stecken, Lenk- und Ruhezeit oben rechts
- Tanken wie in echt: Tankdeckel, an der Säule mit Tankkarte und PIN zahlen, auf Wunsch Kilometerstand, Zapfsäulen-Anzeige und Tankbeleg; bei zwei Tanks ein Beleg
- Kühlauflieger: Kühlgerät als Punkt der Abfahrtskontrolle, mit Anzeige
- Schnellwahl-Rad (Tab halten): Papiere, Taschenlampe, Lampen-Modus, Truck ab-/aufschließen, Ausrüstung, zurück zum Truck
- Funkschlüssel wie ein echter: kurz drücken schließt ab oder auf, am Truck halten fährt die Fenster, weit weg halten findet den Truck (blinkt, hupt, Pfeil)
- Staukasten mit Warndreieck, Unterlegkeilen und Campingstuhl; Keile rasten an den Rädern ein, bei Aufträgen liegen zwei am Auflieger
- Beifahrersitz auch ohne Feststellbremse, auf Wunsch während der Fahrt

### Menü und Bedienung

- Neues Menü wie die Einstellungen am Handy, mit Anleitungen „So funktioniert's“ und einer Einführung beim ersten Start (Allgemein › Hilfe)
- Neuigkeiten jeder Version im Menü unter Allgemein
- Alle Tasten frei belegbar, doppelt belegte werden markiert; Menü mit Strg+F7
- Controller: Y Papiermappe, Steuerkreuz hoch Schnellwahl, Steuerkreuz öffnet Blätter, B legt weg, A blättert, LT Zoom
- Taschenlampe in der Hand sichtbar, Modi Normal, Breit, Weit und Eigen (Feineinstellung)
- Zoom mit der rechten Maustaste, Stärke einstellbar
- Meldungen erscheinen in der Meldungsbox des Spiels; Spiel-Hinweise an der Zapfsäule und beim Kuppeln werden ausgeblendet
- Einstellungen exportieren und importieren
- Neues Setup im Stil des Menüs, kann das Spiel danach gleich starten

### Behoben

- Liege in der Schlafkabine ging nicht, wenn etwas direkt neben dem Truck stand
- Neu belegte Taschenlampen-Taste ging nach dem Neustart verloren
- Pfeiltasten und rechte Strg gehen jetzt auch als Aktions-, Lampen- und Funkschlüssel-Taste; ungültige Werte in der ini werden korrigiert

---

### Jobs and paperwork

- Warehouse worker in a hi-vis vest next to the trailer: hands you the CMR consignment note at pickup, takes it at the destination and gives it back signed after unloading
- Consignment note like the real one: carbon set in the real colours, sign field 23 yourself with the mouse and stamp it, magnifier on the right mouse button; "Skip parking" counts as handing it over
- Check the seal at the rear (at the sender and at the destination), its number is on the consignment note
- Your own trailer: chocks at the dock, wait for loading, sign the loading slip with load securing, then it gets sealed
- Pallet exchange on the consignment note: empty pallets back or a pallet slip
- Weighing ticket for tank, silo and bulk cargo
- Dangerous goods (ADR): UN number with quantity on the consignment note, instructions in writing as the real 4-page form with the real danger labels (click turns the page)
- Paper folder on P: every sheet at a glance, a number opens it
- Roadside checks with fines: no consignment note, no chock and warning signs on board with dangerous goods, no driver card
- Menu → Papers: the last 20 consignment notes and 30 fuel receipts, saved per profile
- Arrows to the trailer and the worker (can be turned off)

### Truck and on the road

- Driver card and driving time (optional): insert the card into the tachograph in the overhead console, driving and rest time at the top right
- Refuelling like the real thing: fuel cap, pay at the pump with fuel card and PIN, optionally the odometer, pump display and fuel receipt; one receipt for two tanks
- Reefers: refrigeration unit as a walkaround check point, with its display
- Quick menu wheel (hold Tab): papers, flashlight, light mode, lock/unlock the truck, equipment, back to the truck
- Remote key like a real one: tap to lock or unlock, hold at the truck for the windows, hold far away to find the truck (flashes, honks, arrow)
- Storage box with warning triangle, wheel chocks and camping chair; chocks snap to the wheels, with jobs two sit at the trailer
- Passenger seat also without the parking brake, optionally while driving

### Menu and controls

- New menu like the settings on a phone, with "How it works" guides and an introduction on first start (General › Help)
- What's new in each version in the menu under General
- Every key can be rebound, keys used twice are marked; menu on Ctrl+F7
- Controller: Y paper folder, d-pad up quick menu, d-pad opens sheets, B puts away, A turns pages, LT zoom
- Flashlight visible in your hand, modes normal, wide, far and custom (fine tuning)
- Zoom with the right mouse button, adjustable strength
- Messages appear in the game's notification box; game hints at the fuel pump and when coupling are hidden
- Export and import settings
- New setup in the style of the menu, can start the game right after

### Fixed

- The bunk in the sleeper cab could not be used with something right next to the truck
- A rebound flashlight key was lost after restarting
- Arrow keys and right Ctrl now also work as action, flashlight and remote key; invalid values in the ini are corrected

## 1.0.1

**Erste Veröffentlichung**

- Laufen in der Ich-Sicht mit Physik-Boden, Kollision, Schritten je Untergrund und Verkehr, der vor dir hält
- Beifahrersitz und Bett in Schlafkabinen, Schlafen über den Schlaf-Dialog des Spiels
- Auflieger von Hand ab- und ankuppeln mit Checkliste, Schlepptest und optionalen Zusatzschritten
- Abfahrtskontrolle, Tanken an der Zapfsäule, Funkschlüssel mit Fenstern und Follow-me-home
- Warnleuchten und Pylonen aus dem Staukasten, die umkippen, wenn ein Fahrzeug dagegen fährt
- Pause auf Bänken, Taschenlampe, Controller-Unterstützung, Menü auf Deutsch und Englisch
- Setup mit Deinstallation; Einstellungen und Daten in `Dokumente\Euro Truck Simulator 2\ETS2 Walk`

---

**First release**

- First-person walking with physics ground, collision, surface-dependent footsteps and traffic that stops for you
- Passenger seat and bed in sleeper cabs, sleeping through the game's sleep dialog
- Uncouple and couple the trailer by hand with a checklist, tug test and optional extra steps
- Walkaround check, refuelling at the pump, remote key with windows and follow-me-home
- Warning lights and traffic cones from the storage box that tip over when a vehicle hits them
- Breaks on benches, flashlight, controller support, menu in German and English
- Setup with uninstaller; settings and data in `Documents\Euro Truck Simulator 2\ETS2 Walk`
