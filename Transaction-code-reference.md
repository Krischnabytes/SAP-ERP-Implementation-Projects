# SAP Transaktionscode-Referenz

Vollständige Liste der Transaktionscodes, die in allen drei Projektphasen verwendet wurden.

## Materialwirtschaft (MM)

### Stammdaten
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **MM01** | Materialstamm anlegen | 6 Materialien angelegt (E-MTBA-21 + 5 Komponenten) |
| **MM02** | Materialstamm ändern | Materialdaten bei Bedarf aktualisiert |
| **MM03** | Materialstamm anzeigen | Materialkonfigurationen überprüft |
| **XK01** | Lieferant anlegen | Lieferant GigaRad-21 (48391) angelegt |
| **XK02** | Lieferant ändern | Lieferantenstammdaten aktualisiert |

### Beschaffung
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **ME51N** | Bedarfsanforderung anlegen | BANF 10000178 für 15 Komponenten angelegt |
| **ME52N** | Bedarfsanforderung ändern | BANF-Details geändert |
| **ME53N** | Bedarfsanforderung anzeigen | BANF-Status überprüft |
| **ME21N** | Bestellung anlegen | Bestellung 4500000165 für 50 Komponenten angelegt |
| **ME22N** | Bestellung ändern | Bestellung bei Bedarf aktualisiert |
| **ME23N** | Bestellung anzeigen | Bestelldetails überprüft |
| **ME2M** | Bestellungen nach Material | Einkäufergruppen-Zuordnung verifiziert |

### Bestandsführung
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **MIGO** | Wareneingang/-ausgang | Wareneingang 5000000177 + fehlerhafte Retouren |
| **MB03** | Materialbelegauskunft | Warenbewegungen überprüft |
| **MMBE** | Bestandsübersicht | Bestandsmengen geprüft |

### Rechnungsprüfung
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **MIRO** | Rechnung erfassen | Lieferantenrechnungen mit 3-Wege-Abstimmung gebucht |
| **MIR4** | Rechnungsbeleg anzeigen | Rechnungsbuchungen überprüft |

---

## Produktionsplanung (PP)

### Stammdaten
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **CS01** | Stückliste anlegen | Stückliste für E-MTBA-21 angelegt (5 Komponenten) |
| **CS02** | Stückliste ändern | Stücklistenstruktur aktualisiert |
| **CS03** | Stückliste anzeigen | Stücklistenkonfiguration überprüft |
| **CA01** | Arbeitsplan anlegen | Arbeitsplan für E-Bike-Montage angelegt |
| **CA02** | Arbeitsplan ändern | Arbeitsplanschritte geändert |
| **CA03** | Arbeitsplan anzeigen | Arbeitsplandetails überprüft |

### Produktionsplanung
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **MD02** | MRP-Lauf - Einzelposition | Materialbedarfsplanung durchgeführt |
| **MD04** | Bestand/Bedarf anzeigen | Planungsergebnisse analysiert |
| **CO41** | Planauftrag umsetzen | Planaufträge in Fertigungsaufträge umgesetzt |

### Fertigungssteuerung
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **CO01** | Fertigungsauftrag anlegen | Fertigungsaufträge für 10 E-Bikes angelegt |
| **CO02** | Fertigungsauftrag ändern | Fertigungsaufträge freigegeben und verwaltet |
| **CO03** | Fertigungsauftrag anzeigen | Auftragsstatus überprüft |
| **CO11N** | Rückmeldung | Komponentenverbrauch und Fertigprodukte rückgemeldet |

---

## Vertrieb (SD)

### Stammdaten
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **XD01** | Kunde anlegen | Kunde RadFan-21 (200098) angelegt |
| **XD02** | Kunde ändern | Kundenstammdaten aktualisiert |
| **XD03** | Kunde anzeigen | Kundenkonfiguration überprüft |

### Vertriebsabwicklung (SAP GUI)
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **VA11** | Anfrage anlegen | Kundenanfrage 10000044 angelegt |
| **VA12** | Anfrage ändern | Anfragedetails geändert |
| **VA13** | Anfrage anzeigen | Anfragestatus überprüft |
| **VA21** | Angebot anlegen | Angebot 20000113 für 8 E-Bikes à €2.750 angelegt |
| **VA22** | Angebot ändern | Angebot bei Bedarf aktualisiert |
| **VA23** | Angebot anzeigen | Angebotsdetails überprüft |
| **VA01** | Kundenauftrag anlegen | Auftrag 150 für 10 E-Bikes mit 8% Rabatt angelegt |
| **VA02** | Kundenauftrag ändern | Kundenauftrag geändert |
| **VA03** | Kundenauftrag anzeigen | Auftragsstatus überprüft |

### Vertriebsabwicklung (SAP Fiori)
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **VA11 (Fiori)** | Anfrage anlegen | Über Fiori-Oberfläche durchgeführt |
| **VA21 (Fiori)** | Angebot anlegen | Fiori-basierte Angebotsanlage |
| **VA01 (Fiori)** | Kundenauftrag anlegen | Fiori-basierte Auftragsbearbeitung |
| **VL01N (Fiori)** | Lieferung anlegen | Fiori-Lieferungsanlage |
| **VF01 (Fiori)** | Faktura anlegen | Fiori-Fakturierung |

### Lieferung & Fakturierung
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **VL01N** | Lieferung anlegen | Lieferungen 80000108, 80000133 angelegt |
| **VL02N** | Lieferung ändern | Warenausgang gebucht |
| **VL03N** | Lieferung anzeigen | Lieferbelege überprüft |
| **VF01** | Faktura anlegen | Kundenrechnungen erstellt |
| **VF02** | Faktura ändern | Rechnungen bei Bedarf geändert |
| **VF03** | Faktura anzeigen | Rechnungsstatus überprüft |

---

## Controlling (CO)

### Kostenstellenrechnung
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **KS01** | Kostenstelle anlegen | Kostenstelle 30-3-21 für Entwicklung angelegt |
| **KS02** | Kostenstelle ändern | Kostenstellendetails aktualisiert |
| **KS03** | Kostenstelle anzeigen | Kostenstellenkonfiguration überprüft |

---

## Customizing (SPRO)

### Konfigurations-Transaktionen
| Transaktion | Beschreibung | Verwendung im Projekt |
|-------------|--------------|----------------------|
| **SPRO** | Customizing - Einführungsleitfaden | Alle Customizing-Menüs aufgerufen |
| **OMSK** | Einkäufergruppen pflegen | Einkäufergruppe G21 angelegt |
| **OPPR** | Produktionssteuerungsprofile pflegen | Profil G00021 angelegt |
| **OPJL** | Fertigungssteuerer pflegen | Steuerer G21 angelegt |
| **VOV8** | Verkaufsbelegtypen definieren | Verkaufsbelegtyp ZG21 angelegt |

---

## Zusammenfassende Statistik

### Insgesamt verwendete Transaktionen: 50+

**Nach Modul:**
- Materialwirtschaft (MM): 15+ Transaktionen
- Produktionsplanung (PP): 14+ Transaktionen
- Vertrieb (SD): 18+ Transaktionen
- Controlling (CO): 3+ Transaktionen
- Customizing (SPRO): 5+ Transaktionen

**Oberflächen-Aufteilung:**
- SAP GUI: 45+ Transaktionen
- SAP Fiori: 5+ Transaktionen (VA11, VA21, VA01, VL01N, VF01)

**Verwendungshäufigkeit:**
- Täglich/Kern: MM01, ME51N, ME21N, MIGO, VA01, VL01N, CO01
- Regelmäßig: CS01, CA01, MD02, MIRO, VF01
- Konfiguration: SPRO, OMSK, OPPR, VOV8

---

## Transaktionscode-Navigationstipps

### Häufige Pfade

**Materialwirtschaft:**
- `Logistik → Materialwirtschaft → Einkauf`
- `Logistik → Materialwirtschaft → Bestandsführung`

**Produktionsplanung:**
- `Logistik → Produktion → Stammdaten`
- `Logistik → Produktion → Fertigungssteuerung`

**Vertrieb:**
- `Logistik → Vertrieb → Verkauf`
- `Logistik → Vertrieb → Versand und Transport`

**Customizing:**
- `Werkzeuge → Customizing → IMG → Projekt bearbeiten`
- `SPRO` → Suche nach spezifischer Konfiguration

---

## Schnellreferenz-Karte

### Meist verwendete Transaktionen

| Aufgabe | Transaktion |
|---------|-------------|
| Material anlegen | MM01 |
| Bedarfsanforderung anlegen | ME51N |
| Bestellung anlegen | ME21N |
| Wareneingang buchen | MIGO |
| Rechnung buchen | MIRO |
| Stückliste anlegen | CS01 |
| Arbeitsplan anlegen | CA01 |
| MRP-Lauf | MD02 |
| Fertigungsauftrag anlegen | CO01 |
| Kundenauftrag anlegen | VA01 |
| Lieferung anlegen | VL01N |
| Faktura anlegen | VF01 |
| Kunde anlegen | XD01 |
| Lieferant anlegen | XK01 |
| Kostenstelle anlegen | KS01 |

---

*Diese Referenz deckt alle Transaktionscodes ab, die im dreiteiligen SAP ERP Implementierungsprojekt an der Johannes Kepler Universität (Juli-September 2025) verwendet wurden.*
