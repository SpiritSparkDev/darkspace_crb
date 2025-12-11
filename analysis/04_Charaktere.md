# 04_Charaktere — Zusammenfassung & gefundene Probleme

- **Datei:** `inCopy/2_Charaktere.icml`
- **Story/Title:** `04_Charaktere`
- **Bereich gelesen:** Kapitelinhalt ab Storybeginn bis KP‑Tabellen (ungefähr Zeilen 1–4800 beim chunked read).

## Kurzfassung
- Kapitel behandelt Charakterkonzept und -erstellung: Hintergrund‑Würfeltabellen (Kultur, Feinde, Traumata, glückliche Wendungen etc.), Spielwerte (Begabungen, Fertigkeiten, Mods, Artifizierungen, Spezialisierungen, Ausrüstung), Startpunkte (EP/KP), EP‑Kosten (direkter Kauf & Entwicklung), Mods (Preis 100 EP, Aktivierung über Stress) und Startausrüstung/KP‑Kosten.

**Wichtige Fakten (kompakt)**

**Tabellen (EP / KP) — aus `inCopy/2_Charaktere.icml`**

- **Quelle:** `inCopy/2_Charaktere.icml` (chunked read, Zeilen ~2400–4800)

## Start-Erfahrung

| Startpunkte | Beschreibung |
|---:|---|
| 1000 | Kompletter Anfänger: Der Charakter hat in seinem Leben nur absolut notwendige Dinge gelernt. |
| 2000 | Neuling: Der Charakter hat sich oberflächlich mit verschiedenen Disziplinen beschäftigt und vielleicht ein Interesse in einer davon entwickelt. |
| 3000 | Versiert: Der Charakter hat mindestens eine Sache, in der er wirklich gut ist. |
| 4000 | Profi: Der Charakter ist ein absoluter Profi in dem, was er tut. |

### EP‑Kosten (direkter Kauf)

| Stufe | Begabungen | Fertigkeit |
|---:|---:|---:|
| 1 | - | 5 EP |
| 2 | - | 25 EP |
| 3 | 180 EP | 70 EP |
| 4 | 500 EP | 150 EP |
| 5 | 1000 EP | 275 EP |

### EP‑Kosten (Entwicklung)

| Stufe | Begabungen | Fertigkeit |
|---:|---:|---:|
| 1 | - | 5 EP |
| 2 | - | 20 EP |
| 3 | 180 EP | 45 EP |
| 4 | 320 EP | 80 EP |
| 5 | 500 EP | 125 EP |

### KP‑Kosten für Startausrüstung

| Größe | MK 1 | MK 2 | MK 3 | MK 4 | MK 5 |
|---|---:|---:|---:|---:|---:|
| 0 (Masse 1) | 3 KP | 15 KP | 42 KP | 90 KP | 165 KP |
| 1 (Masse 2) | 6 KP | 30 KP | 84 KP | 180 KP | 330 KP |
| 2 (Masse 4) | 12 KP | 60 KP | 168 KP | 360 KP | 660 KP |
| 3 (Masse 8) | 24 KP | 120 KP | 336 KP | 720 KP | 1320 KP |
| 4 (Masse 16) | 48 KP | 165 KP | 185 KP | 230 KP | 310 KP | 435 KP |

Hinweis: Das Original‑ICML‑Chunk endete beim Lesen teilweise; Zeile für Größe 4 enthält mindestens den Eintrag `48 KP` (MK1). Wenn du die vollständige Zeile für Größe 4 (MK2–MK5) brauchst, extrahiere ich den nächsten Chunk und ergänze die fehlenden Zellen.

---

Wenn du mehr Tabellen möchtest (z. B. komplette Mod‑Listen oder Handlanger‑Tabellen), sage `weiter` und ich extrahiere die nächsten Abschnitte ebenfalls als Markdown und füge sie dem Kapitel hinzu.
## Dokumentierte Widersprüche, Fehler und Unklarheiten
[x] Begriffsambiguität: Geklärt
[x] EP‑Kosten‑Tabellen vs. Textformulierung: Durch Befragungen von Spielenden geklärt.
[x] Rundungsregel beim Start‑Einkauf: Geklärt
[x] Mods: Aktivierungskosten (Stress) nicht vollständig numerisch spezifiziert
[x] Handicaps ↔ Stress‑Interaktion unpräzise
[ ] Verweise / Seitennummern potenziell veraltet
   - Problem: Viele Cross‑References (z. B. Stress S.22, Mods S.50, Handicaps S.51) können durch Layoutänderungen inkonsistent werden.
   - Empfehlung: Prüfen nach finalem Layout und optional interne Anker/IDs statt statischer Seitenzahlen verwenden.
[ ] Konversion übriggebliebener Startpunkte

[ ] Tabelle „KP‑Kosten für Startausrüstung" enthält viele Zahlen — aber Kontext/Einheiten fehlen
   - Problem: KP vs. reale Kosten/Balance — ohne Beispiele schwer nachzuvollziehen.
   - Empfehlung: Mindestens 1–2 Beispielcases (Einkommen X → Materialpunkte Y → Einkauf einer Waffe MK Z → KP‑Abzug) beifügen.

**Kurze Priorisierte ToDos / Vorschläge zur Korrektur**
- Sofort (hoch): Ergänze klare Definitionen / Legende bei den EP‑/KP‑Tabellen und ein kurzes Rechenbeispiel für jede kritische Regel (Begabungen, Fertigkeiten, Mod‑Aktivierung, Handicaps).
- Mittel: Prüfe und vereinheitliche Cross‑References (nutze Anker statt statischer Seitenzahlen falls möglich).
- Niedrig: Ergänze FAQs oder Beispiele im Kapitel, um typische Missverständnisse zu vermeiden.

**Quellen / Kontext**
- Dieser Report basiert auf dem chunked read von `inCopy/2_Charaktere.icml` (Zeilenbereich ~1–4800). XMP/CDATA (Bilder/Base64) wurde beim Einlesen gekürzt und nicht in voller Länge gespeichert.

Wenn du willst, exportiere ich jetzt die EP‑/KP‑Tabellen als Markdown‑Tabellen in `analysis/` (Standard) oder als CSV (falls du die Zahlen z. B. in Excel weiterverarbeiten willst). Sage mir kurz: `Markdown` oder `CSV` — dann erledige ich das und markiere den Task als erledigt.
