# KegelBuddy – Patchnotes

Neueste Version steht oben.

## v0.12
- Teilen per Link: Pro Spiel („🔗 Teilen“) oder für alle Spiele samt Kategorien. Der Link enthält die Daten selbst, es wird kein Server benötigt. Wer ihn öffnet, sieht eine Auswahl und kann die Spiele importieren.
- Export als Datei: Pro Spiel („📄 Datei“) oder alles zusammen inkl. eigener Sounds (Einstellungen → „Alles als Datei sichern“). Auf dem Handy öffnet sich dafür das Teilen-Menü (z. B. WhatsApp).
- Import mit Auswahl: neue Spiele sind vorausgewählt, bereits vorhandene werden nur auf Wunsch überschrieben, identische übersprungen. Alte Sicherungen (v0.01–v0.11) lassen sich weiter importieren. Importierte Daten werden geprüft und bereinigt.
- Soundboard: Stopp-Button (bleibt oben sichtbar, zeigt die Anzahl laufender Sounds), Option „Neuer Sound beendet den vorherigen“, Sounds stoppen beim Verlassen des Soundboards. Der Mix startet frisch.
- Als App installierbar (PWA): Manifest, Icons und Service Worker für GitHub Pages; läuft danach auch offline.
- Neue Dateien für das Repository: index.html, manifest.webmanifest, sw.js, Icons, README.md.

## v0.11
- 20 weitere Sounds eingebaut, jetzt insgesamt 40 in 6 Gruppen:
  - 🎯 Kill-Ansagen (13): + Monster Kill, Ownage, Rampage, Triple Kill, Unstoppable, Wicked Sick
  - 😂 Pointe & Lachen (6): + Okay, Quietscheente
  - 💀 Fail & Peinlich (6): + Windows-Fehler, Nope
  - 😢 Traurig & Verloren (3, neue Gruppe): Trauriges Klavier, Traurige Geige, Wah wah wah
  - 🎬 Drama & Spannung (7): + Alarm (Metal Gear), Warten, „Two hours later“, Run
  - 🎵 Effekte (5): + Schlag, Ohrfeige, Troped
- Die HTML-Datei ist dadurch ca. 4 MB groß.

## v0.10
- Soundboard: 20 mitgelieferte Sounds, in 5 Gruppen sortiert:
  - 🎯 Kill-Ansagen: Headshot, Boom Headshot, Double Kill, Mega Kill, Killing Spree, Dominating, Godlike
  - 😂 Pointe & Lachen: Ba-dum-tss, Lachen, „Das ist ja eine Giraffe“, Easy
  - 💀 Fail & Peinlich: GTA Wasted, Bruh, Grille, Furz
  - 🎬 Drama & Spannung: Dun dun dun, „A few moments later“, Illuminati
  - 🎵 Effekte: DJ, Doiiing
- Mitgelieferte Sounds sind fest in der App eingebettet und belegen keinen Browser-Speicher.
- Eigene Sounds: beim Hinzufügen eine Gruppe wählen oder eine neue anlegen; später per „Gruppe“ verschieben.
- Sound-Mix ist ebenfalls nach Gruppen sortiert.
- Die HTML-Datei ist dadurch ca. 2 MB groß.

## v0.09
- Bingo zusammengeführt: Ein einziger Eintrag „Bingo“ (gemeinsames Feld als Grundspiel, „jeder bekommt ein eigenes Feld“ als Option). Dadurch wird Bingo im Spielgenerator nicht doppelt gewichtet.
- Die beiden Einträge aus v0.08 (gemeinsames/eigenes Feld) werden beim Start automatisch entfernt.
- Korrektur zur ersten Auslieferung von v0.09: Der neue Eintrag „Bingo“ fehlte dort noch im Archiv und wurde nachgereicht (geprüft mit frischer Installation und Upgrade von v0.08).

## v0.08
- Neu im Spielearchiv: Bingo (gemeinsames Feld) und Bingo (eigenes Feld), jeweils mit Bild.
- Zufallsgenerator: neuer Bereich „Bingo-Feld“ – mischt die Zahlen 1–9 in ein 3×3-Feld, wahlweise mehrere Felder auf einmal (1–12).
- Offen: Zählen Diagonalen? Darf ein Spieler dasselbe Feld mehrfach belegen? Spielende ohne Bingo?

## v0.07
- Bilder für Spiele: Auswahl aus rund 100 Symbolen (Emojis) im Spiel-Editor (Feld „Bild“, „∅“ = kein Bild).
- Alle mitgelieferten Spiele haben ein Bild; bereits vorhandene Spiele bekommen es automatisch, sofern sie noch keins haben.
- Bild wird im Spielearchiv, beim Spielgenerator (groß beim gezogenen Spiel) und in der Liste der gezogenen Spiele angezeigt.
- Fuchsjagd korrigiert: Der Fuchs wirft zweimal, einmal mit rechts und einmal mit links (Vorsprung). Dreimal werfen als Anfänger-Variante.

## v0.06
- Fuchsjagd: Regeln ergänzt (Quelle: Planet Wissen / WDR), inkl. Variante mit bewerteten Kegelbildern.
- Namensliste korrigiert: Log In (Team) und Tannenbaum haben keine Namensliste mehr (Teamspiele). Wird einmalig auch in bereits vorhandenen Daten angepasst.

## v0.05
- Neu: Rechenkette (Rechenspiel mit + − × : =, strikt von links nach rechts, höchstes Ergebnis gewinnt).
- Offen: Platzierung der Zahlen (frei oder feste Wurfreihenfolge).

## v0.04
- Neu: In die Vollen (Grundspiel, 3 Würfe pro Spieler, Kegel nach jedem Wurf neu aufgestellt).
- Regeln ergänzt: Tannenbaum (mit optionalem Joker), Hohe Hausnummer, Niedrige Hausnummer, Schiffe versenken.
- Bereits angelegte Platzhalter ohne Regeltext werden automatisch befüllt; selbst bearbeitete Spiele bleiben unverändert.
- Weiterhin offen: Fuchsjagd (Regeln fehlen), Anzahl Striche pro Boot bei Schiffe versenken.

## v0.03
- Mitgelieferte Spiele werden beim Start einmalig angelegt (gelöschte kommen nicht zurück, eigene Spiele bleiben unberührt):
  - Log In (Team), Log In (Solo)
  - Wie du mir, so ich dir; Berg- und Talbahn; Miteinander; Mensch ärgere Dich nicht; Sargspiel (Regeln aus den Anleitungsblättern)
  - Tannenbaum, Fuchsjagd, Hohe Hausnummer, Niedrige Hausnummer, Schiffe versenken (Platzhalter, Regeln noch offen)
- Neue Kategorien „In die Vollen“ und „Abräumen“ werden automatisch angelegt.
- Sicherung/Export enthält nun auch die Info, welche Spiele bereits mitgeliefert wurden.

## v0.02
- Bisheriger „Zufallsgenerator“ (Spiele ziehen) umbenannt in **Spielgenerator** (Tab, Überschrift, Icon 🎮).
- Neuer **Zufallsgenerator** (Tab): Zahlen würfeln von–bis (einschließlich).
  - Anzahl Würfe (1–50), Summe bei mehreren Würfen
  - Option „Keine doppelten Zahlen innerhalb eines Wurfs“
  - Schnellwahl: W6, W20, W100, Kegel 1–9
  - Verlauf der letzten 30 Würfe, leerbar
- Übersicht: Schnellzugriff um „🎲 Würfeln“ ergänzt.
- Versionsanzeige in Kopfzeile, Fußzeile und Entwicklermodus.

## v0.01
- Erster Prototyp: Spielearchiv, Zufallsgenerator (Spiele ziehen ohne Zurücklegen), Soundboard mit Mix, Kategorien, Export/Import, Entwicklermodus.
