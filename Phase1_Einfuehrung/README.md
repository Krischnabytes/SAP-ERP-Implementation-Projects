# Phase 1: Einführung in ERP-Systeme

**Zeitraum:** Juli-August 2025  
**Status:** ✅ Abgeschlossen  
**Fokus:** Grundlagen und Basis-Geschäftsprozesse

## 🎯 Kursziele

Diese Phase legte die Grundlage für die SAP ERP Implementierung mit Fokus auf:
- Beherrschung fundamentaler SAP Transaktionen
- Implementierung des kompletten Beschaffungsprozesses
- Durchführung des Vertriebsprozesses
- Anlage und Pflege von Stammdaten

## 📋 Meine Erfolge

### Angelegte Stammdaten
- ✅ 6 Materialstammsätze (E-MTBA-21 + 5 Komponenten)
- ✅ 1 Lieferant (GigaRad-21, Nummer: 48391)
- ✅ 1 Kunde (RadFan-21, Nummer: 200098)
- ✅ 1 Kostenstelle (Entwicklung: 30-3-21)

### Implementierte Geschäftszyklen

#### 1. Beschaffungsprozess (MM)
```
Bedarfsanforderung (ME51N)
    ↓
Bestellung (ME21N) - 50 Stück beim Lieferanten GigaRad-21
    ↓
Wareneingang (MIGO) - Teillieferung + fehlerhafte Retouren
    ↓
Rechnungsprüfung (MIRO) - 3-Wege-Abstimmung
```

**Wichtige Belegnummern:**
- Bedarfsanforderung: 10000178
- Bestellung: 4500000165
- Wareneingang: 5000000177

#### 2. Vertriebsprozess (SD)
```
Kundenanfrage (VA11)
    ↓
Angebot (VA21) - 8 E-Bikes à €2.750
    ↓
Kundenauftrag (VA01) - 10 E-Bikes mit 8% Rabatt
    ↓
Lieferung (VL01N/VL02N)
    ↓
Faktura (VF01)
```

**Wichtige Belegnummern:**
- Anfrage: 10000044
- Angebot: 20000113
- Kundenauftrag: 150
- Lieferungen: 80000108, 80000133

## 💡 Wichtige Lernerfolge

### Gelöste praktische Herausforderungen

**Herausforderung 1: Mindestbestellmengen-Konflikt**
- Lieferant forderte 50 Stück, Entwicklung benötigte nur 15
- Lösung: 50 Stück bestellt, Überbestand verwaltet

**Herausforderung 2: Umgang mit fehlerhafter Ware**
- 5 Displays kamen mit Mängeln an
- Lösung: Korrekte MIGO Retourenabwicklung mit Grundcodes

**Herausforderung 3: Rabatt-Konditionsmanagement**
- Benötigter 8% Rabatt (nicht Standard-RA01)
- Lösung: Korrekten Konditionstyp für Vertriebsszenario identifiziert

## 🔧 Verwendete Transaktionscodes

### Materialwirtschaft
- **MM01** - Materialstamm anlegen
- **ME51N** - Bedarfsanforderung anlegen
- **ME21N** - Bestellung anlegen
- **MIGO** - Wareneingang/Retouren
- **MIRO** - Rechnungsprüfung
- **XK01** - Lieferant anlegen

### Vertrieb
- **VA11** - Anfrage anlegen
- **VA21** - Angebot anlegen
- **VA01** - Kundenauftrag anlegen
- **VL01N** - Lieferung anlegen
- **VL02N** - Lieferung ändern
- **VF01** - Faktura anlegen
- **XD01** - Kunde anlegen

### Controlling
- **KS01** - Kostenstelle anlegen

## 📄 Dokumentation

In diesem Ordner finden Sie:
- **Fallstudie.pdf** - Komplette Implementierungsdokumentation
- **Screenshots/** - Visuelle Nachweise aller wichtigen Transaktionen

## 🎓 Demonstrierte Kompetenzen

- SAP GUI Navigation und Transaktionsdurchführung
- Stammdatenanlage mit korrekten Organisationszuordnungen
- End-to-End Geschäftsprozessverständnis
- Problemlösung mit realen Einschränkungen
- Professionelle deutsche Business-Dokumentation

---

[← Zurück zum Hauptportfolio](../README.md) | [Nächste Phase: Anwendung I →](../Phase2_Anwendung_I/README.md)
