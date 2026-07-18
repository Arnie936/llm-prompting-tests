# Micron-Quartalsbericht-Video mit Hyperframes und deutschem ElevenLabs-Voice-over

```text
Erstelle auf Grundlage des neuesten Micron-Quartalsberichts ein ungefähr einminütiges Video im 16:9-Format, das die wichtigsten Finanzzahlen und den zukünftigen Ausblick verständlich, visuell stark und professionell zusammenfasst.

Ziel:
- Erstelle ein kurzes deutschsprachiges Finanz-Erklärvideo über Micron Technology.
- Das Video soll die aktuellsten Quartalszahlen, zentrale Treiber und den Ausblick zusammenfassen.
- Nutze Diagramme, Grafiken, Kennzahlen-Karten und animierte visuelle Elemente.
- Füge ein deutsches Voice-over mit ElevenLabs hinzu.
- Verwende eine dezente Lofi-Hintergrundmusik, die leise genug gemischt ist, damit das Voice-over klar verständlich bleibt.

Datenbasis:
- Verwende den neuesten verfügbaren Micron-Quartalsbericht als primäre Quelle.
- Suche zusätzlich nach offiziellen Micron-Investor-Relations-Materialien, Earnings Releases, Präsentationen oder SEC-Filings, falls nötig.
- Nenne im Projekt oder in den Metadaten die verwendeten Quellen.
- Verwende keine erfundenen Finanzzahlen.
- Falls eine Zahl nicht eindeutig belegbar ist, markiere sie als „nicht eindeutig aus Quelle ableitbar“ und lasse sie im Video lieber weg.

Inhaltliche Anforderungen:
- Zeige die wichtigsten Finanzkennzahlen des neuesten Quartals, z. B. Umsatz, Bruttomarge, operatives Ergebnis, Gewinn/Verlust pro Aktie, Cashflow oder andere relevante Kennzahlen aus dem Bericht.
- Erkläre die wichtigsten Geschäftsbereiche oder Treiber, insbesondere DRAM, NAND, HBM, Rechenzentrum, KI-Nachfrage oder andere im Bericht genannte Segmente.
- Fasse den Ausblick des Managements zusammen: Guidance, Nachfrageentwicklung, Margenerwartungen, Risiken und Chancen.
- Vermeide Anlageberatung. Formuliere neutral und analytisch.

Videoformat:
- Seitenverhältnis: 16:9
- Länge: ungefähr 60 Sekunden
- Sprache: Deutsch
- Stil: modern, clean, tech-finance, leicht futuristisch, aber nicht überladen
- Zielgruppe: interessierte Anleger, Tech- und KI-Interessierte

Animation:
Verwende Hyperframes für die Animation:
https://github.com/heygen-com/hyperframes

Setze Hyperframes ein, um z. B. folgende Szenen zu animieren:
- Intro mit Micron-/Halbleiter-/Speicherchip-Visual
- KPI-Karten mit den wichtigsten Quartalszahlen
- Balken- oder Linienchart für Umsatz, Marge oder Segmententwicklung
- Grafische Darstellung von KI-/HBM-Nachfrage und Rechenzentrumswachstum
- Ausblick-Szene mit Chancen/Risiken
- Abschluss-Slide mit neutralem Fazit

Voice-over:
- Erzeuge ein deutsches Voice-over mit ElevenLabs.
- Verwende diesen ElevenLabs-API-Key als Platzhalter, der lokal oder per Environment Variable ersetzt werden soll:
  [API-KEY EINFÜGEN]
- Der API-Key darf nicht hartcodiert in öffentlich sichtbare Dateien, Logs oder Commits geschrieben werden.
- Empfohlen: `ELEVENLABS_API_KEY` als Environment Variable verwenden.
- Stimme: professionell, klar, ruhig, deutschsprachig, finance-/YouTube-tauglich.
- Tempo: natürlich, nicht zu schnell, passend für ca. 60 Sekunden.

Hintergrundmusik:
- Verwende eine Lofi-MP3 als Hintergrundmusik.
- Suche eine passende lizenzfreie Lofi-MP3 im Web oder erstelle eine passende Musikspur mit ElevenLabs, falls verfügbar.
- Achte auf Nutzungsrechte und dokumentiere die Quelle der Musik.
- Mische die Musik deutlich leiser als das Voice-over, z. B. ungefähr -22 bis -28 LUFS relativ/dezent, sodass Sprache immer klar verständlich bleibt.
- Nutze bei Bedarf Ducking/Sidechain-Kompression oder automatische Lautstärkereduktion unter dem Voice-over.

Skriptvorschlag:
- Schreibe zuerst ein kurzes deutsches Voice-over-Skript für ungefähr 60 Sekunden.
- Das Skript soll die Zahlen und den Ausblick sachlich zusammenfassen.
- Danach generiere daraus das Voice-over.
- Schneide Animationen, Diagramme, Voice-over und Musik zu einem finalen Video zusammen.

Technische Anforderungen:
- Erstelle ein reproduzierbares Projekt mit klarer Ordnerstruktur, z. B. `src/`, `assets/`, `output/`, `scripts/`.
- Dokumentiere Setup und Ausführung in einer README.
- Verwende Hyperframes für die animierten Szenen.
- Verwende ffmpeg oder ein vergleichbares Tool für finalen Schnitt, Audio-Mix und Encoding.
- Exportiere das finale Video als MP4 in 1080p, 16:9.
- Stelle sicher, dass Audio korrekt synchronisiert ist.

Qualitätskontrolle:
- Prüfe, ob alle genannten Finanzzahlen aus offiziellen Quellen stammen.
- Prüfe, ob das Video ungefähr eine Minute lang ist.
- Prüfe, ob das Ausgabeformat 16:9 ist.
- Prüfe, ob das Voice-over klar verständlich ist und nicht von der Musik überdeckt wird.
- Prüfe, ob das finale MP4 abspielbar ist.
- Gib am Ende aus:
  - Pfad zur finalen MP4-Datei
  - verwendete Quellen
  - verwendete Musikquelle
  - verwendete Tools
  - kurze Zusammenfassung der wichtigsten Micron-Aussagen
```
