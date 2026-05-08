# Manus-Auftrag: Logo-Briefing Patches + Schattenwerk LP Konzept

> **Datum:** 2026-05-08 | **Session:** MK_S030
> **Zwei Aufgaben, parallel ausfuehrbar.**

---

## AUFGABE A — Logo-Briefing Ableitung C patchen (4 Patches)

Du hast das Logo-Briefing in `/home/ubuntu/manus_hub/Outputs/brand_design/schattenwerk_ableitung_c_logo_briefing.md` erstellt. Es wurde reviewed — Ergebnis: CONDITIONAL PASS. 4 Patches noetig, kein Blocker.

### Patch 1 — Lena-Voss-Zuordnung

Lena Voss gehoert zum Cluster WSM_SCHADENMANAGER (thematisch und praktisch zu wsm-schaden.de), NICHT als eigenstaendige Marke.

In §1 nach der Produktmarken-Zeile ergaenzen:
> "Lena Voss gehoert zum Cluster WSM_SCHADENMANAGER und wird aus dessen Blocklogik mit blauem Scan-/Wasserlicht abgeleitet. Sie erscheint in der Produktmarken-Tabelle §5 unter WSM."

UND in §5 Produktmarken-Tabelle eine Zeile ergaenzen:

| Lena Voss | WSM | Wortmarke mit forensischer Praezisionskante; blauer Clusterakzent |

### Patch 2 — Farbtoken #f2f0ea ersetzen

`light.mycelium #f2f0ea` existiert in keinem etablierten Farbsystem (weder COLOR_SYSTEM.md noch AUFTRAG_CD_SYSTEM.md).

Aktion: In §2 Farbtabelle `light.mycelium #f2f0ea` ersetzen durch `contrast.text #e8e6e3` (etablierter Token aus beiden Systemen). Kein neuer Token ohne Not.

### Patch 3 — Farbsystem-Quellenhinweis

Am Anfang von §2 oder als Fussnote ergaenzen:

> "Dieses Briefing referenziert das CD-Farbsystem (AUFTRAG_CD_SYSTEM.md), nicht das LP-Farbsystem (COLOR_SYSTEM.md). Abweichungen bei Cluster-Signalfarben und Dachmarken-Palette sind systembedingt. Harmonisierung der zwei Systeme steht als separater Arbeitsschritt aus."

### Patch 4 — Typo-Pool Font-Namen ergaenzen

Pool-Tabelle in §6 um konkrete Font-Namen ergaenzen (entschieden MK_S030, 2026-05-08):

| Pool | Rolle | Font | Einsatz im Logo-System |
|---|---|---|---|
| Pool A — monolithisch | Dachmarke, Autoritaet, Schwere | **Big Shoulders Display** | SCHATTENWERK-Wortmarke, grosse Titel, Systemanker |
| Pool B — handwerklich-industrial | Werkstatt, Produktenergie, Kanten | **IBM Plex Sans** | KI_APPS-Produkte, Kampagnen, markante Subheads |
| Pool C — sachlich-lesbar | Akte, UI, Dokumentation | **Inter** | WSM, WURZELWERK, Labels, Navigation, technische Anwendungen |

Satz "Es wird keine skizzenhafte Hauptschrift eingesetzt" bleibt.

**HALT nach allen 4 Patches. Gepatchte Datei zeigen.**

---

## AUFGABE B — Schattenwerk Landing Page Konzept (Text, kein Code)

Phase 2 des CD-Systems beginnt. Erste Seite: Schattenwerk als Dachmarken-Foyer.

### Was du wissen musst

- Das CD-System ist komplett (Schritte 1–6, Final-GO erteilt).
- Alle 13 Marken, 3 Cluster, 20 Token sind definiert (siehe AUFTRAG_CD_SYSTEM.md in deiner Knowledge Base).
- Logo-Briefing: Werkblock mit Lichtspalt (abstrakt, kein figuratives Element).
- Leitsatz: "Nur wo Licht ist, ist auch Schatten."
- Tagline: "Die Struktur unter deinem Betrieb."
- Kern-Metapher: Myzel unter dem Wald. Verbindet alles. Naehrt alles.

### Deine Aufgabe

Erstelle ein **Seitenstruktur-Konzept** fuer die Schattenwerk Landing Page. NUR TEXT — kein Code, kein HTML, kein CSS.

Das Konzept soll enthalten:
1. **Seitenarchitektur** — Welche Sektionen in welcher Reihenfolge, mit Begruendung
2. **Hero-Konzept** — Was sieht der Besucher zuerst? Wie wird der Leitsatz inszeniert?
3. **Scroll-Dramaturgie** — Wie entfaltet sich die Geschichte von oben nach unten?
4. **Oekosystem-Darstellung** — Wie werden die 3 Cluster + Produkte gezeigt?
5. **CTA-Strategie** — Was ist die primaere Aktion? (kein Marketing-Sprech)
6. **Tonalitaet** — 3-5 Beispielsaetze fuer die Seite (direkt, bodenstaendig, kein Startup-Slang)

### Designprinzipien die gelten

- **Material vor Dekor.** Schwarzer Stein, dunkles Metall, Glas, Erde, Myzel — in dieser Hierarchie.
- **Foyer ueber dem Myzel.** Oberflaeche ruhig, Intelligenz darunter (Glasboden-Konzept).
- **Zustandslogik.** Farbe reagiert auf Zustand (nicht verbunden → rot; verbunden → weiss/Myzel).
- **Dachmarke = ruhigster Auftritt.** Substanz vor Dekoration. Kein buntes Cluster-Feuerwerk.
- **Farben:** Nur Schwarz/Weiss/Rotbruch. KEINE Cluster-Signalfarben (kein Orange, kein Teal, kein Gruen) auf der Dachmarke.
- **Typografie:** Pool A (Big Shoulders Display) fuer Wortmarke + Headlines. Pool C (Inter) fuer Body. Pool B (IBM Plex Sans) nur wenn Produkt-Referenz noetig.

### NICHT TUN

- Kein Code, kein Wireframe, keine Pixel
- Kein Silicon-Valley-Glaette, kein Startup-Frische
- Kein "Wir schuetzen Ihr Unternehmen" — Handwerker-Sprache
- Keine Avengers-Kopie — Energie uebersetzen, nicht nachbauen
- Keine Cluster-Farben auf der Dachmarke

### Fragen

Du darfst **3 Klaerungsfragen** stellen bevor du loslegst. Dann HALT und auf Antwort warten.

**HALT nach Konzept-Text. Mirko gibt Freigabe bevor Code-Phase beginnt.**

---

## Reihenfolge

1. Patches ausfuehren (Aufgabe A) — schnell, mechanisch
2. Parallel Klaerungsfragen fuer LP stellen (Aufgabe B)
3. Nach Patch-HALT: gepatchtes Logo-Briefing zeigen
4. Nach Fragen-Antwort: LP-Konzept schreiben
