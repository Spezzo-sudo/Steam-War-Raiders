# Äther-Imperium: Chroniken des Dampfs

Ein Vite + React Prototyp für die Steampunk-Raiders Verwaltungssimulation.

## Voraussetzungen

- Node.js 18+
- npm 9+

## Lokale Entwicklung

1. Abhängigkeiten installieren:
   ```bash
   npm install
   ```
2. Entwicklungsserver starten:
   ```bash
   npm run dev
   ```
3. Production-Build prüfen:
   ```bash
   npm run build
   ```
4. Typprüfung ausführen:
   ```bash
   npm run typecheck
   ```
5. Linting anstoßen:
   ```bash
   npm run lint
   ```
6. Testsuite starten:
   ```bash
   npm run test
   ```

## Projektstruktur

```
.
├── index.html
├── package.json
├── tsconfig.json
├── vite.config.ts
└── src/
    ├── App.tsx
    ├── components/
    ├── constants.ts
    ├── hooks/
    ├── lib/
    ├── main.tsx
    ├── store/
    └── types.ts
```

- `src/` enthält den kompletten Anwendungscode.
- Der `@`-Alias verweist auf `src/` und verhindert tiefe Relative-Imports.
- Jede exportierte Funktion besitzt eine kurze JSDoc-Beschreibung.

## Umgebungsvariablen

Die API-Schlüssel werden über `GEMINI_API_KEY` aus einer `.env` Datei geladen. Lokale Builds funktionieren auch ohne Schlüssel,
solange keine API-Aufrufe ausgelöst werden.

## Projektstatus

### Erledigt
- Archiv `Dampfnudel-Raiders-main (1).zip` entpackt und Projektdateien in das Repository übernommen.
- Temporäre Archive entfernt und Arbeitsverzeichnis bereinigt.
- Gameplay-Logik für Baukosten und Warteschlangen modularisiert, inklusive neuer Hilfsfunktionen.
- Testsuite (Vitest) sowie ESLint-Konfiguration ergänzt und in die Projekt-Workflows integriert.
- API-Client-Hilfsmodul mit konfigurierbarer Basis-URL und Timeout vorbereitet.

### Offen
- Gameplay-Effekte der Forschung (z. B. Einfluss auf Produktion und Lagerkapazität) implementieren.
- UI-Feedback für Ressourcenüberlauf und Warteschlangendetails erweitern.
- Reale Backend-Endpunkte anbinden und Authentifizierungskonzept definieren.
