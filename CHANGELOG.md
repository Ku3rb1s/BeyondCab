# Änderungen · Changelog

## 1.4.4

### Neu

- **Русский**: Russisch in der Sprachauswahl (Automatisch bei russischem Windows) – Übersetzung von **boss-22-boss** (Issue #7), vielen Dank! Die Sprachauswahl hat jetzt eine eigene Zeile

### Behoben

- **Keine Taste ging** (Issue #6, wohl auch #5): Steht in der `config.cfg` des Spiels `uset g_console_state "1"`, hielt BeyondCab die Konsole für offen und nahm weder Strg + F7 noch E noch die Controller-Taste an. Jetzt zählt dieser gespeicherte Wert erst, wenn die Konsole einmal geschlossen wurde
- Der Hinweis „Entwicklerkamera aus“ kam auch, wenn die `config.cfg` gar nicht gelesen werden konnte; jetzt nur noch, wenn die Zeilen wirklich auf 0 stehen – und erst im laufenden Spiel, 15 Sekunden lang
- Menü in 1440p/4K: Klicks direkt nach einer Mausbewegung landeten manchmal daneben
- Russisch/Chinesisch: Status der Papiere (bezahlt, abgelaufen …) wieder farbig, abgelaufene Nachweise rot; lange Texte nicht mehr abgeschnitten; die US-Bill-of-Lading bleibt englisch; Wochentage, Ländernamen und Sätze mit Tasten jetzt übersetzbar
- Abschnitt „Papiere“ unter Anzeige stand im englischen Menü deutsch
- Log: lange Mod-Listen vollständig, ignorierte Tasten mit Grund, weniger doppelte Zeilen
- **Benutzername mit kyrillischen oder chinesischen Zeichen** (oder OneDrive-Dokumente): BeyondCab fand das Spielprofil nicht – Papiere, Pannenkit und Fahrtenschreiber wurden nie gespeichert, Einstellungen landeten im Plugin-Ordner und die eigenen Modelle (Warnleuchte, Keile …) fehlten. Die bisherigen Einstellungen und Papiere aus dem Plugin-Ordner werden beim ersten Start übernommen
- **Blitzer**: Ein noch ausstehender Bescheid wurde nach einem Profilwechsel im anderen Profil abgebucht
- **Fahrtenschreiber**: Nach dem Laden eines älteren Spielstands blieben Lenkzeit, Pause und Karte auf dem späteren Stand – eine Kontrolle konnte dann zu Unrecht Bußgeld verlangen bzw. Verstöße übersehen
- Maut- und Fährbeleg nannten nach dem Abkoppeln noch den Auflieger
- Konsole: Mit gespeichertem `g_console_state "1"` zählt jetzt auch das erste Öffnen der Konsole (Tippen löst nichts aus)
- Beenden während eines Update-Downloads stürzt nicht mehr ab; lange Fotopfade in den Einstellungen zerschießen die ini nicht mehr
- **Festgesteckt beim Laufen**: Wechselte die Kamera (z. B. Spielstand aus dem Esc-Menü geladen), blieb die Tastatur gesperrt – jetzt endet das Laufen nach 1,5 s von selbst
- **Tasten blieben im Spiel „gedrückt“**: Loslassen geht jetzt immer ans Spiel – vorher fuhr der Truck z. B. weiter, wenn man beim Gasgeben das Menü öffnete, oder Strg hing nach Strg + F7
- Nach einer Abschaltung von BeyondCab (Speicherfehler) bleiben Controller, Esc, Verkehr und Taschenlampe nicht mehr blockiert
- Aussteigen/Einsteigen gibt bei hohen Bildraten nicht mehr nach 0,3 s auf (jetzt 2 s)
- Nach dem Laden eines anderen Spielstands: Boden und Kollision beim nächsten Aussteigen sauber neu, Beifahrersitz/Liege zurück, keine unsichtbaren Wände
- Über einer echten Kante (Kai, Parkdeck) schwebt man nicht mehr endlos – das Halten auf Brückenhöhe endet nach 25 m
- Profilwechsel bzw. älterer Spielstand: Papiere, Aufgestelltes und Fahrtenschreiber des alten Profils werden nicht mehr gekürzt; derselbe Auftrag aus einem älteren Spielstand lädt den Frachtbrief richtig
- Nach dem Übermüdungs-Bußgeld des Spiels kommt bei der Kontrolle nicht noch „Ruhezeit überzogen“ dazu
- Ausrüstung: kein falsches Modell mehr an einem wiederverwendeten Platz, kein Absturzrisiko beim Wegräumen während des Zeichnens; Alt+Tab mitten im Funkschlüssel lässt Shift/Strg nicht mehr hängen
- Menü: Öffnen/Schließen mit Strg + F7 konnte selten abstürzen; Regler ziehen ruckelt nicht mehr (gespeichert wird beim Loslassen); „Alle Einstellungen zurücksetzen“ behält Name, Anschrift, PIN und Führerschein und startet die Einführung nicht neu; eine Taste wird nicht mehr versehentlich belegt, wenn man nach „Ändern“ das Menü schließt oder in der Suche tippt
- Einstellungen: zwei gleichzeitige Speichervorgänge konnten die ini beschädigen
- Installer: schlug das Schreiben bei einem der beiden Spiele fehl, blieb die Installation halb; jetzt werden beide versucht (mit Wiederholung) und das Erfolgreiche eingetragen
- Stabilität: Fahrzeugpositionen, Blitzer-Bescheid und Physik-Suche ohne gleichzeitigen Zugriff; Beenden des Spiels während einer Suche oder mitten im Zeichnen stürzt nicht mehr ab; beschädigte Spielarchive bringen das Spiel nicht mehr zum Absturz
- Nach einem Spiel-Update: die Feststellbremse wird nur noch gesetzt, wenn ihr Speicherwert nachweislich zum Spiel passt
- **Spielstand geladen**: das Pannenkit wurde nicht mehr fälschlich als „in der Werkstatt aufgefüllt“ bezahlt, der Pannendienst rechnet keine Reparatur aus dem verworfenen Spielverlauf mehr ab, es entsteht keine falsche Abschlepprechnung und Tanken vor und nach dem Laden landet nicht mehr auf einem Beleg
- Pannenkit: die Sperre „Auflieger schon geflickt“ geht beim Neustart des Spiels nicht mehr verloren
- Schlafen: blieb der Schlaf-Dialog länger als 3 Minuten offen, gingen danach beim Laufen Tasten ans Spiel
- Profilwechsel: die eigene Bus-Türtaste wird neu gelesen, der unterschriebene Frachtbrief des vorigen Profils liegt nicht mehr bereit
- Das Fensterheber-Geräusch lief endlos, wenn eigene Töne währenddessen ausgeschaltet wurden
- **Blitzer**: Nach dem Laden eines etwas älteren Spielstands kam der Bescheid für ein Foto, das es dort nie gab, trotzdem – mit Abbuchung
- **Fähre**: Der Rundgang am Hafen galt nach dem Laden eines älteren Spielstands bzw. nach einem Profilwechsel weiter; eine Überfahrt aus dem anderen Profil konnte im neuen abgerechnet werden
- Wiegestation: ein gerade gemeldetes Bußgeld des Spiels wurde von der Kontrolle überschrieben (auch die doppelte Ruhezeit-Strafe kam so zurück)
- Papiere: ein älterer Spielstand direkt nach dem Spielstart entfernte die späteren Belege nicht; die zweite Tankseite überschrieb nach dem Löschen des ersten Belegs den Beleg der vorigen Tankstelle; Russisch: Status „quittiert“ und „Polizei“ wieder farbig
- **Frachtbrief nach Abbrechen/Liefern und Neuladen**: Lud man nach dem Abbrechen (oder Liefern) einen Spielstand von davor, waren die schon genommenen Papiere weg – die nächste Kontrolle verlangte Bußgeld für den fehlenden Frachtbrief, die Lieferung lief „unter Vorbehalt“
- Nach dem Laden eines älteren Spielstands: kein halber Kuppel-Ablauf mehr am frisch geladenen Auflieger (sonst kam gleich der Hebel), Tacho-Ausdruck, Tankbeleg sowie Maut- und Fährbeleg aus dem verworfenen Verlauf weg; der Funkschlüssel-Zustand „abgeschlossen“ verhindert das Einsteigen nach dem Laden nicht mehr
- Einsteigen: ein verzögertes Einsteigen (Tür zuerst, Bustüren) zieht einen nicht mehr in die Kabine, wenn man inzwischen weggegangen ist oder das Laufen schon beendet war
- Sitzwechsel: wechselte man währenddessen auf eine Außenkamera, blieb die Maus eingefroren; Esc beim Tanken lässt die Enter-Taste nicht mehr gedrückt
- Pannenkit: nach dem Laden eines älteren Spielstands gilt wieder der Inhalt von damals (vorher blieb ein bezahltes Auffüllen bzw. ein Verbrauch bestehen); Busfahrplan: keine Ankunftszeiten mehr aus dem verworfenen Verlauf
- **Unterlegkeile beim Profilwechsel**: der Auftrag des neuen Profils wurde noch dem alten zugerechnet – dort verschwanden Keile bzw. kamen beim Zurückwechseln doppelt an den Auflieger; beim Spielstart mit laufendem Auftrag wurden fehlende Keile nicht mehr gestellt
- **Funkschlüssel**: nach einer Abschaltung von BeyondCab (Speicherfehler) bzw. beim Beenden blieben vom Schlüssel gedrückte Tasten (Shift, Hupe, Fenster) unten; Alt+Tab beim Halten ließ die Fenster weiterfahren
- Eine Aktionstaste (z. B. E zum Aussteigen), die man nach dem Auslösen noch hält, kommt nicht mehr doch beim Spiel an
- Ausrüstung: konnte ein Modell nicht platziert werden, blieb es belegt (konnte das Beenden aufhalten)
- Menü: Mausbewegung bei offenem Menü und das Zeichnen griffen ohne Absprache auf dieselbe Eingabe-Liste zu (mögliche Abstürze); PIN der Tankkarte nimmt nur noch Ziffern (mit „.“ oder „-“ wurde die Karte an jeder Säule abgelehnt); Namen und Anschrift fassen jetzt auch auf Russisch/Chinesisch die volle Länge; Tasten-Erfassen belegt nicht mehr versehentlich F7/O vom Menü-Kürzel, Controller-Knopf-Erfassen endet beim Seitenwechsel
- Entfernen (Setup): ließ sich die DLL nicht löschen, hieß es trotzdem „entfernt“ und der Eintrag unter Apps war weg – jetzt Meldung mit der Datei, der Eintrag bleibt. Update aus dem Spiel: geht in den selbst gewählten Spielordner statt in eine andere (Steam-)Kopie
- Schlägt ein Update aus dem Spiel fehl, meldet BeyondCab das beim nächsten Start (vorher blieb man unbemerkt auf der alten Version)
- **Niedrige Bildrate**: unter etwa 14 fps schaukelte der Kopf nach einer Landung stark, unter etwa 11 fps konnte die Kamera ganz kaputtgehen – jetzt stabil
- Brücke ohne Fahrbahn: das Halten auf Truck-Höhe galt beim nächsten Aussteigen an einer anderen Brücke noch als „verbraucht“ – man fiel durch
- Strg + F7 sperrt Maus und Tastatur nicht mehr, wenn das Menü gar nicht angezeigt werden kann; Sitz-Sendungssuche braucht nicht mehr Hunderte MB Speicher
- **Ziffernblock**: auf „Num 0“ … „Num 9“ gelegte Tasten gingen bei eingeschaltetem NumLock nicht; Pfeiltasten, Einfg/Entf, Pos1/Ende und Bild auf/ab werden beim Belegen als die richtigen Tasten erkannt (vorher als Ziffernblock)
- Kuppeln: liegt „Ankuppeln“ im Spiel auf Strg/Alt/Shift + Taste, sagt BeyondCab jetzt, dass es die Taste ohne Modifikator braucht (sonst kam „Zustand nicht erreicht“); eine Modifikator-Belegung für den Controller gilt nicht mehr für die Tastatur-Taste
- Funkschlüssel nach einer Abschaltung: auch die Fensterheber werden losgelassen
- **Wegfahren nach dem Abkoppeln**: die Fahrsperre („Stützen unten“/„Luftleitungen ab“) hielt auch nach einem echten Abkoppeln die Feststellbremse fest, solange der Zapfen noch in der Platte stand – man kam vom abgestellten Auflieger nicht weg
- Controller: ein beim Einsteigen noch gehaltener Knopf (z. B. X) löste im Spiel nicht mehr seine Funktion aus (Warnblinker); leere Controller-Plätze werden nur noch alle 2 s abgefragt
- `beyondcab.ini` von Hand: Leerzeichen um „=“ und `true`/`yes`/`on` werden verstanden; bei doppelten Zeilen in der `config.cfg` gilt wie im Spiel die letzte
- Taschenlampe: blieb das echte Licht nach einem Ladebildschirm oder einer Fähre mit eingeschalteter Lampe für die ganze Sitzung aus (nur noch der Bildschirm-Effekt), geht es jetzt weiter
- PDF-Export: chinesische Titel mit bestimmten Zeichen (z. B. 不) standen in den Dokument-Eigenschaften falsch; Führerschein mit Geburtstag 29.02. zeigt kein unmögliches Ablaufdatum mehr; Russisch: Kuppel-Meldungen nicht mehr am Ende abgeschnitten
- **Fahrtenschreiber**: nach der ersten 45-Minuten-Pause reichten danach immer 30 Minuten (die volle Pause galt als „erste 15“); derselbe Lenkzeit-Verstoß einer noch laufenden Schicht wurde bei jeder weiteren Kontrolle erneut bestraft; eine geteilte Tagesruhe mit erstem Teil von 7 bis 9 h (erlaubt, wenn der zweite Teil von 9 h innerhalb von 24 h folgt) wurde sofort als „Ruhezeit zu kurz“ bestraft
- Frachtbrief: ein Spielstand von vor der Übergabe beim Empfänger ließ den Brief „abgegeben“ – danach kam kein Mitarbeiter und keine Übergabe mehr; Vermerke beim Quittieren erscheinen nicht mehr doppelt; der Frachtbrief einer Road-Trip-Sendung bleibt nach Abbruch nicht mehr offen in der Mappe
- Halten-Aktionen: schwenkte man mit gehaltener Taste zum nächsten Prüfpunkt, war er in Sekundenbruchteilen „fertig“, und bei der Licht-Prüfung gingen die Leuchten nicht an („Rückleuchten dunkel“); vom vorigen Schritt herübergeschwenkt, fing das Tanken nicht mehr von selbst an
- Tankkarte: die Zahlung an einer Säule galt nach dem Wegfahren weiter – Tage später an derselben Säule wurde ohne Karte getankt
- Profilwechsel: in ein Profil mit späterer Spielzeit buchte der Fahrtenschreiber den Sprung als Ruhe ins vorige Profil; ein Bus- bzw. Road-Trip-Auftrag des neuen Profils ging verloren bzw. der des alten blieb; ein halber Kuppel-Ablauf wird zurückgesetzt. Werkstattbesuch nach über 24 h Fahrt setzt Sitz und Physik nicht mehr zurück
- Laden eines **neueren** Spielstands mit demselben Truck wird jetzt erkannt (am Sprung des Kilometerstands): Funkschlüssel-Sperre, Pannendienst und Tankstopp gelten danach nicht mehr weiter

---

### New

- **Русский**: Russian in the language selection (Auto on a Russian Windows) – translation by **boss-22-boss** (issue #7), thank you! The language selector now has its own row

### Fixed

- **No key worked** (issue #6, probably also #5): if the game's `config.cfg` contains `uset g_console_state "1"`, BeyondCab thought the console was open and ignored Ctrl + F7, E and the controller button. That saved value now only counts once the console has been closed
- The "developer camera off" hint also appeared when `config.cfg` couldn't be read; now only when the lines really are 0 – and only once you're in the game, for 15 seconds
- Menu at 1440p/4K: clicks right after a mouse move sometimes missed
- Russian/Chinese: paper status (paid, expired …) coloured again, expired certificates red; long texts no longer cut off; the US Bill of Lading stays English; weekdays, country names and sentences with keys can now be translated
- The "Papers" heading under Display showed German in the English menu
- Log: long mod lists complete, ignored keys with the reason, fewer repeated lines
- **User names with Cyrillic or Chinese characters** (or OneDrive Documents): BeyondCab couldn't find the game profile – papers, repair kit and tachograph were never saved, settings went into the plugin folder and the custom models (warning light, chocks …) were missing. The previous settings and papers from the plugin folder are taken over on the first start
- **Speed cameras**: a pending notice was charged in the other profile after switching profiles
- **Tachograph**: after loading an older save, driving time, break and card stayed at the later state – a check could fine you wrongly or miss offences
- Toll and ferry receipts still listed the trailer after uncoupling
- Console: with a saved `g_console_state "1"` the first time you open the console now counts too (typing doesn't trigger anything)
- Quitting during an update download no longer crashes; long photo paths in the settings no longer break the ini
- **Stuck while walking**: if the camera changed (e.g. a save loaded from the Esc menu), the keyboard stayed blocked – walking now ends by itself after 1.5 s
- **Keys stuck "pressed" in the game**: releases now always reach the game – before, the truck kept going if you opened the menu while accelerating, or Ctrl stuck after Ctrl + F7
- After BeyondCab switches itself off (memory error), controller, Esc, traffic and flashlight are no longer left blocked
- Getting out/in no longer gives up after 0.3 s at high frame rates (now 2 s)
- After loading another save: ground and collision start clean on the next exit, passenger seat/bunk reset, no invisible walls
- **Loading a save**: the repair kit is no longer wrongly charged as "topped up at the workshop", the breakdown service no longer bills a repair from the discarded timeline, no false towing invoice appears, and fuel before and after loading no longer ends up on one receipt
- Repair kit: the "trailer already patched" limit is no longer lost when the game restarts
- Sleeping: if the sleep dialog stayed open for more than 3 minutes, keys went to the game while walking afterwards
- Profile switch: the own coach door key is read again, the signed consignment note of the previous profile is no longer waiting
- The window motor sound looped forever if own sounds were switched off meanwhile
- **Speed cameras**: after loading a slightly older save, the notice for a photo that never happened there still came – and was charged
- **Ferry**: the port walk-round stayed valid after loading an older save or switching profiles; a crossing from the other profile could be billed in the new one
- Weigh station: the check overwrote a fine the game had just reported (which also brought back the double rest fine)
- Papers: an older save loaded right after starting the game didn't remove the later receipts; after deleting the first receipt, the second pump side overwrote the previous station's receipt; Russian: "signed" and "police" status coloured again
- **Consignment note after cancelling/delivering and reloading**: loading a save from before the cancellation (or delivery) lost the papers you had already taken – the next check fined you for a missing CMR and delivery went through "with reservation"
- After loading an older save: no half-finished coupling sequence on the freshly loaded trailer (the lever came next), tachograph printout, fuel receipt and toll/ferry tickets from the discarded timeline are gone; the remote key's "locked" state no longer blocks getting in after loading
- Getting in: a delayed get-in (door first, coach doors) no longer pulls you into the cab if you walked away meanwhile or walking had already ended
- Seat change: switching to an outside camera during it left the mouse frozen; Esc while refuelling no longer leaves Enter held
- Repair kit: after loading an older save, the contents from back then apply again (before, a paid top-up or used parts stayed); coach timetable: no arrival times from the discarded timeline
- **Wheel chocks on profile switch**: the new profile's job was still applied to the old one – chocks vanished there or appeared twice at the trailer when switching back; starting the game with a running job no longer placed missing chocks
- **Remote key**: after BeyondCab switched itself off (memory error) or on quitting, keys pressed by the key fob (Shift, horn, windows) stayed down; Alt+Tab while holding it kept the windows moving
- An action key (e.g. E to get out) that is still held after it triggered no longer reaches the game after all
- Equipment: if a model couldn't be placed, its slot stayed taken (could hold up quitting)
- Menu: moving the mouse with the menu open and drawing accessed the same input list without coordination (possible crashes); the fuel card PIN only accepts digits (with "." or "-" the card was refused at every pump); names and address now take the full length in Russian/Chinese too; key capture no longer grabs F7/O from the menu shortcut by accident, controller button capture ends when the page changes
- Removal (setup): if the DLL couldn't be deleted, it still said "removed" and the Apps entry was gone – now it names the file and keeps the entry. In-game update: goes into the game folder you chose instead of another (Steam) copy
- If an in-game update fails, BeyondCab now says so on the next start (before, you silently stayed on the old version)
- **Low frame rates**: below about 14 fps the head bobbed strongly after a landing, below about 11 fps the camera could break completely – now stable
- Bridge without road surface: holding at truck height still counted as "used up" at the next exit on another bridge – you fell through
- Ctrl + F7 no longer blocks mouse and keyboard when the menu can't be shown at all; the seat parcel search no longer uses hundreds of MB
- **Numpad**: keys bound to "Num 0" … "Num 9" didn't work with NumLock on; arrow keys, Insert/Delete, Home/End and Page Up/Down are recognised as the right keys when binding (before: as numpad)
- Coupling: if the game's "attach" is bound to Ctrl/Alt/Shift + key, BeyondCab now says it needs the key without a modifier (otherwise "state not reached"); a controller binding's modifier no longer applies to the keyboard key
- Remote key after a shutdown of BeyondCab: the window switches are released too
- **Driving away after uncoupling**: the drive lock ("landing gear down"/"air lines off") still held the parking brake after a real uncoupling while the kingpin sat in the plate – you couldn't drive away from the dropped trailer
- Controller: a button still held when getting in (e.g. X) no longer triggers its game function (hazard lights); empty controller slots are only polled every 2 s
- `beyondcab.ini` by hand: spaces around "=" and `true`/`yes`/`on` are understood; with duplicate lines in `config.cfg` the last one counts, as in the game
- Flashlight: if the real light dropped out for the whole session after a loading screen or ferry with the lamp on (only the screen effect left), it now keeps working
- PDF export: Chinese titles with certain characters (e.g. 不) were wrong in the document properties; a licence with birthday 29 Feb no longer shows an impossible expiry date; Russian: coupling messages no longer cut off at the end
- **Tachograph**: after the first 45-minute break, 30 minutes were always enough afterwards (the full break counted as the "first 15"); the same driving-time offence of a still running shift was fined again at every further check; a split daily rest with a first part of 7 to 9 h (legal if the 9 h second part follows within 24 h) was fined straight away as "rest too short"
- Consignment note: a save from before the handover at the receiver left the note "handed over" – no worker and no handover afterwards; remarks on signing no longer appear twice; a Road Trip parcel's bill of lading no longer stays open in the folder after cancelling
- Hold actions: swinging over to the next check point while holding the key finished it in a fraction of a second, and the light check didn't switch the lights on ("rear lights dark"); coming over from the previous step no longer starts refuelling by itself
- Fuel card: the payment at a pump stayed valid after driving off – days later the same pump fuelled without the card
- Profile switch: into a profile with a later game time, the tachograph booked the jump as rest in the previous profile; a coach or Road Trip job of the new profile was lost or the old one stayed; a half-finished coupling sequence is reset. A workshop visit after more than 24 h of driving no longer resets the seat and physics
- Loading a **newer** save with the same truck is now detected (by the odometer jump): the remote key lock, breakdown service and fuel stop no longer carry over
- You no longer float endlessly over a real edge (quay, car park deck) – holding bridge height ends after 25 m
- Profile switch or older save: the old profile's papers, placed items and tachograph are no longer trimmed; the same job from an older save loads its consignment note correctly
- After the game's fatigue fine, a check no longer adds "rest overdue" on top
- Equipment: no wrong model on a reused spot, no crash risk when removing while drawing; Alt+Tab in the middle of the remote key no longer leaves Shift/Ctrl stuck
- Menu: opening/closing with Ctrl + F7 could rarely crash; dragging a slider no longer stutters (saved on release); "Reset all settings" keeps name, address, PIN and licence and doesn't restart the introduction; a key is no longer bound by accident when you close the menu or type in the search after "Change"
- Settings: two saves at the same time could corrupt the ini
- Installer: if writing failed for one of the two games, the install was left half-done; now both are tried (with retries) and the successful one is registered
- Stability: vehicle positions, speed camera notice and physics search without concurrent access; quitting the game during a search or while drawing no longer crashes; damaged game archives no longer crash the game
- After a game update: the parking brake is only set if its memory value provably matches the game

## 1.4.3

### Verbessert

- **Menü in hohen Auflösungen**: Das Menü (Strg + F7), die Hinweise und die Markierungen wachsen mit der Auflösung mit – in 1440p und 4K sind sie nicht mehr winzig, die Schrift bleibt scharf. Frachtbrief, Belege und Zapfsäule sehen aus wie bisher
- **Beenden mit anderen Plugins**: Laufen weitere Plugins mit (z. B. CabPlay), stürzt das Spiel beim Beenden nicht mehr ab

---

### Improved

- **Menu at high resolutions**: the menu (Ctrl + F7), the hints and the markers now scale with your resolution – no longer tiny in 1440p and 4K, with sharp text. Waybill, receipts and fuel pump look the same as before
- **Quitting with other plugins**: when other plugins run alongside (e.g. CabPlay), the game no longer crashes on exit

## 1.4.2

### Verbessert

- **Entwicklerkamera aus** (Issue #5): Aussteigen braucht die Entwicklerkamera des Spiels (`uset g_developer "1"` und `uset g_console "1"` in der `config.cfg`). Ist sie aus, sagt BeyondCab das jetzt kurz nach dem Start und zeigt es unter Allgemein › Spielversion – vorher passierte beim Drücken von E einfach nichts
- Das Log nennt die Einstellungen der Entwicklerkamera und den Renderer des Spiels (BeyondCab braucht DirectX 11)
- README: Entwicklerkamera unter den Voraussetzungen, Hinweis zur Fn-Taste für Strg + F7 auf Laptops

---

### Improved

- **Developer camera off** (issue #5): getting out needs the game's developer camera (`uset g_developer "1"` and `uset g_console "1"` in `config.cfg`). If it's off, BeyondCab now tells you shortly after the start and shows it under General › Game version – before, pressing E simply did nothing
- The log lists the developer camera settings and the game's renderer (BeyondCab needs DirectX 11)
- README: developer camera under requirements, note about the Fn key for Ctrl + F7 on laptops

## 1.4.1

### Neu

- **Chinesisch** in der Sprachauswahl: 简体中文 und 繁體中文 (Automatisch je nach Windows-Sprache). Die Übersetzung entsteht gerade in der Community – noch fehlende Texte erscheinen auf Englisch

### Verbessert

- **Ankoppeln zu Fuß** (Issue #4): Wo bisher einfach kein Punkt erschien, sagt BeyondCab jetzt, woran es liegt:
  - Spieloption „Erweitertes Ankoppeln“ aus (Optionen → Gameplay) – ohne sie geht Ankoppeln nur per Anhänger-Taste im Truck
  - „Auf der anderen Seite“, wenn man auf der falschen Seite des Trucks oder Anhängers steht
  - „Zapfen nicht eingerastet“, wenn der Truck knapp vor dem Königszapfen steht oder die Höhe nicht passt
  - „Erst vorziehen und neu unterfahren“ erscheint jetzt auch dann, wenn es vorher still blieb
- Der Kuppel-Punkt verschwindet nicht mehr, wenn der Truck noch minimal rollt
- Ausführlicheres Log für Fehlerberichte: aktive Mods, Kuppel-Einstellungen, Anhänger, Aus- und Einsteigen, jeder Kuppel-Schritt und warum er nicht bedienbar ist

### Behoben

- Papiere: lange Reiter („Bescheide & Rechnungen“) liefen ineinander
- Ankoppeln: Der Ablauf konnte gleich nach „Sattelkupplung prüfen“ abbrechen
- Ankoppeln: „Stützen hochkurbeln“ konnte bei „Erst Leitungen anschließen“ hängen bleiben
- Der Hinweis zum Werkzeugkoffer nennt jetzt auch das Fahrgestell

---

### New

- **Chinese** in the language selection: 简体中文 and 繁體中文 (Auto follows the Windows language). The translation is being made by the community – missing texts show in English

### Improved

- **Coupling on foot** (issue #4): where simply no point appeared, BeyondCab now tells you why:
  - game option "Trailer advanced coupling" is off (Options → Gameplay) – without it coupling only works with the trailer key in the cab
  - "On the other side" when you stand on the wrong side of the truck or trailer
  - "Kingpin not locked" when the truck stopped just short of the kingpin or the height doesn't fit
  - "Pull forward and back under again first" now also shows where it stayed silent before
- The coupling point no longer disappears while the truck is still creeping slightly
- More detailed log for bug reports: active mods, coupling settings, trailer, getting out and in, every coupling step and why it can't be used

### Fixed

- Papers: long tabs ("Notices & invoices") ran into each other
- Coupling: the sequence could end right after "Check fifth wheel"
- Coupling: "Crank up landing gear" could get stuck on "Connect lines first"
- The toolbox note now mentions the chassis too

## 1.4.0

### Neu

- **Pannenkit** (optional): Kleine Schäden notdürftig selbst flicken – Kabine mit Gewebeband und Kabelbindern, Motor mit Kühlmittel und Öl, Fahrgestell mit Kabelbindern, beim Auflieger der Aufbau mit Flicken. Dazu den Werkzeugkoffer aus dem Staukasten holen und an der Stelle abstellen, dann erscheinen die Reparaturpunkte. Repariert wird nur provisorisch (höchstens die Hälfte, bis 20 % Schaden), der Rest bleibt für die Werkstatt. Das Kit gehört zum Truck und wird beim Tanken oder in der Werkstatt nachgefüllt
- **Pannendienst** (optional, über die Schnellwahl): Ein Abschleppwagen mit Rundumleuchten, Warnblinker und Licht fährt vor, ein Mechaniker steigt aus, prüft den Truck, repariert kniend am Vorderrad Motor, Getriebe, Kabine und Fahrgestell zur Hälfte und bringt dir die Rechnung. Ist der Truck nicht mehr fahrbereit, rät er zum Abschleppen. In ETS2 ein Pritschenwagen, in ATS ein Ford F-350 mit Hubarm. Der Platz wird geprüft (Steigung, Mauern, Verkehr), der Verkehr hält an, und der Mechaniker läuft um deinen Zug herum
- **Rechnungen in der Mappe**: Pannendienst und Abschleppen über den Hilfe-Dienst des Spiels (F7) kommen als Rechnung mit Einsatzort, Positionen und Mehrwertsteuer des Landes (optional)
- **Staukasten neu**: übersichtlich in Gruppen, mit Maus-Zeiger (Klick nimmt, Rechtsklick schließt) und Controller-Stick
- **Eigene Geräusche** für Pannendienst und Pannenkit (Anfahrt, Tür, Werkzeugkiste, Schlagschrauber, Ratsche, Gewebeband, Kabelbinder, Abfahrt) mit eigener Lautstärke im Menü
- **Busse**: Fahrtenblatt mit Pünktlichkeit je Halt, Mautbeleg sowie Fähr- und Bahnticket als Blätter in der Mappe

### Verbessert

- Beim Laufen ist auch die Tastatur des Spiels gesperrt, wenn sie über DirectInput gelesen wird – WASD lenkte sonst den Truck
- Island: Orte für Rechnungen und Belege (vorher erschien Glasgow)
- Bus: Tankdeckel und Kartenterminal nicht mehr durch die Wand aus dem Innenraum, dazu weitere Kleinigkeiten (Oberdeck, Aufstehen, Türen)

### Behoben

- Einsteigen ohne Tastaturtaste für die Innenkamera (nur Controller belegt): Die Kamera wechselte nicht (Issue #3)

---

### New

- **Repair kit** (optional): patch up small damage yourself – the cab with duct tape and cable ties, the engine with coolant and oil, the chassis with cable ties, and on the trailer the body with patches. Take the toolbox from the storage box and set it down at the spot, then the repair points appear. Repairs are only temporary (at most half, up to 20 % damage); the rest is left for the workshop. The kit belongs to the truck and is refilled when refuelling or at the workshop
- **Breakdown service** (optional, from the quick menu): a tow truck with beacons, hazard lights and headlights pulls up, a mechanic gets out, checks the truck, kneels at the front wheel to fix half of the engine, gearbox, cab and chassis damage and brings you the invoice. If the truck isn't roadworthy, he recommends towing. A flatbed in ETS2, a Ford F-350 wrecker in ATS. The spot is checked (slopes, walls, traffic), traffic stops, and the mechanic walks around your rig
- **Invoices in the paper folder**: the breakdown service and towing through the game's assistance (F7) arrive as an invoice with place, items and the country's VAT (optional)
- **Storage box redesigned**: grouped and clear, with a mouse pointer (click takes, right-click closes) and controller stick
- **Own sounds** for the breakdown service and repair kit (arrival, door, toolbox, impact wrench, ratchet, duct tape, cable ties, driving off) with their own volume in the menu
- **Coaches**: trip sheet with punctuality per stop, toll receipt and ferry and train tickets as sheets in the paper folder

### Improved

- While walking, the game's keyboard is blocked too when it's read through DirectInput – WASD steered the truck before
- Iceland: places for invoices and receipts (Glasgow showed up before)
- Coach: fuel cap and card terminal no longer reachable through the wall from inside, plus smaller fixes (upper deck, standing up, doors)

### Fixed

- Getting in without a keyboard key for the interior camera (controller only): the camera didn't switch (issue #3)

---

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
