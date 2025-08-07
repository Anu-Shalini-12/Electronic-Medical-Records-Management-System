# 🏥 Electronic Medical Records Management System using Hyperledger Fabric

## ❗ Problem Statement

Traditional Electronic Medical Record (EMR) systems face critical challenges:

- ❌ Lack of interoperability and centralized control  
- 🔓 Vulnerable data storage prone to tampering or leaks  
- 📝 Manual updates resulting in inconsistent patient records  
- 🔍 Limited visibility for both patients and healthcare providers  

These issues can lead to poor healthcare decisions, data breaches, and a lack of trust in digital health systems.

---

## 🎯 Project Objective

To develop a **blockchain-based Electronic Medical Records (EMR) Management System** using **Hyperledger Fabric** that:

- 🛡️ Ensures **secure, immutable** storage of medical records  
- 🔐 Provides **controlled access** to authorized healthcare personnel  
- 🔄 Supports **real-time updates** to patient status and treatments  
- ✅ Enhances **data integrity, transparency, and trust** in EMRs  

---

## 🛠️ Technologies Used

| Technology         | Description                                     |
|--------------------|-------------------------------------------------|
| Hyperledger Fabric | Modular permissioned blockchain framework       |
| Java Chaincode     | Smart contract logic for EMR management         |
| Fabric CA          | Manages identities and certificates             |
| Java SDK           | Client-side app integration                     |
| CouchDB            | World state database (key-value storage)        |
| Practical Lab      | Testbed environment for deployment and testing  |

---

## 🔁 Chaincode Functionalities

Implemented in `MedicalRecordContract.java`:

1. **`initLedger()`**  
   - Preloads the ledger with demo EMRs for testing and validation

2. **`createRecord(id, name, diagnosis, treatment, date)`**  
   - Adds a new medical record with complete patient and treatment details

3. **`readRecord(id)`**  
   - Retrieves a specific patient's medical record by ID

4. **`updateRecord(id, name, diagnosis, treatment, date)`**  
   - Updates the existing medical record with the latest diagnosis/treatment  

---

## 🗂️ Workflow Summary

1. ✅ Admin initializes the blockchain ledger with sample EMRs  
2. ➕ New records are added using `createRecord()`  
3. 🔁 Patient records are updated post consultation or treatment  
4. 🔍 Authorized healthcare personnel retrieve records via `readRecord()`  

Each transaction is recorded immutably on the blockchain ledger ensuring auditability and tamper-resistance.

---

## 🏗️ Hyperledger Fabric Architecture

- **Peers** – Host and execute chaincode, maintain ledger state  
- **Orderer** – Bundles transactions into blocks  
- **Certificate Authority (CA)** – Manages identities, issues certificates  
- **Chaincode** – Contains EMR management business logic  
- **CouchDB Ledger** – Stores current state and historical block data  

---

## 🌟 Features and Benefits

| Feature                 | Benefit                                           |
|-------------------------|---------------------------------------------------|
| 🔐 Immutable Ledger     | Tamper-proof record management                    |
| 🕒 Real-time Updates     | Accurate and up-to-date patient information       |
| 📄 Paperless Automation | Reduces manual data entry and human error         |
| 🔐 Role-Based Access    | Restricts record access to authorized personnel   |
| 🔍 Query Support        | Enables instant patient record look-up by ID      |

---

## ✅ Testing & Verification

- All chaincode functions tested using **Fabric CLI** and **Java SDK**  
- Peer logs and **CouchDB** world state used to verify transactions  
- Verified functionality: record creation, reading, and real-time updates  

---

## 📸 Screenshots Overview

| Operation     | Screenshot | Description                              |
|---------------|------------|------------------------------------------|
| initLedger    | ✅ Included | Initializes ledger with test records     |
| createRecord  | ✅ Included | Adds a new patient record                |
| readRecord    | ✅ Included | Fetches medical data by patient ID       |
| updateRecord  | ✅ Included | Updates patient diagnosis/treatment info |





