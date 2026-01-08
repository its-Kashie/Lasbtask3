# 🚗 Smart Parking Allocation & Zone Management System
**A DSA-focused Backend with a Modern Management Interface**

---

## 1️⃣ Project Overview
This system manages urban parking by dividing a city into a structured hierarchy. It focuses on efficient slot discovery, real-time request handling, and administrative safety through a rollback system.

* **Hierarchy:** `City` ⮕ `Zones` ⮕ `Parking Areas` ⮕ `Slots`
* **Core Features:** * Automated slot allocation (First-available strategy).
    * Cross-zone penalty logic for distance-based pricing.
    * Stack-based rollback (Undo functionality).
    * Live analytics dashboard.
* **Tech Stack:**
    * **Logic:** C++ (OOP & Data Structures)
    * **UI:** Web (HTML/CSS/JS) or Console Menu
    * **Data:** In-memory (Arrays, Stacks, Linked Lists)

---

## 2️⃣ Team Roles & Responsibilities

| Role | Responsibility | Key Focus |
| :--- | :--- | :--- |
| **👤 Person A** | **Core Backend & DSA** | Logic, Allocation Algorithms, Rollback Stack, Unit Tests. |
| **👤 Person B** | **UI, Integration & Docs** | Frontend/Menu, Input Validation, Reports, Final Documentation. |

> [!TIP]
> **Viva Note:** Ensure both members can explain why a **Stack** is used for rollback and how the **State Machine** prevents a completed booking from being cancelled.

---

## 3️⃣ 7-Day Implementation Plan

| Day | Phase | Deliverables |
| :--- | :--- | :--- |
| **Day 1** | **Design** | Finalize DS and Folder structure. |
| **Day 2** | **Core Classes** | Implement `Zone`, `Area`, and `Slot` logic. |
| **Day 3** | **State Machine** | `ParkingRequest` transitions (Pending → Allocated). |
| **Day 4** | **Engine** | Allocation logic (Same-zone vs Cross-zone). |
| **Day 5** | **Rollback** | Stack-based undo for the last $k$ transactions. |
| **Day 6** | **Analytics & UI** | Utilization stats & UI connectivity. |
| **Day 7** | **Finalization** | Bug fixing, 10+ Test Cases, & Readme. |

---

## 4️⃣ Project Structure 📂

📂 **Smart-Parking-System/** ├── 📂 **src/** │   ├── 📂 **core/** │   │   ├── 📄 `Zone.h` / `Zone.cpp`  
│   │   ├── 📄 `ParkingArea.h` / `ParkingArea.cpp`  
│   │   ├── 📄 `ParkingSlot.h` / `ParkingSlot.cpp`  
│   │   ├── 📄 `Vehicle.h` / `Vehicle.cpp`  
│   │   └── 📄 `ParkingRequest.h` / `ParkingRequest.cpp`  
│   ├── 📂 **engine/** │   │   ├── 📄 `AllocationEngine.h` / `AllocationEngine.cpp`  
│   │   └── 📄 `RollbackManager.h` / `RollbackManager.cpp`  
│   ├── 📂 **system/** │   │   └── 📄 `ParkingSystem.h` / `ParkingSystem.cpp`  
│   └── 📄 `main.cpp`  
├── 📂 **ui/** │   ├── 📄 `index.html`  
│   ├── 📄 `style.css`  
│   └── 📄 `app.js`  
├── 📂 **tests/** │   ├── 📄 `test_allocation.cpp`  
│   ├── 📄 `test_rollback.cpp`  
│   └── 📄 `test_states.cpp`  
├── 📂 **reports/** │   └── 📄 `report-day1.md` ... `report-day7.md`  
├── 📂 **docs/** │   ├── 📄 `design.md`  
│   └── 📄 `algorithms.md`  
├── 📄 `README.md`  
└── 📄 `.gitignore`

---

## 5️⃣ Setup Command (Terminal)
Copy and paste this into your terminal to create the skeleton:

```bash
mkdir -p Smart-Parking-System/{src/{core,engine,system},ui,tests,reports,docs} && \
touch Smart-Parking-System/src/core/{Zone,ParkingArea,ParkingSlot,Vehicle,ParkingRequest}.{h,cpp} \
Smart-Parking-System/src/engine/{AllocationEngine,RollbackManager}.{h,cpp} \
Smart-Parking-System/src/system/ParkingSystem.{h,cpp} \
Smart-Parking-System/src/main.cpp \
Smart-Parking-System/ui/{index.html,style.css,app.js} \
Smart-Parking-System/tests/{test_allocation.cpp,test_rollback.cpp,test_states.cpp} \
Smart-Parking-System/reports/report-day{1..7}.md \
Smart-Parking-System/docs/{design.md,algorithms.md} \
Smart-Parking-System/{README.md,.gitignore}
```