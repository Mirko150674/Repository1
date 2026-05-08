# Repository1 — Agent-Kommunikationskanal

> **Zweck:** Asynchroner Austausch zwischen Claude Code (CT01) und Manus
> **Owner:** Mirko Kauert (WSM GmbH)

---

## Naming-Konvention

| Praefix | Richtung | Bedeutung |
|---|---|---|
| `AUFTRAG_*.md` | Claude → Manus | Neuer Job mit Briefing |
| `ERGEBNIS_*.md` | Manus → Claude | Fertige Lieferung |
| `REVIEW_*.md` | Claude → Manus | Feedback / Patch-Auftraege |
| `FINAL_*.md` | Manus → Claude | Gepatchte Endfassung |

## Ordnerstruktur

```
/
├── README.md                  # Diese Datei
├── .github/workflows/         # Automatisierung
│   └── agent-notify.yml       # Issue-Erstellung + Notification
├── schattenwerk/              # CD-System, Logo, LP
│   ├── AUFTRAG_*.md
│   ├── ERGEBNIS_*.md
│   └── ...
└── wsm-app/                   # WSM Betrieb + App (spaeter)
    └── ...
```

## Workflow

### Stufe 1 (aktiv)
1. Claude pusht `AUFTRAG_xxx.md` ins Repo
2. GitHub Action erstellt automatisch ein Issue (Label: `manus-job`)
3. Mirko startet Manus-Session, verweist auf die Datei
4. Manus arbeitet, pusht `ERGEBNIS_xxx.md` zurueck
5. GitHub Action schliesst das Issue (Label: `manus-done`) + Notification
6. Claude/Mirko reviewt, bei Bedarf `REVIEW_xxx.md` pushen

### Stufe 2 (geplant)
- Manus-API-Trigger statt manuellem Start
- Automatischer Review-Cycle

## Regeln

- **D:\ bleibt Master.** GitHub ist Kommunikationskanal, nicht Primaerspeicher.
- **Keine sensiblen Daten.** Repo ist public. Keine Kundennamen, Credentials, Finanzdaten.
- **Ein Auftrag = eine Datei.** Kein Auftrag ueber mehrere Files verteilt.
- **Manus-Input muss perfekt sein.** Lieber 1h laenger briefen als Mittelmass korrigieren.
