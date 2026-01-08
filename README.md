Perfect, this is a smart move 😄
UI + any language = no viva + free marks → we’ll play this strategically.

Below is a complete, practical guide so you can finish this in 7 days, push daily reports, and look solid in front of sir.


---

1️⃣ Project Outline (High-Level)

Project Name
Smart Parking Allocation & Zone Management System

Core Idea
A city is divided into zones → zones have parking areas → areas have slots.
Vehicles request parking → system allocates slots → handles cancellation + rollback → shows analytics via UI.

Tech Stack (Recommended)

Backend logic: C++ (DSA-heavy, sir-friendly)

UI: Simple Web UI (HTML + CSS + JS) OR Console UI with menus

Data Storage: In-memory (arrays, linked lists, stacks, queues)

Reports: Daily report-dayX.md



---

2️⃣ Divide Work Between 2 Persons (Very Important)

👤 Person A – Core DSA & Backend Logic

Responsible for marks safety

Zone, ParkingArea, ParkingSlot classes

ParkingRequest lifecycle (state machine)

Allocation logic

Rollback logic (stack-based)

Analytics calculations

Unit test cases


👤 Person B – UI + Integration + Reports

Responsible for no viva 😎

UI (web or menu-driven)

Connect UI with backend

Input validation

Visualization (tables, stats)

Daily reports

Final documentation


> ⚠️ BOTH should understand everything (sir may randomly ask).




---

3️⃣ 1-Week Completion Plan (Daily Breakdown)

📅 Day 1 – Project Setup & Design

Finalize data structures

Create folder structure

Write design.md outline

Push Day 1 report


📅 Day 2 – Zone & Slot Management

Implement:

Zone

ParkingArea

ParkingSlot


Basic slot availability logic

Push Day 2 report


📅 Day 3 – Parking Requests & State Machine

ParkingRequest class

Enforce valid transitions

Prevent invalid state changes

Push Day 3 report


📅 Day 4 – Allocation Engine

Same-zone allocation

Cross-zone allocation + penalty

First-available strategy

Push Day 4 report


📅 Day 5 – Cancellation & Rollback

Stack-based rollback

Undo last k allocations

Restore slot + request state

Push Day 5 report


📅 Day 6 – Analytics + UI

Average duration

Zone utilization

Peak zones

UI screens

Push Day 6 report


📅 Day 7 – Testing & Final Touch

10+ test cases

Bug fixing

README + screenshots

Final report

Push Day 7 report



---

4️⃣ Complete Folder & File Structure

Smart-Parking-System/
│
├── src/
│   ├── core/
│   │   ├── Zone.h
│   │   ├── Zone.cpp
│   │   ├── ParkingArea.h
│   │   ├── ParkingArea.cpp
│   │   ├── ParkingSlot.h
│   │   ├── ParkingSlot.cpp
│   │   ├── Vehicle.h
│   │   ├── Vehicle.cpp
│   │   ├── ParkingRequest.h
│   │   ├── ParkingRequest.cpp
│   │
│   ├── engine/
│   │   ├── AllocationEngine.h
│   │   ├── AllocationEngine.cpp
│   │   ├── RollbackManager.h
│   │   ├── RollbackManager.cpp
│   │
│   ├── system/
│   │   ├── ParkingSystem.h
│   │   ├── ParkingSystem.cpp
│
│   ├── main.cpp
│
├── ui/
│   ├── index.html
│   ├── style.css
│   ├── app.js
│
├── tests/
│   ├── test_allocation.cpp
│   ├── test_rollback.cpp
│   ├── test_states.cpp
│
├── reports/
│   ├── report-day1.md
│   ├── report-day2.md
│   ├── report-day3.md
│   ├── report-day4.md
│   ├── report-day5.md
│   ├── report-day6.md
│   ├── report-day7.md
│
├── docs/
│   ├── design.md
│   ├── algorithms.md
│
├── README.md
└── .gitignore


---

5️⃣ Terminal Command to Create Structure (One Shot)

```bash
mkdir -p Smart-Parking-System/{src/{core,engine,system},ui,tests,reports,docs}

touch Smart-Parking-System/src/core/{Zone,ParkingArea,ParkingSlot,Vehicle,ParkingRequest}.{h,cpp}
touch Smart-Parking-System/src/engine/{AllocationEngine,RollbackManager}.{h,cpp}
touch Smart-Parking-System/src/system/{ParkingSystem}.{h,cpp}
touch Smart-Parking-System/src/main.cpp

touch Smart-Parking-System/ui/{index.html,style.css,app.js}

touch Smart-Parking-System/tests/{test_allocation.cpp,test_rollback.cpp,test_states.cpp}

touch Smart-Parking-System/reports/report-day{1..7}.md

touch Smart-Parking-System/docs/{design.md,algorithms.md}

touch Smart-Parking-System/{README.md,.gitignore}

```bash

---

6️⃣ Daily Report Format (Use This)

# Day X Report

## Work Done
- Implemented zone structure
- Added parking slot logic

## Data Structures Used
- Arrays
- Linked Lists

## Issues Faced
- Slot state sync issue

## Next Day Plan
- Implement allocation engine


---
