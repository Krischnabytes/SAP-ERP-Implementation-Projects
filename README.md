# SAP ERP Implementierungsprojekte

> Praktische SAP ECC Erfahrung in den Modulen Materialwirtschaft, Produktionsplanung und Vertrieb

[![SAP ECC](https://img.shields.io/badge/SAP-ECC-0FAAFF?style=flat-square&logo=sap)](https://www.sap.com/)
[![Status](https://img.shields.io/badge/Status-Abgeschlossen-success?style=flat-square)]()
[![Zeitraum](https://img.shields.io/badge/Zeitraum-Jul--Sep%202025-blue?style=flat-square)]()

## 👤 Über mich

**Name:** Krishnanunne Sajeev  
**Hochschule:** Johannes Kepler Universität Linz  
**Studiengang:** Wirtschaftsinformatik  
**SAP System:** H03, Mandant 352  

## 📋 Inhaltsverzeichnis

- [Überblick](#überblick)
- [Business Szenario](#business-szenario)
- [Technische Umsetzung](#technische-umsetzung)
- [Demonstrierte Kompetenzen](#demonstrierte-kompetenzen)
- [Projektphasen](#projektphasen)
- [Erfolge](#erfolge)
- [Problemlösungsbeispiele](#problemlösungsbeispiele)
- [Dokumentation](#dokumentation)
- [Kontakt](#kontakt)

## 🎯 Überblick

Dieses Repository dokumentiert **praktische SAP ERP Implementierungserfahrung** aus drei aufeinander aufbauenden Universitätskursen. Das Projekt umfasst die Implementierung integrierter Geschäftsprozesse für den strategischen E-Bike Markteintritt der Global Bike Inc.

**Projektumfang:**
- End-to-End Geschäftsprozess-Konfiguration im produktiven SAP ECC System
- Cross-Modul Integration (MM ↔ PP ↔ SD)
- Stammdatenanlage und Organisationsstruktur-Setup
- SPRO Customizing und Prozessautomatisierung
- Praktische Problemlösung bei Lieferantenbeschränkungen und Qualitätsproblemen

**Dauer:** 3 Monate (Juli - September 2025)  
**Module:** Materialwirtschaft (MM), Produktionsplanung (PP), Vertrieb (SD), Controlling (CO)  
**Benutzeroberflächen:** SAP GUI + SAP Fiori

## 🚴 Business Szenario

**Unternehmen:** Global Bike Inc. (GBI) Österreich  
**Herausforderung:** Markteintritt im E-Bike Segment mit neuer Produktlinie  
**Komplexität:** Komplette Supply Chain Einrichtung von Beschaffung über Produktion bis Vertrieb

**Anforderungen:**
- Neues Produkt: E-Bike Super Toll 1234-21
- 5-teilige Fertigungsstruktur
- Lieferantenintegration (GigaRad-21) mit Mindestbestellmengen-Einschränkungen
- Kundenbeziehung (RadFan-21) mit Mengenrabatten
- Entwicklungs-Kostenstelle für F&E Tracking
- Produktionsstandort: Werk Wien (W000)

## 🔧 Technische Umsetzung

### Angelegte Stammdaten

| Typ | Beschreibung | ID/Material |
|-----|--------------|-------------|
| **Fertigprodukt** | E-Bike Super Toll 1234 | E-MTBA-21 |
| **Komponenten** | Rahmen, Akku, Motor, Display, Kabelbaum | 5 Materialien (MTBA2-21, Battery-21, etc.) |
| **Lieferant** | Komponentenlieferant | GigaRad-21 (48391) |
| **Kunde** | E-Bike Händler | RadFan-21 (200098) |
| **Kostenstelle** | Entwicklungsabteilung | 30-3-21 |

### Implementierte Geschäftsprozesse

#### 1️⃣ Beschaffungsprozess (MM)
```
Bedarfsanforderung (ME51N)
    ↓
Bestellung (ME21N)
    ↓
Wareneingang (MIGO)
    ↓
Rechnungsprüfung (MIRO)
```

#### 2️⃣ Vertriebsprozess (SD)
```
Kundenanfrage (VA11)
    ↓
Angebot (VA21)
    ↓
Kundenauftrag (VA01)
    ↓
Lieferung (VL01N/VL02N)
    ↓
Faktura (VF01)
```

#### 3️⃣ Produktionsplanung & Durchführung (PP)
```
Stücklistenanlage (CS01)
    ↓
Arbeitsplananlage (CA01)
    ↓
Materialbedarfsplanung (MD02/MD04)
    ↓
Fertigungsauftrag (CO01)
    ↓
Rückmeldung (CO11N)
```

### SPRO Customizing-Objekte

| Objekt | ID | Zweck |
|--------|-----|-------|
| Einkäufergruppe | G21 | Beschaffungsorganisation |
| Produktionssteuerungsprofil | G00021 | Prozessautomatisierung |
| Fertigungssteuerer | G21 | Verantwortungszuordnung |
| Verkaufsbelegtyp | ZG21 | Kundenspezifische Auftragsbearbeitung |

## 💡 Demonstrierte Kompetenzen

### SAP Fachkenntnisse

**Beherrschte Transaktionscodes (30+):**
- **MM:** MM01, MM02, ME51N, ME21N, MIGO, MIRO, XK01
- **PP:** CS01, CA01, MD02, MD04, CO01, CO02, CO11N
- **SD:** VA11, VA21, VA01, VL01N, VL02N, VF01, XD01
- **CO:** KS01, KS02

**Benutzeroberflächen:**
- SAP GUI (klassische Oberfläche)
- SAP Fiori (moderne Web-UI) - 4+ Transaktionen

**Konfiguration:**
- SPRO Customizing
- Organisationsstruktur-Setup
- Stammdaten-Sichten Konfiguration

### Business Skills

- End-to-End Prozessverständnis
- Cross-Modul Integration
- Geschäftsprozessmodellierung (BPMN)
- Strategische Analyse (Porter's Wertkette)
- Professionelle Dokumentation

## 📚 Projektphasen

### Phase 1: Einführung in ERP-Systeme
**Zeitraum:** Juli-August 2025  
**Fokus:** Grundlagen und Basis-Geschäftsprozesse  
**Status:** ✅ Abgeschlossen

**Ergebnisse:**
- Komplette Beschaffungs-Implementierung
- Vertriebsprozess-Durchführung
- 6 Materialstammsätze angelegt
- 2 Geschäftspartner konfiguriert
- Professionelle Fallstudiendokumentation

[📄 Phase 1 Dokumentation ansehen](./Phase1_Einfuehrung/)

---

### Phase 2: ERP-Systeme Anwendungen I
**Zeitraum:** September 2025  
**Fokus:** Produktionsplanung und Fiori-Kompetenz  
**Status:** ✅ Abgeschlossen

**Ergebnisse:**
- Stücklisten- und Arbeitsplananlage
- Materialbedarfsplanung und Fertigungsauftragsdurchführung
- SAP Fiori Transaktionen (4+)
- Porter's Wertketten-Analyse
- Prozessflussdiagramme (BPMN)

[📄 Phase 2 Dokumentation ansehen](./Phase2_Anwendung_I/)

---

### Phase 3: ERP-Systeme Anwendungen II
**Zeitraum:** September 2025  
**Fokus:** System Customizing und Automatisierung  
**Status:** ✅ Abgeschlossen (~85%)

**Ergebnisse:**
- 4 Customizing-Objekte angelegt
- Prozessautomatisierungs-Konfiguration
- Systemtests und Validierung
- Technische Dokumentation

[📄 Phase 3 Dokumentation ansehen](./Phase3_Anwendung_II/)

## 🏆 Erfolge

- ✅ **30+ SAP Transaktionen** erfolgreich durchgeführt
- ✅ **8 Stammdatenobjekte** angelegt (6 Materialien, 2 Geschäftspartner)
- ✅ **3 komplette Geschäftszyklen** End-to-End implementiert
- ✅ **4 Customizing-Objekte** für Prozessautomatisierung konfiguriert
- ✅ **Dual-Interface Kompetenz** - SAP GUI und Fiori
- ✅ **70+ Seiten** professionelle Dokumentation
- ✅ **Praktische Problemlösung** - Mindestbestellmengen, fehlerhafte Ware, Systemfehler

## 🔥 Problemlösungsbeispiele

### Herausforderung 1: Mindestbestellmengen-Konflikt

**Problem:** Lieferant GigaRad-21 forderte Mindestbestellmenge von 50 Stück pro Komponente, Entwicklung benötigte nur 15 für Prototyping.

**Lösung:** 
- Bestellung der Lieferanten-Mindestmenge (50 Stück)
- Verwaltung des Überbestands (35 Stück) mit Lagerplanung
- Dokumentation der geschäftlichen Auswirkungen

**Kompetenzen:** Beschaffungsverhandlung, Lagerverwaltung, Umgang mit Geschäftseinschränkungen

---

### Herausforderung 2: Umgang mit fehlerhafter Ware

**Problem:** 5 Display-Einheiten kamen mit Oberflächenfehlern an, Retouren und angepasste Rechnungsstellung erforderlich.

**Lösung:**
- MIGO Retourentransaktion mit korrekten Grundcodes durchgeführt
- Wareneingangsmenge angepasst (30 gut vs 35 erhalten)
- Rechnungsprüfung nur für akzeptierte Menge abgestimmt

**Kompetenzen:** Qualitätsmanagement, Retourenabwicklung, 3-Wege-Abstimmung (Bestellung-Wareneingang-Rechnung)

---

### Herausforderung 3: Produktionssteuerungsprofil-Konfiguration

**Problem:** Initiale Fertigungsauftragserstellung schlug fehl - Arbeitsplan nicht korrekt mit Materialstamm verknüpft.

**Lösung:**
- Alternative Materialbedarfsplanungs-Route verwendet (MD02 → CO41)
- Planaufträge erstellt, dann in Fertigungsaufträge konvertiert
- Fertigungssteuerer G21 explizit bei Konvertierung angegeben

**Kompetenzen:** System-Troubleshooting, PP-Modul Abhängigkeiten, alternative Lösungswege

## 📖 Dokumentation

### Repository Struktur

```
SAP-ERP-Projekte/
│
├── README.md                          # Diese Datei
├── Portfolio_Übersicht.pdf            # Zusammenfassung
│
├── Phase1_Einfuehrung/
│   ├── Fallstudie.pdf                # Komplette Dokumentation
│   ├── Screenshots/                  # Wichtige Transaktionen
│   └── Transaktions_Zusammenfassung.md
│
├── Phase2_Anwendung_I/
│   ├── Fallstudie.pdf                # Erweiterte Prozesse
│   ├── Porter_Wertkette.pdf          # Strategische Analyse
│   ├── Prozessfluss_Diagramm.pdf     # BPMN Diagramme
│   └── Screenshots/                  # Fiori & Produktionsplanung
│
├── Phase3_Anwendung_II/
│   ├── Customizing_Dokumentation.pdf # SPRO Konfigurationen
│   ├── Test_Ergebnisse.pdf           # Validierungsergebnisse
│   └── Screenshots/                  # Konfigurationsbildschirme
│
└── Ressourcen/
    ├── Transaktionscode_Referenz.md  # Alle verwendeten T-Codes
    ├── Stammdaten_Übersicht.md       # Angelegte Objekte
    └── System_Architektur.md         # Technisches Setup
```

### Verfügbare Dokumente

- 📄 **Portfolio Übersicht** - Zusammenfassung für Recruiter
- 📄 **Fallstudien (3)** - Detaillierte Implementierungsdokumentation
- 📄 **Prozessdiagramme** - BPMN Flussdiagramme
- 📄 **Strategische Analyse** - Porter's Wertkette
- 📄 **Screenshots** - Wichtige Transaktionen und Konfigurationen
- 📄 **Transaktionsreferenz** - Komplette T-Code Liste

## 🎓 Absolvierte Kurse

1. **256.904 Einführung in ERP-Systeme**  
   Einführung in ERP-Systeme

2. **256.905 ERP-Systeme Anwendungen I**  
   ERP-Systeme Anwendungen I

3. **256.907 ERP-Systeme Anwendungen II**  
   ERP-Systeme Anwendungen II

**Institution:** Johannes Kepler Universität Linz  
**Dozentin:** Barbara Krumay et al.  
**Zeitraum:** Sommersemester 2025

## 🌟 Warum das wichtig ist

Dieses Projekt demonstriert:

1. **Echte Systemerfahrung** - Keine Simulationen, tatsächliche SAP ECC Arbeit
2. **Problemlösungsfähigkeit** - Umgang mit realen Komplikationen
3. **Cross-Modul Verständnis** - Wie MM, PP, SD zusammenarbeiten
4. **Moderne Kenntnisse** - Sowohl traditionelles GUI als auch modernes Fiori
5. **Business-Verständnis** - Strategische Analyse und Prozessdenken
6. **Professionelle Dokumentation** - Komplettes technisches Schreiben

## 📬 Kontakt

**Krishnanunne Sajeev**  
Wirtschaftsinformatik Student  
Johannes Kepler Universität Linz

📧 E-Mail: [Ihre E-Mail]  
💼 LinkedIn: [Ihr LinkedIn]  
🌐 Portfolio: [Dieses Repository]

---

## 📝 Lizenz

Dieses Repository enthält akademische Projektarbeit, die im Rahmen von Universitätskursen erstellt wurde. Dokumentation und Screenshots dienen Portfoliopräsentationszwecken.

---

## 🙏 Danksagungen

- Johannes Kepler Universität ERP-Systemkurse
- Dozentin: Barbara Krumay
- SAP University Alliance Programm

---

<div align="center">

**⭐ Für Recruiter:** Dieses Repository zeigt praktische SAP-Implementierungskenntnisse, die für Praktikumsbewerbungen bereit sind.

**📧 Interesse an SAP-Möglichkeiten?** Bitte kontaktieren Sie mich!

</div>
