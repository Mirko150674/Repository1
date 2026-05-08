# Setup-Anleitung

Die Datei `agent-notify.yml` in diesem Ordner muss manuell nach `.github/workflows/agent-notify.yml` verschoben werden.

**Warum manuell?** GitHub verlangt den `workflow`-Scope fuer API-Zugriff auf `.github/workflows/`. Die CLI-Authentifizierung hat diesen Scope nicht.

**Wie (30 Sekunden):**
1. Oeffne `agent-notify.yml` in diesem Ordner auf GitHub
2. Klicke den Stift (Edit)
3. Aendere den Pfad oben von `_setup/agent-notify.yml` zu `.github/workflows/agent-notify.yml`
4. Commit

Danach kann `_setup/` geloescht werden.
