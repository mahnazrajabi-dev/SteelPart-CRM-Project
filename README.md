# 🏭 SteelParts CRM — Salesforce Sales Cloud Portfolio Project

**Built by:** Mahnaz Rajabi | Salesforce Business Analyst | Salesforce Admin
**Industry:** Steel & Foundry (B2B)
**Platform:** Salesforce Sales Cloud
**Contact:** mahnazrajabi444@gmail.com

---

## 📌 Project Overview
A full end-to-end Salesforce Sales Cloud CRM implementation for a fictional B2B steel industry company — **SteelParts**. Built to demonstrate real-world Salesforce Admin and Business Analyst skills for enterprise B2B sales operations.

---

## ✅ What Was Built

### 1. Lead Management & Conversion
- Created and qualified 5 B2B leads representing major European steel companies
- Converted leads into linked **Accounts, Contacts, and Opportunities**
- Companies: TŘINECKÉ ŽELEZÁRNY, Voestalpine AG, ArcelorMittal, U.S. Steel Košice, Salzgitter AG

### 2. Product Catalog & Price Book
- Created custom Price Book: **SteelParts Standard Pricing**
- Added 6 industrial products with SKUs and pricing (PLN)

| SKU | Product | Price |
|-----|---------|-------|
| SP-001 | Industrial Roller Bearing | 85 zł |
| SP-002 | Mechanical Seal Assembly | 120 zł |
| SP-003 | Gear Coupling Unit | 340 zł |
| SP-004 | Furnace Refractory Brick | 45 zł |
| SP-005 | Hydraulic Pump Seal Kit | 95 zł |
| SP-006 | Conveyor Belt Drive Chain | 280 zł |

### 3. Opportunity Management
- Attached all 6 products to each Opportunity
- Full itemised sales records with quantities and pricing

### 4. Process Automation — Flow Builder
- Built a **Record-Triggered Flow** on Opportunity object
- Trigger: Stage updated to **Closed Won**
- Action: Auto-sets Close Date to current date
- Result: Zero manual entry, clean CRM data

### 5. Custom Reports & Dashboards
- Built Opportunities Pipeline report grouped by Stage
- Columns: Account Name, Opportunity Name, Stage, Amount, Close Date, Probability
- Full pipeline visibility for sales management

### 6. Validation Rules

| Rule Name | Object | Business Logic | Error Message |
|---|---|---|---|
| Minimum Order Value | Opportunity | Amount < 500 | "Minimum order value is 500 PLN" |
| Close Date Not In Past | Opportunity | Close Date cannot be in past when Stage is Prospecting or Qualification | "Close Date cannot be in the past for active opportunities" |
| Opportunity Name Must Include Year | Opportunity | Name must contain 2024, 2025 or 2026 | "Opportunity Name must include the year (e.g. Q1 2025 - Voestalpine)" |

📸 Screenshot: `validation-rules.png`

### 7. Permission Set — SteelParts Sales Rep

Created a Permission Set to control access for sales 
representatives in the SteelParts org.

- Read + Edit on Opportunities
- Read + Edit on Contacts
- Read only on Accounts
- No delete permissions on any object

📸 Screenshot: `permission-set.png`

### 8. Screen Flow — New Parts Inquiry

Built a Screen Flow to capture inbound parts inquiries 
and automatically create a Lead record.

- Screen 1: collects Company Name, Contact Name, 
  Product Interest, Urgency Level
- Creates Lead record automatically with LeadSource = Web
- Screen 2: confirmation message to user
- Flow activated and tested end to end

📸 Screenshot: `screen-flow.png`

### 9. Approval Process — Large Order Approval

Built an Approval Process for high-value opportunities 
requiring manager sign-off before closing.

- Triggered when Opportunity Amount exceeds 10,000 PLN
- Approved: Stage updates to Closed Won
- Rejected: Stage updates to Needs Review
- Email alert sent to opportunity owner on rejection

📸 Screenshot: `approval-process.png


## 🛠 Salesforce Features Used

- Leads & Lead Conversion
- Accounts, Contacts, Opportunities
- Products & Price Books
- Flow Builder (Record-Triggered Flow)
- Flow Builder (Screen Flow)
- Reports & Dashboards
- Lightning App Builder
- Validation Rules
- Permission Sets
- Approval Processes
- Process Automation

## 🎯 Skills Demonstrated
- Salesforce Sales Cloud configuration
- B2B CRM implementation
- Process automation without code
- Data modelling and relationships
- Pipeline reporting and analytics

---

## 📸 Screenshots
### Opportunities Pipeline
![Pipeline Report](pipeline-report.png)

### Price Book
![Price Book](price-book.png)

### Opportunity Record with Products
![Opportunity Record](opportunity-record.png)

### Flow Builder Automation
![Flow Builder](flow-builder.png)

### Accounts List
![Accounts List](accounts-list.png)
---

## 👩‍💼 About Me
**Mahnaz Rajabi** — Salesforce Business Analyst | Salesforce Admin
- 📧 mahnazrajabi444@gmail.com
