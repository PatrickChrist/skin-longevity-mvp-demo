# Skin Longevity Lab – MVP

Klickbares Frontend-MVP für eine Skin-Longevity-Web-App.

## Enthalten

- Foto-Upload mit Vorschau
- kurzer Intake-Fragebogen
- automatische Score-Berechnung für:
  - Skin Longevity
  - Photoaging Risk
  - Barrier Resilience
  - Inflammation Load
  - Protocol Fit
- lokaler Bildsignal-Extractor via Canvas
- optionaler Cloud-/LLM-Hook
  - OpenAI-kompatibel
  - Anthropic / Claude
- generiertes Starter-Protokoll
- JSON-Debug-Ausgabe für schnelle Iteration

## Dateien

- `index.html` – komplette klickbare App ohne Build-Step

## Lokal starten

### Variante 1
Datei direkt im Browser öffnen.

### Variante 2
```bash
cd /Users/patrickchrist/.openclaw/workspace/skin-longevity-mvp
python3 -m http.server 8137
```
Dann öffnen:

`http://127.0.0.1:8137`

## Wichtiger Hinweis

Dieses MVP ist **nicht medizinisch** und **nicht diagnostisch**.
Die Scores sind bewusst als Produkt-/UX-Prototyp gebaut:

- Intake + Verhalten
- einfache Bildheuristiken
- optional ergänzende LLM-Bildanalyse

Für echte Produktion solltest du:

1. API-Keys nie im Browser halten
2. den Cloud-Call über ein Backend routen
3. Score-Logik versionieren
4. Claims juristisch sauber prüfen
5. Re-Scan-Flow, Nutzerkonto und Verlauf ergänzen

## Nächste sinnvolle Schritte

1. Branding / Sprache schärfen
2. Score-Gewichtung verfeinern
3. Produktdatenbank + kuratierte Product Picks ergänzen
4. Backend-Proxy für Claude/OpenAI bauen
5. Monatsverlauf / Compare-View einbauen
