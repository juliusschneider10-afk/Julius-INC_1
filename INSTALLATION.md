# JULIUS INC. — THE HUGO TRADING COMPANY
Fabric-Mod für Minecraft 26.1.2 (Mac). Du musst nichts programmieren.

## Schritt 1: Jar-Datei bauen lassen (einmalig, ca. 10 Minuten)
Die .jar wird kostenlos von GitHub gebaut.

1. Konto erstellen auf github.com (kostenlos) und einloggen.
2. Oben rechts "+" > "New repository". Name z.B. `julius-inc`, "Private" wählen, "Create repository".
3. Entpacke dieses ZIP. Auf der Repository-Seite "uploading an existing file" klicken und den KOMPLETTEN INHALT des Ordners `julius-inc` hineinziehen
   (Ordner `src`, Dateien `build.gradle`, `gradle.properties`, `settings.gradle` usw.). Dann "Commit changes".
4. Den Bau-Workflow anlegen (Finder versteckt den Ordner `.github`, deshalb so):
   "Add file" > "Create new file". Als Dateiname exakt `.github/workflows/build.yml` eintippen
   (die Schrägstriche erzeugen die Ordner). Inhalt der Datei `WORKFLOW-build.yml` hineinkopieren. "Commit changes".
5. Oben auf den Reiter "Actions" gehen. Der Lauf "Build JULIUS INC." startet automatisch (ca. 3-5 Minuten, grüner Haken = fertig).
6. Auf den fertigen Lauf klicken, unten bei "Artifacts" `JULIUS-INC-mod` herunterladen und entpacken.
   Darin liegt `julius-inc-1.0.0.jar`.

Wenn der Lauf rot wird: auf den Lauf klicken, den roten Fehlertext kopieren und im Chat an Claude schicken. Das wird dann behoben.

## Schritt 2: Installation auf dem Mac
1. Fabric-Installer von fabricmc.net laden, Minecraft-Version 26.1.2 wählen, installieren
   (er legt ein Profil im Minecraft-Launcher an).
2. Fabric API für 26.1.2 von modrinth.com/mod/fabric-api laden.
3. Finder > Menü "Gehe zu" > "Gehe zum Ordner…" > `~/Library/Application Support/minecraft/mods`
   (Ordner `mods` anlegen, falls er fehlt). Dort hinein: Fabric-API-Jar und `julius-inc-1.0.0.jar`.
4. Launcher: Fabric-Profil starten.

## Benutzung
- Taste **J** öffnet das Dashboard (änderbar unter Optionen > Steuerung > Tastenbelegung > JULIUS INC.).
- Tabs: Übersicht, Handel (Kauf/Verkauf/Ausgabe/Einnahme buchen), Verlauf, Bestand, Preise, Feed, Optionen.
- Zuerst unter Optionen das Startkapital setzen.
- Zahlen: `1500`, `1,5k`, `2m`, `1b`. Währungssymbol in der Anzeige: `$`.
- Daten liegen lokal in `~/Library/Application Support/minecraft/config/julius_inc.json` (Sicherung = diese Datei kopieren).

## Hugo SMP / Serverregeln
Die Mod sendet nichts an den Server und liest keine Serverdaten aus. Preise trägst du selbst ein.
Der Feed merkt sich nur Chat-Zeilen mit deinen Stichwörtern, die dein Client ohnehin anzeigt.
Prüfe bei Unsicherheit die Regeln des Hugo SMP.
