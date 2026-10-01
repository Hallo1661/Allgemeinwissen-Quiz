# Herkunft und Lizenzen

## 1. Wikidata: 2.683 Werkfragen

Die Daten stammen aus [Wikidata](https://www.wikidata.org/), bereitgestellt durch die Wikidata-Gemeinschaft unter [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). Die [Wikidata-Lizenzrichtlinie](https://www.wikidata.org/wiki/Wikidata:Licensing) stellt die strukturierten Daten unter CC0 bereit.

Abruf: 1. Oktober 2026. Genutzte Beziehungen: [P50 – Autor](https://www.wikidata.org/wiki/Property:P50), [P170 – Urheber](https://www.wikidata.org/wiki/Property:P170) und [P86 – Komponist](https://www.wikidata.org/wiki/Property:P86). Ausgangspunkt waren in mehreren Sprachversionen vertretene Personen und Werke mit einer deutschen Wikipedia-Seite. Die Werk- und Personennamen wurden aus den lokal gespeicherten Abfrageergebnissen bzw. Einzeldatensätzen übernommen.

Änderungen: Auswahl, Zusammenfassung doppelter Werk-IDs, Ausschluss unklarer Fälle, Formulierung deutscher Fragevorlagen, Ergänzung hinterlegter Antwortvarianten, Kategorien sowie drei falsche Auswahlantworten aus anderen Personen desselben Themenbestands. Die Vorlagen fragen verschiedene reale Werke ab; es wurden keine erfundenen Werkzuordnungen und keine künstlichen Zahlenschleifen zur Mengensteigerung erzeugt. Jede Werk-ID kommt nur einmal vor. Fragevorlagen und auf CC0-Fakten beruhende Aufbereitung können ebenfalls unter CC0 verwendet werden.

Jede Frage mit ID `wd-...` enthält den Link zur passenden Wikidata-Eigenschaft und zur deutschen Wikipedia-Seite des Werks. `DATENPRUEFUNG.json` hält die verwendeten Werk-, Eigenschafts- und Antwort-IDs sowie den verfügbaren Prüfstatus fest. Verlinkte Webseiten können sich nach dem Abruf ändern. Die App enthält keine aus diesen Wikipedia-Werkartikeln kopierten Volltexte.

## 2. GermanQuAD: 330 redaktionell ausgewählte Fragen

Quelle: [deepset/GermanQuAD auf Hugging Face](https://huggingface.co/datasets/deepset/germanquad), insbesondere die [Datensatzbeschreibung mit Lizenz](https://huggingface.co/datasets/deepset/germanquad/blob/main/README.md). Datensatzlizenz: [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).

Urheberinnen und Urheber des Datensatzes laut Beschreibung: Timo Möller, Julian Risch, Malte Pietsch, Julian Gutsch, Tom Hersperger, Luise Köhler, Iuliia Mozhina und Justus Peter, deepset.

Wissenschaftliche Referenz: Timo Möller, Julian Risch und Malte Pietsch (2021), *GermanQuAD and GermanDPR: Improving Non-English Question Answering and Passage Retrieval*. [Veröffentlichung](https://aclanthology.org/2021.mrqa-1.4/).

Verwendete Datenfassungen: die gespeicherte Parquet-Konvertierung des Trainings- und Testbestands unter `refs/convert/parquet/plain_text/train/0000.parquet` bzw. `test/0000.parquet` des deepset/germanquad-Repositorys. Ausgangszahlen: 11.518 Trainings- und 2.204 Testfragen. Abruf am 1. Oktober 2026.

Änderungen: Auswahl kurzer beantwortbarer Fragen; Ausschluss vieler zeitabhängiger, fehlerhafter oder unklarer Einträge; Überarbeitung von Grammatik und Fragestellung; Kürzung von Musterantworten; Ergänzung gleichwertiger Schreibweisen; Zuordnung zu Kategorien. Die ursprüngliche Split- und Frage-ID bleibt als `originalId` und im Präfix `gq-...` erhalten. Die bearbeiteten Fragen und Antworten stehen weiterhin unter CC BY 4.0. Es wird keine Unterstützung dieser App durch deepset behauptet.

### Hintergrundpassagen aus Wikipedia

Die GermanQuAD-Hintergrundtexte stammen aus historischen Fassungen der deutschen Wikipedia. Urheber sind die jeweiligen Wikipedia-Autorinnen und -Autoren, erreichbar über den in jeder Frage mitgelieferten Artikel- und Versionsgeschichtslink. Diese Texte werden mit Quellenangabe unter [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) weitergegeben; maßgeblich sind die Lizenzangaben der zugrunde liegenden Wikipedia-Fassung. Die hier vorgenommenen Änderungen beschränken sich auf die Textdarstellung, insbesondere entfernte Wiki-Formatzeichen und Überschriftsmarkierungen. Die historischen Texte wurden nicht auf einen vollständigen aktuellen Stand gebracht. Die Datensatzlizenz ersetzt nicht die Namensnennung und Share-Alike-Bedingungen dieser Wikipedia-Passagen.

## 3. App-Code

HTML, CSS, JavaScript-Programmlogik und SVG-Signet stehen unter der MIT-Lizenz in `LICENSE-CODE.txt`. Die MIT-Lizenz überträgt sich nicht auf die GermanQuAD-Fragen und Wikipedia-Hintergrundtexte. Es werden keine externen Schriftarten, Fotos, Frameworks oder kostenpflichtigen Bibliotheken ausgeliefert.

Die Quellen- und Lizenzdateien sowie die Herkunftsinformationen in `questions.js` beim Hochladen und Weitergeben beibehalten.
