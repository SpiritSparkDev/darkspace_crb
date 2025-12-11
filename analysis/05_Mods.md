**05_Mods — Analyse**
- **Kurzfassung:**: Das Kapitel beschreibt das Mod‑System: Mods sind Sonderregeln, die Fertigkeiten, Aktionen oder Gegenstände einmalig beeinflussen. Charakter‑Mods kosten 100 EP, Gegenstands/Maschinen‑Mods 100 KP. Mods werden einer Begabung zugeordnet; Aktivierungen kosten Stress (Charakter) oder Material (Gegenstand).
- **Wichtig — einheitliche Kosten:** Alle Mods haben standardmäßig dieselben Erwerbskosten: **100 EP** wenn sie als Charakter‑Mod gekauft werden, bzw. **100 KP** wenn sie als Gegenstands-/Maschinen‑Mod eingebaut werden. Abweichungen werden nur dann angegeben, wenn explizit in der Mod‑Beschreibung oder einer Technik‑Tabelle eine andere Zahl genannt wird.
- **Keywords:**: Mods, Begabung, Aktivierung, Stress, Material, EP‑Kosten, KP‑Kosten, Gegenstände, Maschinen, Routiniert, Reflexartig, Zuordnung
- **Indexeintrag:**: `inCopy/2-1_Mods.icml` (StoryTitle="05_Mods" — ungefähre Startzeile: 467)
- **Wichtigste extrahierte Regeln (kurz):**
  - **Mods erhalten:** Eine Charakter‑Mod kostet **100 EP**.
  - **Mods in Gegenständen:** Gegenstände/Maschinen können Mods für **100 KP** erhalten.
  - **Zuordnen:** Mods werden einer **Begabung** zugeordnet; bei einer Probe mit dieser Begabung kann die Mod aktiviert werden und wirkt einmalig.
  - **Aktivierung (Charakter):** Jede Aktivierung verursacht **1 Punkt Stress**.
  - **Aktivierung (Gegenstand):** Gegenstände nutzen **Material** statt Stress; jede Aktivierung verbraucht ein Material.
  - **Allgemein:** Eine Mod wirkt einmalig pro Aktivierung und ist dazu gedacht, besondere Fähigkeiten/Mechaniken darzustellen (Beispiele: **Reflexartig**, **Routiniert**).
- **Offene Fragen / Unklarheiten:**
  - **Limit pro Charakter:** Gibt es ein Limit, wie viele Mods ein Charakter haben oder wie viele einer Begabung zugeordnet werden dürfen? (nicht im gelesenen Abschnitt spezifiziert)
  - **Kumulierung / Stacking:** Dürfen mehrere Mods dieselbe Probe gleichzeitig beeinflussen? Wie verhalten sich modifizierte Würfelmechaniken zueinander?
  - **Aktivierungszeitpunkt / Aktion:** Ist die Aktivierung an eine Aktion gebunden (Vor-/Nach-/Unterbrechung) oder frei während der Probe? (Beispiel „Reflexartig“ deutet auf Unterbrechung hin, aber die allgemeine Regel fehlt)
  - **Materialvorrat bei Gegenständen:** Wie viele Materialien hat ein Gegenstand standardmäßig? Wie wird Materialkapazität bestimmt? (Technik/Konstruktion‑Regeln beziehen sich auf KP/Größe/MK, aber im Mods‑Text fehlen die konkreten Materialregeln)
  - **Kosten‑Interpretation:** Steht die Angabe "Mods eines Gegenstands kosten 100 KP" für einen Pauschalpreis pro Mod zusätzlich zu den Basis‑KP des Gegenstands (Größe/MK), oder sind das alternative Angaben? (siehe Abgleich mit `inCopy/3_Technik.icml` notwendig)
  - **Wiederholbarkeit:** Formulierungen wie "einmalig aktiviert" sprechen dafür, dass Aktivierungen wiederholt möglich sind (gegen Stress/Material) — ist das ausdrücklich so gemeint?
- **Gefundene Widersprüche / Stellen zum Abgleichen:**
  - **KP‑Kosten vs. Technik‑KP‑Tabelle:** In `inCopy/3_Technik.icml` existiert eine ausführliche KP‑Kosten‑Tabelle (Größe × MK → KP). Die Formulierung hier ("Mods für 100 KP") muss mit der Technik‑Tabelle abgeglichen werden: 100 KP pro Mod könnte ein Aufpreis sein oder eine alternative Pauschale — Klärung empfohlen.
  - **Charakter‑KP vs. Gegenstandskostenerläuterung:** Falls in anderen Kapiteln (z. B. `2_Charaktere.icml`) KP‑Werte für Ausrüstung anders dargestellt sind, ist ein Abgleich nötig.
- **Veraltetes / Anmerkungen zur Version:**
  - XMP‑Metadata (Create/Modify) zeigt letzte Änderung `2024-12-10T21:49:53+01:00` — kein offensichtlicher Hinweis auf veraltete Regeln im gelesenen Abschnitt.
- **Empfehlungen / nächste Schritte:**
  - Kurzer Abgleich der Formulierung "100 KP pro Mod" mit der KP‑Tabelle in `inCopy/3_Technik.icml` und mit bereits extrahierten Werten in `analysis/04_Charaktere.md`.
  - Vollständige Extraktion der restlichen Mod‑Definitionen aus `inCopy/2-1_Mods.icml` (weitere Beschreibungen, Beispielmods, evtl. Tabellen), dann Erstellen einer kanonischen Mod‑Tabelle (Name, Kurzbeschreibung, EP/KP‑Kosten, Aktivierungskosten, Wiederholbarkeit, Zuordnung).
  - Klärung offener Fragen, insbesondere Materialkapazität von Gegenständen und Limitierung pro Begabung/Charakter.
- **Provenienz:**: Ausschnitt aus Datei `inCopy/2-1_Mods.icml`, StoryTitle="05_Mods" (ungefährer Lesestart: Zeile 467; XMP: CreateDate 2024-10-14, ModifyDate 2024-12-10).

**Basis‑Mods — extrahierte Definitionen (Tabelle)**

| Mod | Kurzbeschreibung | Aktivierung (Kosten) | EP | KP | Wiederholbar | Provenienz |
|---|---|---:|---:|---:|---:|---|
| Bollwerk | Setzt gegnerische Schwierigkeitsgrade für Aktionen gegen den Charakter auf `10 + Aktivierung × 2`. Gegner‑Routinen werden als verzweifelte Proben ausgeführt (Angreifer kann abbrechen). | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (Block: Basis‑Mods, ~Zeilen 1000–1160)
| Detailarbeit | Erlaubt, einen erfolgreich beendeten Prozess bis zum Ende der nächsten Ruhephase zurückzustellen; erhöht Ergebnis in der nächsten Ruhephase um +2 pro Aktivierung. | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (Block: Basis‑Mods, ~Zeilen 1000–1160)
| Durchbrechen | Ignoriert 1 Unterbrechung pro Aktivierung. | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1000–1160)
| Effizient | Reduziert pro Aktivierung AE‑Kosten einer Aktion oder die Zeitstufe eines Prozesses um 1 (Minimum 1). | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1000–1160)
| Forcieren | Spieler wählt pro Aktivierung eine Zahl 1–9; die Zahl löst die Regel der 10 aus; keine Zahl darf zweimal gewählt werden. Kann auch nach dem Wurf, aber vor der Wirkungsbeschreibung aktiviert werden. | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung (jede Zahl nur einmal) | `inCopy/2-1_Mods.icml` (~Zeilen 1000–1160)
| Reflexartig | Verringert das Ergebnis gegnerischer Proben um 2 pro Aktivierung (Beispiel: Nahkampf‑Konter). | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (Beispieltext, ~Zeilen 820–1043)
| Routiniert | Bei mehrfachen Routine‑Proben in einer Ruhephase: das höchste Ergebnis aus allen Proben gilt für alle Proben (bei Aktivierung). | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 830–1055)
| Versiert | Addiert pro Aktivierung die Fertigkeitsstufe der Probe zusätzlich zum Probeergebnis. | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1000–1160)
| Verstärkt | Pro Aktivierung wird dem Ergebnis entweder die Augenzahl eines weiteren Würfels aus dem Wurf oder +2 hinzugefügt. | 1 Stress / 1 Material | 100 EP | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1000–1160)

_Anmerkung:_ Die allgemeinen Aktivierungskosten (1 Stress für Charakter‑Mods, 1 Material für Ausrüstungs‑/Gegenstands‑Mods) gelten ergänzend; einige Mods erwähnen explizit "pro Aktivierung" oder spezielle Einschränkungen (z. B. Forcieren: Zahl darf nicht mehrfach gewählt werden).

**Technische Mods — extrahierte Definitionen (Tabelle)**

| Mod | Kurzbeschreibung | Aktivierung (Kosten) | KP | Wiederholbar | Provenienz |
|---|---|---:|---:|---:---|
| Angepasst | Nach dem Sortieren der Würfel kann per Aktivierung die Modulklasse des Gegenstands auf einen beliebigen Würfel addiert werden (max Würfelwert 10). Weitere Aktivierungen erlauben zusätzliche Würfel‑Additionen. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1196–1220)
| Ausklinken | Reduziert Größe um 1; heilt Schaden auf einem Monitor vollständig und entfernt die Mod (Gegenstand teilweise zerstört). Kann mehrfach gewählt werden (mehrere Schichten). | 1 Material | 100 KP | pro Aktivierung / mehrfach wählbar | `inCopy/2-1_Mods.icml` (~Zeilen 1220–1244)
| Erhöhte Reichweite | Handlungen haben Reichweite MK² × [Aktivierung] Meter; Angriffe verschieben Ausgangspunkt um MK² × [Aktivierung] Meter. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1244–1256)
| Explosiv | Nach Aktivierung: nach 5 AE/Sekunden Explosion mit Wirkbereich 10 × (Größe² + Modulklasse²). Schaden: [Größe × 2], Durchschlag = Modulklasse. Gegenstand wird zerstört. | 1 Material | 100 KP | wird Verbrauchsdurch Aktivierung (zerstört) | `inCopy/2-1_Mods.icml` (~Zeilen 1256–1276)
| Faltsystem | Gegenstand klappt zusammen / entfaltet sich; zusammengefaltete Nutzung erfordert Aktivierung, Auf-/Zufalten kosten keine Aktivierung. | 1 Material (für Nutzung im gefalteten Zustand) | 100 KP | pro Aktivierung / entfalten kostenlos | `inCopy/2-1_Mods.icml` (~Zeilen 1276–1296)
| Gepanzert | Schützt Träger/verbundene Systeme; senkt eingehenden Schaden um Anzahl Aktivierungen. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1296–1316)
| Hochtechnologie | Pro Aktivierung gilt Modulklasse +1. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1316–1330)
| Kontrollknoten | Leitet Cortex‑Handlungen im Netzwerk zum Knoten; Knoten darf Mods aller Geräte verwenden (muss aktivieren). Dominanz durch höhere MK. Pro Aktivierung +1 Firewall. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1330–1360)
| Regenerativ | Heilt pro Aktivierung 1 TP am eigenen Ziel oder eines verbundenen Monitors (max ≤ Modulklasse). | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1360–1384)
| Parallelisierung | Bei mehrfachen Aktionen mit demselben Gegenstand in einer Handlungsphase: AE‑Kosten jeder weiteren Aktion −1 (min 1 AE). | 1 Material | 100 KP | pro Aktivierung / wirkt passiv auf Folgeaktionen | `inCopy/2-1_Mods.icml` (~Zeilen 1384–1404)
| Triebwerk | Erlaubt Reisen (Ruhephase) — Aktivierung ermöglicht Reisen; Geschwindigkeit nach SL. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1404–1428)
| Unkompliziert | Gerät hat keine Elektronik; darf nicht Ziel von Cortex‑Handlungen sein; bei Aktivierung erhält die Probe einen zusätzlichen Würfel. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1428–1448)
| Vektorschub | Hält Modulklasse in Zeitstufen in der Luft; pro Aktivierung +1 Zeitstufe Flugdauer. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1448–1472)
| Synchronisiert | Zwei Aktivierungen setzen Nebenergebnis auf Hauptergebnis. | 1 Material | 100 KP | 2 Aktivierungen | `inCopy/2-1_Mods.icml` (~Zeilen 1472–1496)

**Technische Handicaps — Kurzliste**

| Handicap | Kurzbeschreibung | Provenienz |
|---|---|---|
| Einseitig | Gerät kann nur eine festgelegte Handlung ausführen. | `inCopy/2-1_Mods.icml` (~Zeilen 1496–1510)
| Fehleranfällig | Würfelpool ist durch Modulklasse begrenzt. | `inCopy/2-1_Mods.icml` (~Zeilen 1510–1528)
| Fehlkalibrierung | Proben mit dem Gegenstand lösen keine Regel der Zehn aus. | `inCopy/2-1_Mods.icml` (~Zeilen 1528–1544)
| Harter Impuls | Nach jeder Handlung mit dem Gegenstand verliert der Charakter 1 AE. | `inCopy/2-1_Mods.icml` (~Zeilen 1544–1560)
| Gefährlich | Bei Misserfolg erleidet Anwender 1 TP. | `inCopy/2-1_Mods.icml` (~Zeilen 1560–1576)
| Schwer | (Eintrag im ICML vorhanden; Textabschnitt weiter unten) | `inCopy/2-1_Mods.icml` (~Zeilen 1576–1600)

**Waffenmods — extrahierte Definitionen (Tabelle)**

| Mod | Kurzbeschreibung | Aktivierung (Kosten) | KP | Wiederholbar | Provenienz |
|---|---|---:|---:|---:---|
| Besondere Form | Handlungen ohne Schaden: Ergebnis + doppelte Aktivierungen. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1600–1620)
| Dauerangriff | Pro Aktivierung +1W, aber Ergebnis −1. Jede zweite Aktivierung: Schaden +1 und AE +1. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1620–1640)
| Energiewaffe | Pro Aktivierung Durchschlag + MK; jede weitere Aktivierung +1 Durchschlag. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1848–1864)
| Lädieren | Bei Schaden: würfle 1W10; bei 10 Ziel erleidet erneut Schaden; weitere Aktivierungen erweitern Trefferbereich. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1864–1884)
| Panzerbrechend | Aktivierung reduziert Zielpanzerung dauerhaft (MK −1). | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1884–1904)
| Reichweitenvorteil | Pro Aktivierung ideale Reichweite um eine Kategorie erhöhen. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1904–1920)
| Schalldämpfer | Aktivierung: Angriff erzeugt keine SE. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1920–1936)
| Schock | Nach Treffer: Aktivierung erhöht AE‑Kosten des Ziels um 1 (Dauer bis Ende nächste Handlungsphase); weitere Aktivierungen erhöhen Dauer. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1936–1960)
| Streuung | Pro Aktivierung trifft 1 zusätzliches Ziel. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1960–1976)
| Werfer | Waffe kann Objekte verschießen; Aktivierung ignoriert Zieldeckung. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1976–1996)
| Zielsuchend | Aktivierung setzt alle Würfel auf 6. | 1 Material | 100 KP | pro Aktivierung | `inCopy/2-1_Mods.icml` (~Zeilen 1996–2012)

**Waffenmods — Aktivierungsübersicht**

| Aktivierungen | W | Ergebnis | Schaden | AE |
|---:|---:|---:|---:|---:|
| 1 | +1 | −1 | +0 | +0 |
| 2 | +2 | −2 | +1 | +1 |
| 3 | +3 | −3 | +1 | +1 |
| 4 | +4 | −4 | +2 | +2 |
| 5 | +5 | −5 | +2 | +2 |

**Waffen‑Handicaps — Kurzliste**

| Handicap | Kurzbeschreibung | Provenienz |
|---|---|---|
| Lademechanismus | Vor Angriff muss Routine zum Laden durchgeführt werden; bei Probe <10: Ladehemmung (muss mit Aktivierung+Routine beseitigt werden). | `inCopy/2-1_Mods.icml` (~Zeilen 2012–2032)
| Nicht‑Tödlich | Waffe verursacht nur Betäubungsschaden. | `inCopy/2-1_Mods.icml` (~Zeilen 2032–2044)
| Verringerte Reichweite | Reichweite Fernkampf −1 Kategorie; Nahkampf: Waffe gilt kleiner im Größenvergleich. | `inCopy/2-1_Mods.icml` (~Zeilen 2044–2060)

**Provenienz (gesamt):** Inhalte aus `inCopy/2-1_Mods.icml`, Abschnitte "Technische Mods" (~Zeilen 1196–1520) und "Waffenmods" (~Zeilen 1600–2072). 
**Klärung: KP‑Kosten / "100 KP pro Mod"**
 
 - **Was die Texte explizit sagen:** In `inCopy/2-1_Mods.icml` steht klar: *"Die KP‑Kosten für Mods entsprechen den EP‑Kosten bei Charakteren und kosten 100 KP pro Mod."* (siehe ~Zeile 863). Außerdem findet sich im Kapitel ein kleines Tabellenfragment *"Mod hinzufügen / Handicap entfernen — 100 KP*" (Technik‑Bereich, siehe `inCopy/3_Technik.icml`).
 - **Kontext aus `inCopy/3_Technik.icml`:** In der Technik‑Datei werden vielfach KP‑Werte tabellarisch angegeben; manche Zellen enthalten zwei Werte, z. B. `80 KP (100 KP)`. Direkt oberhalb der Tabelle steht die Erläuterung: *"Zahlen in Klammern sind fertig addierte KP‑Kosten um die gewünschte Stufe direkt zu kaufen."* (siehe `inCopy/3_Technik.icml`, ~Zeile 4902).
 
 - **Interpretation / abgeleitete Regel:**
   - Die Regelformulierung im Mods‑Kapitel legt einen *Pauschalpreis von 100 KP pro Mod* nahe (analog zu 100 EP für Charakter‑Mods). Das ist die einfache, explizite Anweisung für Design/Spielleitung.
   - Die Technik‑Tabelle zeigt dagegen auch *fertig addierte Totalsummen in Klammern*; diese Klammern stellen Komfortwerte dar für das direkte Kaufen oder Vor-Konfigurieren einer Stufe (also bereits summierte Kosten), nicht unbedingt eine alternative Preisliste, die die 100‑KP‑Regel außer Kraft setzt.
   - Daher ist die praktisch sinnvollste Konsolidierung: **Benutze die Technik‑Tabelle als Quelle für die Basis‑KP eines Gegenstands (Größe × MK) und addiere für jede zusätzliche Mod standardmäßig 100 KP**, es sei denn, eine spezifische Mod‑Beschreibung nennt eine abweichende KP‑Angabe oder die Technik‑Tabelle liefert als (in Klammern) explizite Komplettpreise für ein bestimmtes konfiguriertes Produkt.
 
 - **Konkreter Vorschlag / Empfehlung:**
   1. Formuliere in der endgültigen Fassung der Regeln explizit: *"Mods auf Gegenständen kosten standardmäßig 100 KP zusätzlich zur Basis‑KP des Gegenstands (Größe × MK). Ausnahmen werden in der Mod‑Beschreibung genannt. Zahlen in Klammern in der Technik‑Tabelle sind fertig addierte Kaufpreise für Komfort; sie können als Abkürzung benutzt werden."*
   2. Markiere in `analysis/05_Mods.md` alle Mods, die eine abweichende KP‑Angabe enthalten, und verlinke auf die relevante Technik‑Tabelle‑Zeile (ich kann das automatisch ergänzen, wenn du willst).
 
 - **Provenienz der Klärung:**
   - `inCopy/2-1_Mods.icml` (Text: *"Die KP‑Kosten für Mods ... kosten 100 KP pro Mod."*, ~Zeile 863)
   - `inCopy/3_Technik.icml` (Erläuterung: *"Zahlen in Klammern sind fertig addierte KP‑Kosten ..."*, ~Zeile 4902; Tabelle mit Beispielen: Zeilen ~4940–5064)
 
 _Status:_ Abgleich durchgeführt; Empfehlung oben ins `analysis/05_Mods.md` eingetragen. Wenn du möchtest, setze ich nun alle relevanten Mod‑Einträge auf explizite KP‑Spalte (Standard: 100 KP) und markiere Ausnahmen anhand der Technikstabelle.
 
```

