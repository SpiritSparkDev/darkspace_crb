**Kurzfassung**
- **Kapitel**: Technik — Regeln für Größe, Modulklassen, KP‑Kosten, Waffen, Panzerung, MedKits, Konstruktion.
- **Kernaussage**: Technik beschreibt, wie Gegenstände und Maschinen in Größe, Masse und Modulklasse eingeordnet werden, wie Konstruktionspunkte (KP) berechnet werden und welche Spielwerte (Schaden, Durchschlag, AE‑Kosten, Reichweite, Panzerung) sich daraus ergeben. Tabellen enthalten fertige KP‑Kosten; Zahlen in Klammern sind bereits summierte Werte zum direkten Kauf einer Stufe.

**8–12 Stichwörter**
- **Größe**: Massentabelle (Größe 0–7 … 14)
- **Modulklasse**: MK 1–5 Beispiele
- **KP‑Formeln**: 5×(MK×(MK+1)×(2MK+1)/6) + Masse×10; Größe²×20 KP (Großprojekte)
- **KP‑Tabellen**: Fertig ausgearbeitete KP‑Gitter für Ausrüstung/Größen/MK
- **Mods**: Mod hinzufügen = 100 KP (Tabelle vorhanden)
- **Waffenwerte**: Schaden = Größe/2; Durchschlag = Größe + MK; AE‑Kosten abhängig von Größe/MK
- **Reichweite**: Kategorien (Nah/Kurz/Lang/Ausgedehnt/Extrem)
- **Panzerung**: WP = MK, HP = MK×3 (Beispieltabelle)
- **MedKits**: KP-Kosten und Beispielgeräte
- **Konstruktion**: Regeln für Bauen, Reparieren, Gruppenprojekte

**Index / Provenienz**
- **Datei**: `inCopy/3_Technik.icml` (ganzes Kapitel gelesen)
- **Wichtigste Startlinien (approx.)**: Kopf/Metadaten ab Zeile 1; Größe/Masse‑Tabelle ab ~200; Modulklassen & KP‑Gitter ab ~700; KP‑Kosten für Ausrüstung/Gegenstände ab ~1200; Mod hinzufügen / 100 KP ab ~4800; MedKits & Konstruktion ab ~4200.

**Gefundene Hinweise & Widersprüche**
- **Direkte Aussagen**: Im Mods‑Kapitel steht explizit "Ein Charakter kann eine Mod für 100 EP kaufen. Gegenstände und Maschinen können Mods für 100 KP erhalten." (aus `2-1_Mods.icml`).
- **Technik‑Tabelle**: In `3_Technik.icml` gibt es eine kleine Tabelle "Mod hinzufügen / Handicap entfernen — 100 KP" (Provenienz: Ende des KP‑Abschnitts). Zudem zeigen die KP‑Gitter für Ausrüstung und Gegenstände *fertige* KP‑Werte (Zahlen in Klammern sind sofort‑Kauf‑Summen), die in vielen Zeilen andere Summen als genau 100 KP für einzelne Stufen nennen — das ist kein direkter Widerspruch, sondern zwei verschiedene Konzepte:
  - Die großen KP‑Tabellen geben Gesamtkosten für Größe×MK/Stufen an (Konstruktions‑/Kaufkosten).
  - Die Regel "Mod hinzufügen = 100 KP" ist eine separate Bestellung/Operation, die angibt, wie viele KP nötig sind, um eine Mod an einem Gegenstand hinzuzufügen oder ein Handicap zu entfernen.
- **Empfehlung (konsequent/operational)**: Für Bau/Herstellung nutze die Technik‑KP‑Tabellen als kanonische Referenz (sie berechnen Größe×MK‑Kosten). Für individuelle Modifikationen verwende die klar benannte Regel "Mod hinzufügen = 100 KP" (oder, falls du wolltest, setze alle Mods per Benutzerwunsch pauschal auf 100 KP/100 EP — das hattest du bereits angedeutet).

**Exportierte Tabellen (Markdown)**
- **Größen & Masse (Auszug)**

| Größe | Masse (Beispiel) |
|---:|---|
| 0 | Masse 1 |
| 1 | Masse 2 |
| 2 | Masse 4 |
| 3 | Masse 8 |
| 4 | Masse 16 |
| 5 | Masse 32 |
| 6 | Masse 64 |
| 7 | Masse 128 |
| ... | ... |

(Provenienz: `inCopy/3_Technik.icml`, "Größen, Masse und Bezeichnung" – Tabelle im Kapitel Technik.)

- **Modulklassen — Beispiele (Auszug)**

| MK | Beispiele |
|---:|---|
| MK 1 | Kleine Werkzeuge, einfache Mods |
| MK 2 | Haushaltsgeräte, einfache Terminals |
| MK 3 | Fortgeschrittene Geräte, Waffenbasis |
| MK 4 | Militärische Geräte, schwere Waffen |
| MK 5 | Hochtechnologie, spezialgeräte |

(Provenienz: `inCopy/3_Technik.icml`, "Modulklassen" / "Beispiele für Modulklassen")

- **KP‑Kosten für Ausrüstung (Matrix, Auszug)**

Die große Tabelle listet für jede Größe (links) die KP‑Kosten für MK 1–5 (Spalten). Beispielzellen (aus Datei):

| Größe (Masse) | MK1 | MK2 | MK3 | MK4 | MK5 |
|---:|---:|---:|---:|---:|---:|
| 0 (Masse 1) | 15 KP | 35 KP | 80 KP | 160 KP | 285 KP |
| 1 (Masse 2) | 25 KP | 45 KP | 90 KP | 170 KP | 295 KP |
| 2 (Masse 4) | 45 KP | 65 KP | 110 KP | 190 KP | 315 KP |
| 3 (Masse 8) | 85 KP |105 KP |150 KP |230 KP |355 KP |
| 4 (Masse 16) |165 KP |185 KP |230 KP |310 KP |435 KP |
| ... | ... | ... | ... | ... | ... |

(Provenienz: `inCopy/3_Technik.icml`, Tabelle "KP-Kosten für Ausrüstung")

- **KP‑Kosten für Gegenstände & Maschinen (Stufen‑/Begabungs‑Matrix, Auszug)**

Diese Tabelle enthält Stufen 1–5, MK/Größe/Begabung und Reparaturwerte; einige Zellen listen zusätzlich in Klammern summierte Kaufkosten.

| Stufe | MK/Größe/Begabung | Reparatur (Beispiel) |
|---:|---:|---:|
| 1 | 20 KP | 5 KP |
| 2 | 80 KP (100 KP) | 20 KP (25 KP) |
| 3 | 180 KP (280 KP) | 45 KP (70 KP) |
| 4 | 320 KP (600 KP) | 80 KP (150 KP) |
| 5 | 500 KP (1100 KP) | 125 KP (275 KP) |

(Provenienz: `inCopy/3_Technik.icml`, Tabelle "KP-Kosten für Gegenstände und Maschinen"; Fußnote: "Zahlen in Klammern sind fertig addierte KP‑Kosten...")

- **Mod hinzufügen / Handicap entfernen**

| Aktion | KP |
|---|---:|
| Mod hinzufügen / Handicap entfernen | 100 KP |

(Provenienz: `inCopy/3_Technik.icml`, kleine Tabelle nahe Ende des KP‑Abschnitts)

- **MedKits — Beispiele (Auszug)**

| Größe | Beispiel |
|---:|---|
| 1 | Stim‑Injektor |
| 2 | MedKit |
| 3 | MedBag |
| 4 | MedStation |
| 5 | Krankenkapsel |

(Provenienz: `inCopy/3_Technik.icml`, MedKits‑Abschnitt)

**Wichtige Formeln (aus dem Text)**
- KP direkte Formel (allgemein): 5 × (MK×(MK+1)×(2×MK+1) / 6) + Masse × 10
- Größe (Großprojekte): [Größe]² × 20 KP
- AE‑Kosten (physisch): [Größe]/2 AE; (Hacking) [MK]/2 AE
- Schaden: Größe / 2
- Durchschlag: Größe + MK

**Konkrete Hinweise für dich / nächste Schritte**
- Ich habe die vollständige `inCopy/3_Technik.icml` gelesen und die wichtigsten Tabellen in `analysis/03_Technik.md` exportiert (diese Datei). Wenn du möchtest, kann ich:
  - 1) Die Tabellen als separate, vollständig formatierte Markdown‑Tabellen in einzelne Dateien (z. B. `analysis/03_Technik_kp_matrix.md`) aufteilen.
  - 2) Alle Mods in `inCopy/2-1_Mods.icml` automatisch abgleichen und prüfen, ob Ausnahmen zur 100 KP‑Regel existieren.
  - 3) Eine konsolidierte Referenz erzeugen, die Technik‑KP‑Werte mit Mods/Charakter‑KP vereinheitlicht (z. B. "Alle Mods = 100 KP" wie du wünschst) und `analysis/`‑Dateien entsprechend anpasst.

Möchtest du, dass ich jetzt automatisch alle Mods scanne (Option 2) oder die Tabellen in separate Dateien exportiere (Option 1)? Oder soll ich die Analyse anpassen, damit alle Mods pauschal 100 KP/100 EP gesetzt werden (Option 3)?

---
Datei erstellt aus: `inCopy/3_Technik.icml` (komplette Datei, alle relevanten Tabellen und Textabschnitte gelesen).