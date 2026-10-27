<div align="center">

<img src="bilder/icon.png" width="112" alt="BeyondCab">

# BeyondCab

**Raus aus der Kabine.**<br>
Aussteigen, um den Truck gehen, von Hand kuppeln, Papiere unterschreiben, tanken und Pause machen – zu Fuß und aus der Ich-Sicht in **Euro Truck Simulator 2** und **American Truck Simulator**.

[![Version](https://img.shields.io/github/v/release/Ku3rb1s/BeyondCab?label=Version&color=ff9500)](../../releases/latest)
![Windows 10/11](https://img.shields.io/badge/Windows-10%20%7C%2011-1f6feb)
![ETS2 und ATS](https://img.shields.io/badge/Spiele-ETS2%20%7C%20ATS-34c759)
![Kostenlos](https://img.shields.io/badge/kostenlos-ohne%20Konto-ff9f0a)

### [⬇&nbsp; BeyondCab herunterladen](../../releases/latest)

[English](README.md) · Deutsch

<img src="bilder/einstellungen-de.png" alt="BeyondCab im Spiel: Einstellungsmenü" width="900">

</div>

## Was dich erwartet

🚶 **Zu Fuß unterwegs** – Aussteigen, wenn die Feststellbremse gezogen ist, gehen, rennen, springen, ducken. Der Boden kommt aus der Physik des Spiels, Schritte klingen je nach Untergrund, der Verkehr bremst vor dir, Tore gehen auf, wenn du davorstehst.

🔗 **Auflieger von Hand kuppeln** – Leitungen lösen, Keile anlegen, Stützen kurbeln (oder hydraulisch fahren), Königszapfen ziehen – und alles wieder zurück. Mit Checkliste, Schlepptest und Abfahrtskontrolle rund um den Zug.

📄 **Papiere wie in echt** – In ETS2 der CMR-Frachtbrief vom Lager-Mitarbeiter, in ATS die Bill of Lading. Selbst unterschreiben und stempeln, am Ziel quittiert zurück. Dazu Plombe, Wiegeschein, Gefahrgut-Papiere, Fahrerkarte bzw. ELD und Polizei- bzw. DOT-Kontrollen.

⛽ **Tanken mit Karte** – Tankdeckel auf, Karte ins Terminal, PIN, an der Säule zählen Betrag und Liter (in ATS Gallonen und Dollar) mit, danach gibt es einen Beleg.

📦 **Road Trip (ATS)** – Bei Kurieraufträgen holst du die Sendung beim Absender ab, legst sie auf den Beifahrersitz und übergibst sie am Ziel dem Empfänger – mit Lieferschein.

🔦 **Und noch mehr** – Funkschlüssel mit Fenstern und Truck-Finder, Taschenlampe, Warnleuchten und Unterlegkeile aus dem Staukasten, Bänke zum Pause machen, Schlafen in der Kabine, Controller-Unterstützung.

## In 3 Schritten startklar

1. **[Herunterladen](../../releases/latest)** und `BeyondCab-Setup-….exe` starten – das Setup findet ETS2 und ATS selbst und installiert in beide.
2. **Spiel starten** und einmal bestätigen, dass es SDK-Plugins laden darf.
3. **Anhalten, Feststellbremse ziehen, E drücken** – du stehst neben dem Truck. Das Menü öffnest du mit Strg + F7.

Am Spiel selbst wird nichts verändert: keine Mods in den Spieldateien, keine Änderung an der `config.cfg`.

## Bilder

| | |
|---|---|
| ![Frachtbrief](bilder/frachtbrief-de.png) | ![Bill of Lading](bilder/bill-of-lading.png) |
| CMR-Frachtbrief (ETS2), quittiert | Bill of Lading mit HAZMAT (ATS) |
| ![Papiermappe](bilder/papiermappe-de.png) | ![Schnellwahl](bilder/schnellwahl-de.png) |
| Papiermappe (P) | Schnellwahl-Rad (Tab halten) |
| ![Tanken](bilder/tanken-de.png) | ![Tanken in den USA](bilder/tanken-us.png) |
| Tankbeleg, Kartenterminal und Zapfsäule | Dasselbe in ATS: Gallonen und Dollar |
| ![Schriftliche Weisungen](bilder/weisungen-de.png) | ![ELD](bilder/eld.png) |
| Schriftliche Weisungen nach ADR | ELD-Protokoll (ATS) |

## Voraussetzungen

- Windows 10 oder 11 (64 Bit)
- Euro Truck Simulator 2 **1.61** und/oder American Truck Simulator **1.61** über Steam, Einzelspieler
- Nach einem Spiel-Update kann es sein, dass einzelne Funktionen ausfallen, bis eine neue Version erscheint. Das Plugin prüft beim Start, ob die Stellen im Spiel noch passen, und schaltet sonst nur den betroffenen Teil ab

---

## Alles im Detail

<details>
<summary><b>Laufen</b></summary>

- Aussteigen mit der Aktionstaste, wenn die Feststellbremse gezogen ist. Die Tür geht auf, du stehst neben dem Truck – auch auf der Beifahrerseite
- Gehen, Rennen, Springen, Ducken. Bergauf langsamer, leichtes Kopfwippen, Körpergröße einstellbar
- Der Boden kommt aus der Physik des Spiels: Gehwege, Rampen, Treppen, Laderampen. Leitplanken, Zäune und Fahrzeuge halten dich auf
- Schritte klingen je nach Untergrund (Asphalt, Kies, Gras, Metall, Schnee, Holz)
- Der KI-Verkehr bremst vor dir und hupt, wenn du zu lange auf der Straße stehst
- Tore und Schranken an Firmengeländen gehen auf, wenn du davorstehst (ETS2)
- Pfeile oben im Bild zeigen auf Wunsch, wo Truck, Auflieger und Lager-Mitarbeiter stehen

</details>

<details>
<summary><b>Im Truck</b></summary>

- Auf den Beifahrersitz wechseln oder dich in einer Schlafkabine aufs Bett legen. Ob dein Truck ein Bett hat, erkennt das Plugin selbst
- Auf dem Bett: Taste halten zum Schlafen (über den Schlaf-Dialog des Spiels)
- Am Beifahrersitz und auf dem Bett klingt es wie in der Kabine, nicht wie draußen
- Lenkzeit (optional): In ETS2 steckst du zu Schichtbeginn die Fahrerkarte in den Fahrtenschreiber, in ATS meldest du dich am ELD an. Oben rechts siehst du Lenk- und Ruhezeit, am Gerät druckst du den Tagesausdruck bzw. das ELD-Protokoll

</details>

<details>
<summary><b>Auflieger von Hand kuppeln</b></summary>

- Abkoppeln: Luft- und Stromleitungen lösen, Unterlegkeile anlegen, Stützen runterkurbeln, Königszapfen-Hebel ziehen
- Ankoppeln: unterfahren, Sattelkupplung prüfen, Leitungen anschließen, Stützen hochkurbeln, Keile entfernen. Danach Schlepptest
- Hydraulische Stützen (zum Beispiel am Autotransporter) fährst du per Knopf statt zu kurbeln – mit eigenen Schritten und Geräuschen
- Optional mehr Schritte: Sicherung am Kupplungshebel, Anhänger-Feststellbremse (roter Knopf), Beleuchtung prüfen
- Eine Checkliste zeigt, was als Nächstes dran ist. Hängt einmal etwas fest, setzt „Kuppeln hängt fest?“ im Menü den Ablauf zurück
- Nach dem Ankuppeln einmal um Truck und Auflieger gehen: Reifen, Licht, Ladung und Türen, beim Kühlauflieger das Kühlgerät

</details>

<details>
<summary><b>Aufträge und Papiere</b></summary>

- Bei jedem Auftrag steht ein Lager-Mitarbeiter neben dem Auflieger und gibt dir die Papiere: in ETS2 der CMR-Frachtbrief im Durchschreibesatz, in ATS die Bill of Lading – mit Firmen, Städten, Ladung, Gewicht und Kennzeichen aus dem Auftrag
- Du unterschreibst selbst mit der Maus und drückst deinen Stempel drauf. Name und Ort stellst du im Menü ein
- Am Ziel gibst du sie beim Mitarbeiter ab, nach dem Entladen bekommst du sie quittiert zurück. „Parken überspringen“ zählt wie die Übergabe
- Verplombte Auflieger, eigener Auflieger mit Verladeschein, Palettentausch (ETS2), Wiegeschein bei Tank, Silo und Schüttgut
- Gefahrgut: in ETS2 nach ADR mit Schriftlichen Weisungen, in ATS nach 49 CFR mit HAZMAT-Kennzeichnung und ERG-Leitfaden
- Polizei- bzw. DOT-Kontrollen: Hält dich die Polizei an, prüft sie Papiere, Fahrerkarte bzw. ELD und bei Gefahrgut die Ausrüstung. Was fehlt, kostet ein Bußgeld
- Kühlauflieger: Am Kühlaggregat druckst du das Temperaturprotokoll aus
- Alles steckt in der Papiermappe (P), die letzten Papiere liegen im Menü unter Papiere

</details>

<details>
<summary><b>American Truck Simulator</b></summary>

BeyondCab erkennt von selbst, welches Spiel läuft – es gibt nichts auszuwählen.

- Bill of Lading statt CMR, Bundesstaaten statt Länder, Datum im US-Format
- Tanken in Gallonen und Dollar, Kilometerstand in Meilen
- ELD statt Fahrerkarte, Pause nach 8 Stunden Lenkzeit (Hours of Service), DOT-Kontrolle mit drei Warndreiecken und Feuerlöscher
- Eigene Modelle für Warnleuchte, Warndreieck und Leuchtpunkt
- **Road Trip**: Bei Kurieraufträgen mit dem Auto holst du Umschlag, Aktenkoffer oder Paket beim Absender ab und unterschreibst den Lieferschein, legst die Sendung auf den Beifahrersitz und übergibst sie am Ziel dem Empfänger. Danach ist der Auftrag automatisch abgeschlossen. Die Sendung erscheint erst im Auto, wenn du sie hingelegt hast

</details>

<details>
<summary><b>Tanken</b></summary>

- Ablauf wie in echt: Tankdeckel öffnen, zur Säule, Tankkarte rein, PIN eintippen (im Menü einstellbar), auf Wunsch Kilometerstand, dann am Deckel tanken. Bei großem Tank geht es auf beiden Seiten
- Die Anzeige der Säule zählt Betrag und Menge mit, danach gibt es einen Beleg mit dem Preis des Landes bzw. Bundesstaats, Kennzeichen und Kilometerstand

</details>

<details>
<summary><b>Funkschlüssel, Ausrüstung und mehr</b></summary>

- Funkschlüssel: ab- und aufschließen mit Blinkern und auf Wunsch kurzem Hupen, am Truck halten für die Fenster, weit weg halten zum Finden. Follow-me-home und automatisches Abschließen
- Im Staukasten hinter der Kabine: Warnleuchten, Pylonen, Warndreieck, Unterlegkeile, Feuerlöscher und ein Campingstuhl. Rausnehmen, aufstellen, wieder einsammeln
- Schnellwahl-Rad (Tab halten), Bänke an Rastplätzen zum Pause machen
- Taschenlampe in der Hand oder am Kopf, mit mehreren Modi
- Controller mit Xbox- oder PlayStation-Symbolen, alle Knöpfe frei belegbar
- Einführung beim ersten Start, Einstellungen exportieren und importieren, Deutsch und Englisch

</details>

<details>
<summary><b>Bedienung</b></summary>

| Taste | Controller | Was |
|---|---|---|
| E | X | Aktion: aussteigen, einsteigen, tanken, kuppeln, Papiere … (halten, wo angezeigt) |
| W A S D | linker Stick | laufen |
| Shift | RT | rennen |
| Leertaste | A | springen |
| Strg | B | ducken |
| T | LB | Taschenlampe (halten: Modus wechseln) |
| K | RB | Funkschlüssel: kurz ab-/aufschließen, am Truck halten: Fenster, weiter weg halten: Truck finden |
| P | Y | Papiermappe; darin öffnen 1–4 (Controller: Steuerkreuz) ein Blatt |
| Tab (halten) | Steuerkreuz hoch | Schnellwahl |
| rechte Maustaste | LT | Zoom, auf Papieren die Lupe |
| Strg + F7 | – | Menü |
| Strg + Alt + Z | Back (halten) | zurück zum Truck |

Alle Tasten und Knöpfe lassen sich im Menü unter **Tastatur** bzw. **Controller** umlegen.

</details>

<details>
<summary><b>Einstellungen und Daten</b></summary>

Töne und Listen (Bänke, Tankstellen, Parkplätze) stecken in der DLL. In `Dokumente\<Spiel>\BeyondCab\` liegen nur deine Einstellungen (`beyondcab.ini`), was du aufgestellt hast, deine Papiere und die eigenen Modelle (`models\`, legt das Plugin selbst an).

Eigene Töne: Eine Datei mit demselben Namen in `BeyondCab\sounds\` ersetzt den eingebauten Ton (zum Beispiel `truck_lock.wav`).

Im Spiel-Log (`Dokumente\<Spiel>\game.log.txt`) stehen alle Meldungen des Plugins mit `[BeyondCab]` davor. Bei Problemen hilft diese Datei weiter.

</details>

<details>
<summary><b>Häufige Fragen</b></summary>

**Windows warnt beim Start des Setups („Der Computer wurde durch Windows geschützt“).**
Die Datei ist nicht digital signiert. Auf „Weitere Informationen“ und „Trotzdem ausführen“ klicken. Wer sichergehen will, vergleicht die Prüfsumme mit der `SHA256SUMS.txt` im Release:

```powershell
Get-FileHash .\BeyondCab-Setup-*.exe -Algorithm SHA256
```

**Ich kann nicht aussteigen.** Erst anhalten und die Feststellbremse ziehen. Das lässt sich im Menü unter **Truck** abschalten.

**Das Menü erscheint nicht.** Prüfe im Spiel-Log, ob `[BeyondCab]` auftaucht. Wenn nicht, liegt die DLL nicht im richtigen Ordner oder die SDK-Meldung beim Start wurde abgelehnt.

**Ich will keinen Papierkram.** Frachtpapiere, Tankkarte, Unterlegkeile bei Aufträgen und Fahrerkarte bzw. ELD lassen sich im Menü einzeln abschalten.

**Ich habe noch „ETS2 Walk“ (1.0.x).** Einfach das neue Setup starten. Es entfernt die alte `ets2_walk.dll`, Einstellungen und Papiere ziehen in den Ordner `BeyondCab` um.

**Funktioniert es mit TruckersMP?** Nein, nur im Einzelspieler.

**Verträgt es sich mit CabPlay?** Ja, beide Plugins laufen zusammen.

</details>

<details>
<summary><b>Deinstallieren</b></summary>

Windows-Einstellungen → **Apps** → BeyondCab → Deinstallieren, oder das Setup erneut starten und **Entfernen** wählen. Das Spiel muss geschlossen sein. Entfernt wird das Plugin in beiden Spielen, auf Wunsch kommen Einstellungen und Papiere in den Papierkorb.

</details>

<details>
<summary><b>Lizenzen und Danke</b></summary>

- Teile zum Lesen des Spielspeichers stammen aus dem [ETS2LA-Spielplugin](https://github.com/ETS2LA/plugin) (MIT)
- [Dear ImGui](https://github.com/ocornut/imgui) (MIT), [MinHook](https://github.com/TsudaKageyu/minhook) (BSD-2), SCS Telemetry SDK, NVIDIA PhysX 3.4 (Header, BSD-3)
- Lesen der Spielarchive nach dem Kartenparser von [truckermudgeon/maps](https://github.com/truckermudgeon/maps), CityHash von Google (MIT)
- Gefahrzettel: gemeinfreie Zeichnungen von [Wikimedia Commons](https://commons.wikimedia.org/wiki/Category:Diagrams_of_ADR_markings)
- Geräusche: [Kenney](https://kenney.nl) (CC0) und Aufnahmen von [Pixabay](https://pixabay.com) (Pixabay-Lizenz, nur zusammen mit dem Plugin weitergeben)
- Entwickelt mit [Claude Code](https://claude.com/claude-code) (Anthropic): Den Code hat Claude geschrieben, nach Ideen, Vorgaben und Tests im Spiel von Ku3rb1s

</details>

---

<sub>Fan-Projekt, nicht verbunden mit SCS Software. Die Marken gehören ihren Inhabern. Früher „ETS2 Walk“. Alle Änderungen: [CHANGELOG](CHANGELOG.md)</sub>
