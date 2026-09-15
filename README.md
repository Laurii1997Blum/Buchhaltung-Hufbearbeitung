# Hufbuch — als eigene App über GitHub Pages

Dieses Paket macht aus der Buchhaltungs-App eine installierbare PWA
(App-Icon, Vollbild ohne Browserleiste, Offline-Nutzung).

## Wichtig zur Privatsphäre

Eine GitHub-Pages-Seite ist über ihre URL für jeden erreichbar, der den Link
kennt — auch bei einem privaten Repository, sofern du keinen bezahlten
GitHub-Plan hast. Die Seite wird aber nicht in Suchmaschinen gelistet und ist
für Fremde praktisch nicht auffindbar. Alle deine Buchhaltungsdaten selbst
liegen sowieso **nur lokal in deinem eigenen Browser** (localStorage) — nicht
auf GitHub. Wer den Link kennt, sieht also die leere App, nicht deine Daten.

## Einrichtung (einmalig, ca. 5 Minuten)

1. Auf [github.com](https://github.com) ein kostenloses Konto erstellen (falls
   noch nicht vorhanden).
2. Neues Repository anlegen, z. B. Name `hufbuch`. Sichtbarkeit "Private" oder
   "Public" — beides funktioniert für Pages, siehe Hinweis oben.
3. Alle Dateien aus diesem Ordner (`index.html`, `manifest.json`,
   `service-worker.js`, `icons/`) per Drag & Drop auf der GitHub-Weboberfläche
   hochladen ("Add file" → "Upload files") und committen.
4. Im Repository zu **Settings → Pages** gehen. Unter "Build and deployment"
   → Source: "Deploy from a branch" → Branch: `main`, Ordner: `/ (root)` →
   Speichern.
5. Nach ein bis zwei Minuten ist die App erreichbar unter:
   `https://DEIN-BENUTZERNAME.github.io/hufbuch/`

## Auf dem Handy installieren

- **iPhone (Safari):** Seite öffnen → Teilen-Symbol → "Zum Home-Bildschirm"
- **Android (Chrome):** Seite öffnen → Menü (⋮) → "App installieren" bzw.
  "Zum Startbildschirm hinzufügen"

Danach erscheint ein eigenes App-Icon, die App startet im Vollbild und
funktioniert auch ohne Internetverbindung.

## Updates

Wenn ich dir später eine neue Version der App schicke: einfach die
`index.html` (und ggf. die anderen Dateien) im GitHub-Repository ersetzen —
die installierte App aktualisiert sich beim nächsten Öffnen mit
Internetverbindung automatisch im Hintergrund.

## Backup nicht vergessen

Die Daten liegen nur in diesem einen Browser auf diesem einen Gerät. Nutze
regelmäßig den Button "Backup herunterladen" in den Einstellungen der App.
