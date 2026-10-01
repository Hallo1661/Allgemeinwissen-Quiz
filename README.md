# Wissensraum – deutsches Lernquiz

Eine fertige statische Quiz-App mit **3.013 Fragen**. Kein Build, kein Backend, kein API-Schlüssel, kein kostenpflichtiger Dienst.

**Umfang:** Das gewünschte reduzierte Ziel von 5.000 Fragen ist nicht erreicht; es fehlen 1.987. Der Bestand ist deutlich literaturlastig. Gemischte kurze Runden verteilen die Fragen gleichmäßig über die verfügbaren Kategorien. Quellen und Prüfgrenzen stehen in [QUELLEN.md](QUELLEN.md) und [PRUEFBERICHT.md](PRUEFBERICHT.md). Eine unabhängige fachliche Prüfung jeder einzelnen Antwort wird nicht behauptet.

## Sofort ausprobieren

1. Die ZIP-Datei vollständig entpacken.
2. Im entpackten Ordner **index.html** doppelt anklicken.
3. Antwort auswählen oder eintippen und **Antwort prüfen** drücken. Sofort erscheint richtig oder falsch; bei Fehlern wird die richtige Lösung angezeigt.

Die Dateien müssen zusammenbleiben. Eine Vorschau innerhalb eines ZIP-Archivs funktioniert nicht zuverlässig.

## Bei GitHub hochladen und online nutzen

1. Bei GitHub anmelden und ein neues **öffentliches Repository** anlegen, z. B. `wissensquiz`. Öffentlich ermöglicht GitHub Pages mit GitHub Free.
2. Im Repository **Add file → Upload files** öffnen. Bei einem noch leeren Repository auf **uploading an existing file** klicken.
3. **Alle entpackten Dateien aus diesem Ordner** hochladen. Wichtig: `index.html` muss direkt auf der obersten Ebene des Repositorys liegen, nicht in einem zusätzlichen Unterordner. **Nicht die ZIP-Datei selbst hochladen.**
4. Mit **Commit changes** speichern. Der Standardbranch heißt gewöhnlich `main`.
5. **Settings → Pages** öffnen. Unter **Build and deployment → Source** die Option **Deploy from a branch** wählen.
6. Branch **main**, Ordner **/ (root)** wählen und **Save** klicken.
7. Einige Minuten warten. Unter **Settings → Pages** erscheint der Website-Link, normalerweise `https://DEIN-NAME.github.io/wissensquiz/`.

Du brauchst kein Terminal, kein npm und keinen eigenen Build. GitHub erledigt die Pages-Bereitstellung. Der Upload und die Aktivierung werden von dir vorgenommen; für diese Lieferung wurde nichts veröffentlicht und kein Repository angelegt.

Offizielle Anleitung: [GitHub Pages konfigurieren](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## So lernst du

- Wähle ein Themengebiet und 10, 20, 50 oder alle Fragen. **Neue Runde starten** übernimmt die Einstellungen.
- **Auswahl:** Bei 2.683 Werkfragen gibt es vier Antwortmöglichkeiten; genau eine davon ist die hinterlegte richtige Antwort. Die 330 übrigen Fragen verwenden Freitext.
- **Eintippen:** Nutzt bei allen Fragen Freitext. Der lokale Vergleich ignoriert Großschreibung, Akzente, manche Artikel und überflüssige Satzzeichen. Hinterlegte Namensvarianten und numerische Datumsformen werden berücksichtigt. Es findet keine semantische KI-Bewertung statt. Eine sinngleiche, nicht erkannte Antwort lässt sich über **Meine Formulierung ist auch richtig** korrigieren.
- **Weiß ich noch nicht** zeigt die Lösung und merkt die Frage als Fehler.
- **Hintergrund & Quelle** zeigt die jeweilige Herkunft; bei GermanQuAD auch den historischen Hintergrundtext.
- **Fehler wiederholen** nutzt Fragen, deren letzte Bewertung falsch war. Eine richtige Wiederholung entfernt sie aus dieser Auswahl.
- Am Rundenende kannst du gezielt die Fehler dieser Runde wiederholen.

## Speicherung und Offline-Nutzung

Fortschritt und laufende Runde werden nur im lokalen Speicher dieses Browsers gespeichert. Kein Benutzerkonto, keine Übertragung der Antworten, kein Tracking. Andere Geräte oder Browser haben einen eigenen Fortschritt. Privater Modus oder das Löschen von Websitedaten kann ihn entfernen. Ohne erlaubten lokalen Speicher bleibt das Quiz spielbar, speichert aber nicht dauerhaft.

Die entpackte lokale Version funktioniert offline. Für die erstmalige Nutzung der GitHub-Pages-Version brauchst du Internet; ein installierbarer Offline-Cache ist nicht Bestandteil der App. Das Spielen selbst fragt keine externen APIs ab. Quellenlinks benötigen Internet.

## Dateien

- `index.html`, `styles.css`, `app.js`, `engine.js`, `questions.js`, `favicon.svg`: vollständige App.
- `ANLEITUNG.html`, `README.md`: Bedienung und GitHub-Upload.
- `QUELLEN.md`, `LICENSE-CODE.txt`: Herkunft und Lizenzen; beim Weitergeben beibehalten.
- `PRUEFBERICHT.md`, `DATENPRUEFUNG.json`: Zählung, Auswahlgrenzen und Prüfung.
- `.nojekyll`: verhindert eine unnötige Jekyll-Verarbeitung, sofern mit hochgeladen. Die App verwendet keine speziellen Jekyll-Funktionen und funktioniert auch ohne diese Datei.

## Falls die Website nicht erscheint

- Prüfen, ob `index.html` tatsächlich im Repository-Hauptordner liegt und die Schreibweise unverändert ist.
- Unter Pages prüfen: richtiger Branch, **/ (root)** und **Deploy from a branch**.
- Unter **Actions** den Pages-Bereitstellungsstatus ansehen. GitHub kann einige Minuten brauchen.
- Wenn nur die Fragen fehlen: `questions.js` und `engine.js` mit hochladen und die Seite neu laden.

Stand: 1. Oktober 2026.
