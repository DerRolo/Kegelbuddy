# 🎳 KegelBuddy
Aufrufen: https://derrolo.github.io/Kegelbuddy/

**Der Werkzeugkasten für den Kegelabend.** Spielregeln nachschlagen, ein Spiel auslosen, Zahlen würfeln und mit einem Soundboard für die richtige Stimmung sorgen. Alles läuft im Browser, ohne Konto und ohne Server. Als App auf dem Handy installierbar, auch offline.

## Was kann die App?

| Bereich | Das kannst du tun |
|---|---|
| **Spielearchiv** | 15 Kegelspiele mit Regeln, nach Kategorien filterbar und durchsuchbar. Eigene Spiele anlegen, Bild (Emoji) wählen, bearbeiten und löschen. |
| **Spielgenerator** | Zufälliges Spiel ziehen, ohne Zurücklegen. Filter nach Kategorie und danach, ob das Spiel eine Namensliste braucht (Einzelspiele) oder ein Teamspiel ist. |
| **Zufallsgenerator** | Zufallszahlen von–bis würfeln (W6, W20, W100, Kegel 1–9, beliebiger Bereich, mehrere Würfe, ohne Doppelte). Dazu ein **Bingo-Feld**-Generator, der die Zahlen 1–9 in ein 3×3-Feld mischt. |
| **Soundboard** | 40 Sounds in 6 Gruppen, eigene Sounds hinzufügen, mehrere Sounds als Mix abspielen, **Stopp**-Button. |
| **Teilen** | Einzelne Spiele oder alle per **Link** in die WhatsApp-Gruppe schicken, oder als **Datei** exportieren. Beim Import wählst du aus, was übernommen wird. |

## Die Spiele

Die vollständigen Regeln stehen in der App selbst.

**Teamspiele (ohne Namensliste):** Log In (Team), Tannenbaum

**Gegeneinander (mit Namensliste):** Log In (Solo), Wie du mir so ich dir, Berg- und Talbahn, Miteinander, Mensch ärgere Dich nicht, Sargspiel, In die Vollen, Hohe Hausnummer, Niedrige Hausnummer, Schiffe versenken, Rechenkette, Bingo, Fuchsjagd

Begriffe: **In die Vollen** = auf alle neun Kegel werfen · **Abräumen** = auf stehende Kegel werfen · **Gosse/Pudel** = die Kugel trifft nichts · **Strich** = Minuspunkt.

## So spielt ihr einen Abend

1. **Spielgenerator** öffnen, Kategorie wählen, „Lostopf neu füllen“ und „Nächstes Spiel ziehen“. Ein gezogenes Spiel kommt in der Runde nicht noch einmal dran.
2. Im **Spielearchiv** die Regeln des gezogenen Spiels vorlesen.
3. Für Spiele mit Zufallszahlen (z. B. Bingo-Feld) den **Zufallsgenerator** benutzen.
4. Bei Treffer, Pudel oder Pleite das passende Geräusch aus dem **Soundboard** abfeuern. Mit **⏹ Stopp** ist sofort Ruhe.

## Sounds

- 🎯 **Kill-Ansagen**: Headshot, Boom Headshot, Double Kill, Mega Kill, Killing Spree, Dominating, Godlike, Monster Kill, Ownage, Rampage, Triple Kill, Unstoppable, Wicked Sick
- 😂 **Pointe & Lachen**: Ba-dum-tss, Lachen, „Das ist ja eine Giraffe“, Easy, Okay, Quietscheente
- 💀 **Fail & Peinlich**: GTA Wasted, Bruh, Grille, Furz, Windows-Fehler, Nope
- 😢 **Traurig & Verloren**: Trauriges Klavier, Traurige Geige, Wah wah wah
- 🎬 **Drama & Spannung**: Dun dun dun, „A few moments later“, Illuminati, Alarm (Metal Gear), Warten, „Two hours later“, Run
- 🎵 **Effekte**: DJ, Doiiing, Schlag, Ohrfeige, Troped

Eigene Sounds (Audiodateien) kannst du im Soundboard hinzufügen und einer Gruppe zuordnen.

## Auf dem Handy installieren

- **Android (Chrome):** Link öffnen → Menü ⋮ → **App installieren**.
- **iPhone (Safari):** Link öffnen → Teilen-Symbol → **Zum Home-Bildschirm**.
- **PC (Chrome/Edge):** Symbol „Installieren“ in der Adresszeile.

## Spiele mit der Gruppe teilen

- **Link:** Beim Spiel auf **🔗 Teilen** tippen oder in den Einstellungen **Alle Spiele & Kategorien als Link teilen**. Den Link in WhatsApp senden. Wer ihn öffnet, bekommt eine Auswahl und kann die Spiele importieren. Sounds sind im Link nicht enthalten.
- **Datei:** **📄 Datei** beim Spiel oder in den Einstellungen **Alles als Datei sichern** (inkl. eigener Sounds). Import: Einstellungen → **Import aus Datei**. Gut als Backup.

Beim Import werden neue Spiele vorausgewählt. Bereits vorhandene Spiele werden nur überschrieben, wenn du sie ankreuzt.

**Wichtig zu wissen**
- Alle Daten liegen nur lokal im Browser des Geräts. Wer die Browserdaten löscht, verliert sie. Darum gelegentlich eine Datei sichern.
- Auf dem **iPhone** hat die installierte App einen eigenen Speicher, getrennt von Safari. Ein in Safari geöffneter Link landet nicht in der installierten App. Dort bitte die Export-Datei verwenden.
- Der Browser-Speicher fasst etwa 5 MB. Viele große eigene Sounds können ihn füllen („Speicher voll“).

## Selbst veröffentlichen (GitHub Pages)

1. Neues Repository auf github.com anlegen (öffentlich) und alle Dateien dieses Ordners hochladen, inklusive `.nojekyll`. `index.html` muss im Hauptverzeichnis liegen.
2. **Settings → Pages**: Source **Deploy from a branch**, Branch **main**, Ordner **/ (root)**, speichern.
3. Nach ein bis zwei Minuten ist die App erreichbar unter `https://<dein-name>.github.io/<repo-name>/`.

Update veröffentlichen: `index.html` und `patchnotes.md` im Repository ersetzen und in `sw.js` die Zahl bei `CACHE` hochzählen, damit installierte Apps die neue Version laden.

## Technik

Eine einzelne HTML-Datei ohne Abhängigkeiten, dazu Manifest, Service Worker und Icons. Speicherung per `localStorage`. Versionsverlauf: [patchnotes.md](patchnotes.md).
