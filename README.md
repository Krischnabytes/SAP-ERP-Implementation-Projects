# SAP ERP Implementation Projects

> Hands-on SAP ECC experience across Materials Management, Production Planning, and Sales & Distribution modules

[![SAP ECC](https://img.shields.io/badge/SAP-ECC-0FAAFF?style=flat-square&logo=sap)](https://www.sap.com/)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=flat-square)]()
[![Period](https://img.shields.io/badge/Period-Jul--Sep%202025-blue?style=flat-square)]()

## 👤 About

**Name:** Krishnanunne Sajeev  
**Institution:** Johannes Kepler University, Linz  
**Program:** Business Informatics  
**SAP System:** H03, Client 352  

## 📋 Table of Contents

- [Overview](#overview)
- [Business Scenario](#business-scenario)
- [Technical Implementation](#technical-implementation)
- [Skills Demonstrated](#skills-demonstrated)
- [Project Phases](#project-phases)
- [Key Achievements](#key-achievements)
- [Problem-Solving Examples](#problem-solving-examples)
- [Documentation](#documentation)
- [Contact](#contact)

## 🎯 Overview

This repository showcases **hands-on SAP ERP implementation experience** from three progressive university courses implementing integrated business processes for Global Bike Inc.'s strategic e-bike market entry.

**Project Scope:**
- End-to-end business process configuration in live SAP ECC system
- Cross-module integration (MM ↔ PP ↔ SD)
- Master data creation and organizational structure setup
- SPRO customizing and process automation
- Real-world problem-solving with vendor constraints and quality issues

**Duration:** 3 months (July - September 2025)  
**Modules:** Materials Management (MM), Production Planning (PP), Sales & Distribution (SD), Controlling (CO)  
**Interfaces:** SAP GUI + SAP Fiori

## 🚴 Business Scenario

**Company:** Global Bike Inc. (GBI) Austria  
**Challenge:** Enter the e-bike market with new product line  
**Complexity:** Complete supply chain setup from procurement through production to sales

**Requirements:**
- New product: E-Bike Super Toll 1234-21
- 5-component manufacturing structure
- Supplier integration (GigaRad-21) with MOQ constraints
- Customer relationship (RadFan-21) with volume discounts
- Development cost center for R&D tracking
- Production site: Vienna plant (W000)

## 🔧 Technical Implementation

### Master Data Created

| Type | Description | ID/Material |
|------|-------------|-------------|
| **Finished Product** | E-Bike Super Toll 1234 | E-MTBA-21 |
| **Components** | Frame, Battery, Motor, Display, Wiring | 5 materials (MTBA2-21, Battery-21, etc.) |
| **Vendor** | Component Supplier | GigaRad-21 (48391) |
| **Customer** | E-Bike Retailer | RadFan-21 (200098) |
| **Cost Center** | Development Department | 30-3-21 |

### Business Processes Implemented

#### 1️⃣ Procure-to-Pay Cycle (MM)
```
Purchase Requisition (ME51N)
    ↓
Purchase Order (ME21N)
    ↓
Goods Receipt (MIGO)
    ↓
Invoice Verification (MIRO)
```

#### 2️⃣ Order-to-Cash Cycle (SD)
```
Customer Inquiry (VA11)
    ↓
Sales Quotation (VA21)
    ↓
Sales Order (VA01)
    ↓
Delivery (VL01N/VL02N)
    ↓
Customer Invoice (VF01)
```

#### 3️⃣ Production Planning & Execution (PP)
```
BOM Creation (CS01)
    ↓
Routing Creation (CA01)
    ↓
MRP Run (MD02/MD04)
    ↓
Production Order (CO01)
    ↓
Production Confirmation (CO11N)
```

### SPRO Customizing Objects

| Object | ID | Purpose |
|--------|-----|---------|
| Purchasing Group | G21 | Procurement organization |
| Production Control Profile | G00021 | Process automation |
| Production Controller | G21 | Responsibility assignment |
| Sales Document Type | ZG21 | Custom order processing |

## 💡 Skills Demonstrated

### SAP Technical Skills

**Transaction Codes Mastered (30+):**
- **MM:** MM01, MM02, ME51N, ME21N, MIGO, MIRO, XK01
- **PP:** CS01, CA01, MD02, MD04, CO01, CO02, CO11N
- **SD:** VA11, VA21, VA01, VL01N, VL02N, VF01, XD01
- **CO:** KS01, KS02

**Interfaces:**
- SAP GUI (traditional interface)
- SAP Fiori (modern web UI) - 4+ transactions

**Configuration:**
- SPRO Customizing
- Organizational structure setup
- Master data views configuration

### Business Skills

- End-to-end process understanding
- Cross-module integration
- Business process modeling (BPMN)
- Strategic analysis (Porter's Value Chain)
- Professional documentation (German)

## 📚 Project Phases

### Phase 1: Einführung in ERP-Systeme
**Period:** July-August 2025  
**Focus:** Foundation and basic business cycles  
**Status:** ✅ Completed

**Deliverables:**
- Complete procure-to-pay implementation
- Order-to-cash cycle execution
- 6 material masters created
- 2 business partners configured
- Professional case study documentation

[📄 View Phase 1 Documentation](./Phase1_Einfuehrung/)

---

### Phase 2: ERP-Systeme Anwendungen I
**Period:** September 2025  
**Focus:** Production planning and Fiori proficiency  
**Status:** ✅ Completed

**Deliverables:**
- BOM and routing creation
- MRP and production order execution
- SAP Fiori transactions (4+)
- Porter's Value Chain analysis
- Process flow diagrams (BPMN)

[📄 View Phase 2 Documentation](./Phase2_Anwendung_I/)

---

### Phase 3: ERP-Systeme Anwendungen II
**Period:** September 2025  
**Focus:** System customizing and automation  
**Status:** ✅ Completed (~85%)

**Deliverables:**
- 4 customizing objects created
- Process automation configuration
- System testing and validation
- Technical documentation

[📄 View Phase 3 Documentation](./Phase3_Anwendung_II/)

## 🏆 Key Achievements

- ✅ **30+ SAP transactions** executed successfully
- ✅ **8 master data objects** created (6 materials, 2 business partners)
- ✅ **3 complete business cycles** implemented end-to-end
- ✅ **4 customizing objects** configured for process automation
- ✅ **Dual interface proficiency** - SAP GUI and Fiori
- ✅ **70+ pages** of professional documentation
- ✅ **Real-world problem solving** - MOQ conflicts, defective goods, system errors

## 🔥 Problem-Solving Examples

### Challenge 1: Minimum Order Quantity Conflict

**Problem:** Supplier GigaRad-21 required MOQ of 50 units per component, but development only needed 15 for prototyping.

**Solution:** 
- Ordered supplier minimum (50 units)
- Managed excess inventory (35 units) with warehouse planning
- Documented business impact and cost implications

**Skills:** Procurement negotiation, inventory management, business constraint handling

---

### Challenge 2: Defective Goods Handling

**Problem:** 5 display units arrived with surface defects, requiring returns and adjusted invoicing.

**Solution:**
- Executed MIGO returns transaction with proper reason codes
- Adjusted goods receipt quantities (30 good vs 35 received)
- Reconciled invoice verification for accepted quantity only

**Skills:** Quality management, returns processing, three-way matching (PO-GR-IR)

---

### Challenge 3: Production Control Profile Configuration

**Problem:** Initial production order creation failed - routing not properly linked to material master.

**Solution:**
- Used alternative MRP planning route (MD02 → CO41)
- Created planned orders, then converted to production orders
- Explicitly specified production controller G21 in conversion

**Skills:** System troubleshooting, PP module dependencies, alternative solution paths

## 📖 Documentation

### Repository Structure

```
SAP-ERP-Projects/
│
├── README.md                          # This file
├── Portfolio_Overview.pdf             # Executive summary
│
├── Phase1_Einfuehrung/
│   ├── Case_Study.pdf                # Complete documentation
│   ├── Screenshots/                  # Key transactions
│   └── Transaction_Summary.md        # Reference list
│
├── Phase2_Anwendung_I/
│   ├── Case_Study.pdf                # Advanced processes
│   ├── Porter_Value_Chain.pdf        # Strategic analysis
│   ├── Process_Flow_Diagram.pdf      # BPMN diagrams
│   └── Screenshots/                  # Fiori & production planning
│
├── Phase3_Anwendung_II/
│   ├── Customizing_Documentation.pdf # SPRO configurations
│   ├── Test_Results.pdf              # Validation outcomes
│   └── Screenshots/                  # Configuration screens
│
└── Resources/
    ├── Transaction_Code_Reference.md # All T-codes used
    ├── Master_Data_Overview.md       # Created objects
    └── System_Architecture.md        # Technical setup
```

### Available Documents

- 📄 **Portfolio Overview** - Executive summary for recruiters
- 📄 **Case Studies (3)** - Detailed implementation documentation
- 📄 **Process Diagrams** - BPMN flowcharts
- 📄 **Strategic Analysis** - Porter's Value Chain
- 📄 **Screenshots** - Key transactions and configurations
- 📄 **Transaction Reference** - Complete T-code list

## 🎓 Courses Completed

1. **256.904 Einführung in ERP-Systeme**  
   Introduction to ERP Systems

2. **256.905 ERP-Systeme Anwendungen I**  
   ERP Systems Applications I

3. **256.907 ERP-Systeme Anwendungen II**  
   ERP Systems Applications II

**Institution:** Johannes Kepler University, Linz  
**Instructor:** Barbara Krumay et al.  
**Period:** Summer Semester 2025

## 🌟 Why This Matters

This project demonstrates:

1. **Real System Experience** - Not simulations, actual SAP ECC work
2. **Problem-Solving Ability** - Handled real-world complications
3. **Cross-Module Understanding** - How MM, PP, SD integrate
4. **Modern Skills** - Both traditional GUI and modern Fiori
5. **Business Acumen** - Strategic analysis and process thinking
6. **Professional Documentation** - Complete technical writing

## 📬 Contact

**Krishna Sajeev**  
Business Informatics Student  
Johannes Kepler University, Linz

📧 Email: [Your Email]  
💼 LinkedIn: [Your LinkedIn]  
🌐 Portfolio: [This Repository]

---

## 📝 License

This repository contains academic project work completed as part of university coursework. Documentation and screenshots are for portfolio demonstration purposes.

---

## 🙏 Acknowledgments

- Johannes Kepler University ERP Systems courses
- Instructor: Barbara Krumay
- SAP University Alliance Program

---

<div align="center">

**⭐ If you're a recruiter:** This repository showcases hands-on SAP implementation skills ready for internship application.

**📧 Interested in discussing SAP opportunities?** Please reach out!

</div>
