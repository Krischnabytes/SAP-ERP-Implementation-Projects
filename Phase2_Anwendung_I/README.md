# Phase 2: ERP-Systeme Anwendungen I

**Zeitraum:** September 2025  
**Status:** ✅ Abgeschlossen  
**Fokus:** Erweiterte Prozesse, Produktionsplanung und SAP Fiori-Kompetenz

## 🎯 Kursziele

Diese Phase baute auf Grundkenntnissen auf und umfasste:
- Produktionsplanung und -durchführung
- Stücklisten- (BOM) und Arbeitsplananlage
- Materialbedarfsplanung (MRP)
- SAP Fiori Benutzeroberflächen-Kompetenz
- Strategische Business-Analyse

## 📋 Meine Erfolge

### Produktionsplanungs-Implementierung

#### 1. Stücklistenanlage (CS01)
Stückliste für E-MTBA-21 angelegt:
- 1x Mountainbike-Rahmen (MTBA2-21)
- 1x Akku (Battery-21)
- 1x Motor (Motor-21)
- 1x Display (Display-21)
- 1x Kabelbaum (Wiring harness-21)

#### 2. Arbeitsplan (CA01)
Arbeitsschritte für E-Bike-Montage definiert:
- Komponentenvorbereitung
- Rahmenmontage
- Elektroinstallation
- Qualitätskontrolle
- Endverpackung

#### 3. Materialbedarfsplanung (MD02/MD04)
- MRP für 10 fertige E-Bikes durchgeführt
- Komponentenbedarf analysiert
- Planaufträge generiert

#### 4. Fertigungsauftragsdurchführung (CO01/CO02/CO11N)
- Fertigungsaufträge angelegt
- Zur Durchführung freigegeben
- Komponentenverbrauch rückgemeldet
- Warenzugang Fertigprodukte gebucht

### SAP Fiori Kompetenz

**4+ Transaktionen** über SAP Fiori-Oberfläche durchgeführt:
- ✅ Kundenanfrage (VA11)
- ✅ Angebot (VA21)
- ✅ Kundenauftrag (VA01)
- ✅ Lieferungsabwicklung (VL01N)
- ✅ Fakturierung (VF01)

### Strategische Business-Analyse

**Porter's Wertketten-Analyse:**
- E-Bike-Einführung über alle Wertkettenaktivitäten abgebildet
- Primäraktivitäten identifiziert (Eingangslogistik, Operationen, Ausgangslogistik, Marketing & Vertrieb, Service)
- Unterstützungsaktivitäten hervorgehoben (Unternehmensinfrastruktur, Personal, Technologieentwicklung, Beschaffung)
- Gezeigt, wie ERP Geschäftsprozesse integriert

**Prozessflussdiagramme:**
- BPMN-Flussdiagramme mit Camunda Modeler erstellt
- Abhängigkeiten zwischen Beschaffung, Entwicklung, Produktion und Vertrieb dargestellt
- Entscheidungspunkte und Ausnahmebehandlung dokumentiert

## 🔧 Verwendete Transaktionscodes

### Produktionsplanung (PP)
- **CS01** - Stückliste anlegen
- **CS02** - Stückliste ändern
- **CS03** - Stückliste anzeigen
- **CA01** - Arbeitsplan anlegen
- **CA02** - Arbeitsplan ändern
- **CA03** - Arbeitsplan anzeigen
- **MD02** - MRP-Lauf - Einzelposition
- **MD04** - Bestand/Bedarf anzeigen
- **CO41** - Planauftrag umsetzen

### Fertigungssteuerung
- **CO01** - Fertigungsauftrag anlegen
- **CO02** - Fertigungsauftrag ändern
- **CO03** - Fertigungsauftrag anzeigen
- **CO11N** - Rückmeldung

### Vertrieb (Fiori)
- **VA11** - Anfrage anlegen (Fiori)
- **VA21** - Angebot anlegen (Fiori)
- **VA01** - Kundenauftrag anlegen (Fiori)
- **VL01N** - Lieferung anlegen (Fiori)
- **VF01** - Faktura anlegen (Fiori)

## 💡 Wichtige Lernerfolge

### Integrationsverständnis
- Wie Stückliste die MRP-Planung steuert
- Automatische Komponentenreservierung in Fertigungsaufträgen
- Cross-Modul Datenfluss (MM → PP → SD)
- Bestandsauswirkungen der Fertigungsdurchführung

### Moderne UI-Vorteile
- Fioris rollenbasierte, vereinfachte Oberfläche
- Bessere Benutzererfahrung vs. traditionelles GUI
- Mobile-freundliches Design
- Aufgabenorientierte Workflows

## 📄 Dokumentation

Dateien in diesem Ordner:
- **Fallstudie.pdf** - Komplette Dokumentation erweiterter Prozesse
- **Porter_Wertkette_Analyse.pdf** - Strategisches Business-Framework
- **Prozessfluss_Diagramm.pdf** - BPMN Flussdiagramme
- **Screenshots/** - Fiori-Oberfläche und Produktionsplanungsbildschirme

## 🎓 Demonstrierte Kompetenzen

- Produktionsplanung und Stücklistenverwaltung
- Arbeitsplananlage
- MRP-Durchführung und -Analyse
- Moderne SAP Fiori-Oberflächenkompetenz
- Strategische Business-Analyse-Frameworks
- Prozessmodellierung (BPMN)
- Cross-Modul Integrationsverständnis

---

[← Vorherige Phase: Einführung](../Phase1_Einfuehrung/README.md) | [Nächste Phase: Anwendung II →](../Phase3_Anwendung_II/README.md) | [Zurück zum Hauptportfolio](../README.md)
