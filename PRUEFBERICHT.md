# Prüfbericht – Wissensraum

Stand: 1. Oktober 2026.

## Tatsächlich enthalten

**3.013 Fragen statt der gewünschten 5.000. Es fehlen 1.987.** Die Zahl bezeichnet ausgelieferte unterschiedliche Datensätze mit Frage, Antwort und Herkunft; sie ist kein Gütesiegel für eine unabhängige fachliche Einzelprüfung aller Fakten.

| Kategorie | Fragen |
|---|---:|
| Geografie | 36 |
| Geschichte | 82 |
| Gesellschaft & Wirtschaft | 17 |
| Naturwissenschaften | 81 |
| Philosophie & Religion | 31 |
| Sprache & Kultur | 32 |
| Technik & Informatik | 51 |
| Literatur | 2.251 |
| Kunst | 66 |
| Musik | 366 |

Der Bestand enthält 330 ausgewählte GermanQuAD-Fragen und 2.683 aus tatsächlichen Wikidata-Werkzuordnungen formulierte Fragen. Literatur ist mit Abstand die größte Kategorie. Kurze gemischte Runden werden nach Kategorien ausgewogen zusammengestellt; über „Alle Fragen“ ist der gesamte Bestand erreichbar.

## Datenauswahl und Grenzen

Die vorhandenen Werk-Abfragen lieferten 2.857 Literatur-, 1.166 Kunst- und 4.669 Musikzeilen. Eine Rohdatenzeile ist nicht automatisch eine geeignete Quizfrage. Ausgeschlossen wurden insbesondere:

- fehlende auf Deutsch nutzbare Personennamen im lokalen Bestand;
- mehrere unterschiedliche Personen für dieselbe abgefragte Zuordnung;
- offensichtliche Nummernserien und Katalognummern, verräterische Namen im Werktitel sowie unklare Klammerzusätze;
- bei Musik: Filme, Sammlungen und Einträge ohne lokal prüfbare musikalische Einordnung;
- bei vorhandenen Einzelangaben: widersprüchliche Werte und bestimmte unsichere oder eingeschränkte Zuschreibungen;
- redaktionell erkannte problematische Kunstzuschreibungen, gemeinsame Gesamtwerke und eine besonders ähnliche Frageform;
- doppelte Werk-IDs, gleiche normalisierte Werktitel und doppelte normalisierte Frageformulierungen.

Für 369 der ausgelieferten Wikidata-Fragen lagen zusätzliche vollständige Eigenschaftsangaben zur Einzelprüfung auf Widersprüche/Einschränkungen vor. 2.314 beruhen auf der gespeicherten direkten Wikidata-Abfrage. Das bestätigt die Herkunft der Zuordnung, nicht ihre unabhängige wissenschaftliche Richtigkeit. Die Auswahl wurde stichprobenartig inhaltlich gesichtet; beispielsweise wurden Filmmusik-Zuordnungen nicht als Komposition des Films ausgegeben. Nicht jede der 3.013 Fragen wurde durch eine zweite Fachquelle bestätigt. Verbleibende Fehler oder unerkannte semantische Überschneidungen sind möglich. Eine vollständige Garantie semantischer Duplikatfreiheit wird nicht behauptet.

Die GermanQuAD-Fragen wurden einzeln auf Verständlichkeit und Plausibilität ausgewählt und vielfach umformuliert. Die Originalantworten der Kandidaten wurden automatisch gegen die im Datensatz angegebenen Textpositionen geprüft. Die Hintergrundtexte sind historische Datensatzpassagen, keine aktuellen Nachschlageartikel. In der App lassen sich Quellen direkt nach der Antwort öffnen.

Die Auswahl wurde nicht mit erfundenen Fakten, Wiederholungen oder künstlichen Zahlenvariationen auf 5.000 aufgefüllt. Nicht vollständig aufbereitete Rohdaten werden nicht als fertige Fragen mitgezählt und nicht mit der App ausgeliefert.

## Technischer Test

Automatischer Browserlauf in Microsoft Edge/Chromium 154.0.4258.48, zusätzlich direkte Prüfungen der Daten und Programmlogik. Getestet über einen lokalen HTTP-Unterpfad `/lernquiz/` als Modell eines GitHub-Pages-Projektpfads sowie per `file://`.

- Bestanden: Alle Datensätze: IDs, normalisierte Fragen, Antworten, Quellen und genau eine richtige Auswahl
- Bestanden: Freitext: Großschreibung, Datum, falsche Werte und leere Antworten
- Bestanden: Gemischte Runde verteilt 20 Fragen über alle 10 Kategorien
- Bestanden: Start unter GitHub-Pages-Unterpfad, keine externen Spiel-Anfragen
- Bestanden: Falsche Auswahl zeigt sofort Falsch, richtige Lösung und Wiederholungszähler
- Bestanden: Neuladen erhält laufende Frage, Bewertung und Fortschritt
- Bestanden: Richtige Antwort, Weiter und Rundenabschluss zählen korrekt
- Bestanden: Fehler dieser Runde wiederholen; richtige Wiederholung entfernt den Fehler
- Bestanden: Freitext per Enter sofort richtig bewertet
- Bestanden: Freitextfehler zeigt Lösung; manuelle Wertungskorrektur aktualisiert Statistik
- Bestanden: Weiß ich noch nicht deckt Lösung auf und merkt Frage zur Wiederholung
- Bestanden: Kategorie und Rundenlänge funktionieren
- Bestanden: Leerer Fehlerfilter gibt verständliche Rückmeldung
- Bestanden: Alle Fragen: vollständiger Bestand ohne Wiederholung in der Runde
- Bestanden: Beschädigte lokale Speicherung wird abgefangen
- Bestanden: Mobile Breite 375 px: keine horizontale Überbreite; Antworten bedienbar
- Bestanden: Ohne localStorage spielbar, Speichereinschränkung wird angezeigt
- Bestanden: Direkt per index.html vom Dateisystem spielbar
- Bestanden: Keine unbehandelten JavaScript-Fehler im Test

Die Desktop- und mobile Darstellung (375 Pixel Breite) wurden zusätzlich anhand der gerenderten Screenshots visuell angesehen. Die App enthält keine unbehandelten JavaScript-Fehler in den getesteten Abläufen. Es wurde kein echtes GitHub-Repository angelegt und keine Website veröffentlicht; eine tatsächlich ausgeführte GitHub-Pages-Bereitstellung ist daher nicht Bestandteil dieser Prüfung.

## Antwortvergleich

Bei Auswahlfragen ist genau eine angebotene Antwort hinterlegt. Freitext wird gegen gespeicherte Antworten und Varianten verglichen, nicht semantisch durch KI beurteilt. Eine andere richtige Formulierung kann als falsch erkannt werden; die App erklärt diese Grenze und ermöglicht eine manuelle Korrektur der Wertung. Das Aufdecken ohne eigene Antwort zählt als zu wiederholende Frage.

## Nachvollziehbarkeit

`DATENPRUEFUNG.json` enthält Zählungen, Aussonderungsstatistiken und die verwendeten Wikidata-Zuordnungen. SHA-256 der ausgelieferten `questions.js`:

`31c934b832074acc1250e1a3b9da6e4233ad89e17aaa206f87f6ac45773a3187`
