# Phase 3: ERP-Systeme Anwendungen II

**Zeitraum:** September 2025  
**Status:** ✅ Abgeschlossen (~85%)  
**Fokus:** System Customizing, SPRO-Konfiguration und Prozessautomatisierung

## 🎯 Kursziele

Diese Phase konzentrierte sich auf erweiterte Systemkonfiguration:
- SPRO Customizing-Implementierung
- Organisationsstruktur-Anlage
- Prozessautomatisierungs-Einstellungen
- Systemtests und Validierung

## 📋 Meine Erfolge

### Angelegte SPRO Customizing-Objekte

#### 1. Einkäufergruppe G21 ✅
**Zweck:** Getrennte Auswertung und Organisationsstruktur für Beschaffung

**Konfiguration:**
- Angelegt über OMSK-Transaktion
- Mit Einkaufsorganisation EK00 verknüpft
- Spezifischen Materialien zugeordnet
- Getestet über ME2M (erfolgreiche Zuordnung bestätigt)

**Status:** Voll funktionsfähig und validiert

---

#### 2. Produktionssteuerungsprofil G00021 ✅
**Zweck:** Prozessautomatisierung für Fertigungsaufträge

**Konfiguration:**
- Angelegt über OPPR-Transaktion
- Automatische Terminierung aktiviert
- Komponentenverfügbarkeitsprüfungs-Einstellungen
- Freigabestrategie-Konfiguration

**Status:** Erfolgreich mit Automatisierungsfunktionen angelegt

---

#### 3. Fertigungssteuerer G21 ✅
**Zweck:** Verantwortungszuordnung für Produktionsplanung

**Konfiguration:**
- Angelegt über OPJL-Transaktion
- Mit Produktionssteuerungsprofil G00021 verknüpft
- Werk W000 zugeordnet

**Status:** Angelegt und mit Profil verknüpft

**Aufgetretene Herausforderung:**
- Fertigungssteuerer-Feld nicht in MM02 sichtbar
- Gelöst über MRP-Planungsroute (MD02 → CO41)
- Fertigungsaufträge erfolgreich mit G21-Zuordnung angelegt

---

#### 4. Verkaufsbelegtyp ZG21 ✅
**Zweck:** Kundenspezifische Auftragsbearbeitung mit automatischer Lieferanlage

**Konfiguration:**
- Angelegt über VOV8-Transaktion
- Basierend auf Standard-Auftragstyp OR
- Automatische Lieferanlage aktiviert
- Positionstypen-Konfiguration abgeschlossen

**Status:** Angelegt, aber Testen blockiert

**Aufgetretene Herausforderung:**
- Verkaufsbereich VK00/01/01 nicht im System konfiguriert
- Erfordert OVXR-Berechtigung (im Studentenkonto eingeschränkt)
- Konfiguration als korrekt bestätigt, System-Zugang ausstehend

## 🔧 Verwendete Transaktionscodes

### Customizing (SPRO)
- **SPRO** - SAP-Implementierungsleitfaden
- **OMSK** - Einkäufergruppen pflegen
- **OPPR** - Produktionssteuerungsprofile pflegen
- **OPJL** - Fertigungssteuerer pflegen
- **VOV8** - Verkaufsbelegtypen definieren
- **OVXR** - Verkaufsbereiche pflegen (versucht - Berechtigungsproblem)

### Test & Validierung
- **ME2M** - Bestellungen nach Material (Einkäufergruppe verifiziert)
- **MD02** - MRP-Lauf (Produktionsplanung getestet)
- **CO41** - Planauftrag umsetzen (Fertigungssteuerer verifiziert)
- **MM02** - Materialstamm (Fertigungssteuerer-Zuordnung versucht)

## 💡 Wichtige Lernerfolge

### Systemkonfigurations-Komplexität
- Selbst einfache Geschäftsanforderungen benötigen mehrstufige Konfiguration
- Abhängigkeiten zwischen Customizing-Objekten
- Systemberechtigung beeinflusst, was konfiguriert werden kann
- Alternative Lösungswege, wenn direkter Ansatz blockiert

### Problemlösungsansatz
1. **Fertigungsauftrags-Problem:**
   - Fehler: "Arbeitsvorbereitungsdaten von Material E-GEBIKE-G21 sind nicht gepflegt"
   - Ursache: Fertigungssteuerer nicht mit Material verknüpft
   - Lösung: MRP-Route (MD02 → CO41) mit expliziter G21-Spezifikation

2. **Verkaufsbereichs-Problem:**
   - Fehler: Benötigter Verkaufsbereich existiert nicht
   - Ursache: Studentenkonto fehlt OVXR-Berechtigung
   - Status: Konfiguration komplett, Dozenten-Unterstützung ausstehend

### Test-Methodik
- Test 1 (Beschaffung): ✅ Komplett - Über ME2M verifiziert
- Test 2 (Produktion): ⚠️ Teilweise - Alternative Lösung erfolgreich
- Test 3 (Vertrieb): ❌ Blockiert - Systemkonfigurations-Einschränkung

## 📄 Dokumentation

Dateien in diesem Ordner:
- **Customizing_Dokumentation.pdf** - Komplette SPRO-Konfigurationsdetails
- **Test_Ergebnisse.pdf** - Validierungsergebnisse für alle Tests
- **Screenshots/** - Konfigurationsbildschirme und Fehlermeldungen

## 🎓 Demonstrierte Kompetenzen

- SPRO-Navigation und Customizing
- Organisationsstruktur-Konfiguration
- Prozessautomatisierungs-Setup
- System-Troubleshooting und alternative Lösungen
- Professionelle Problem-Dokumentation
- Verständnis von Berechtigungskonzepten
- Fähigkeit, innerhalb von System-Einschränkungen zu arbeiten

## 🔍 Technische Einblicke

### Was ich über SAP Customizing gelernt habe:

**Organisationsstrukturen:**
- Einkäufergruppen ermöglichen getrennte Beschaffungsauswertung
- Produktionssteuerungsprofile automatisieren Auftragsbearbeitung
- Verkaufsbelegtypen definieren Auftragsverhalten

**Systemabhängigkeiten:**
- Materialstamm → Produktionsplanung → Vertrieb
- Berechtigungsstufen beschränken Konfigurations-Zugang
- Mehrere Lösungswege existieren für die meisten Aufgaben

**Praxisnahe Implementierung:**
- Nicht alle Konfigurationen gelingen beim ersten Versuch
- System-Einschränkungen erfordern kreative Umgehungslösungen
- Dokumentation von Blockern ist genauso wertvoll wie Erfolgsgeschichten

## 📈 Fertigstellungsstatus

| Komponente | Status | Anmerkungen |
|-----------|--------|-------------|
| Einkäufergruppe G21 | ✅ 100% | Voll funktionsfähig, über ME2M getestet |
| Produktionssteuerungsprofil | ✅ 100% | Mit Automatisierungseinstellungen angelegt |
| Fertigungssteuerer G21 | ✅ 85% | Funktionsfähig über MRP-Route |
| Verkaufsbelegtyp ZG21 | ✅ 90% | Angelegt, Testen durch System-Zugang blockiert |

**Gesamt-Phasenfertigstellung: ~85%**

Unvollständige Arbeit ist klar dokumentiert mit:
- Spezifischen Fehlermeldungen
- Ursachenanalyse
- Versuchten Lösungen
- Empfohlenen nächsten Schritten

---

[← Vorherige Phase: Anwendung I](../Phase2_Anwendung_I/README.md) | [Zurück zum Hauptportfolio](../README.md)
