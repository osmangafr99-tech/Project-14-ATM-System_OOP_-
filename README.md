# 🏧 Project 14 — ATM System (OOP)

## 📌 Overview

**Project 14 — ATM System (OOP)** is a complete Object-Oriented reimplementation of the previous structured project  
**Project 4.1 — ATM System (1st Extension)**.

After completing **Course 11 — OOP as it Should Be (Applications)** and finishing **Projects 12 & 13**, we were required to rebuild the ATM system using **Object-Oriented Programming principles**, clean architecture, and real-world inspired design.

Although the ATM system is **fully independent from the Bank System**, both systems **share the same clients database**, exactly as in real-world banking environments.

---

## 🎯 Project Objectives

- Convert a **procedural (structured)** ATM system into a **fully OOP-based system**
- Apply all **OOP concepts, rules, and best practices**
- Build a **clean, scalable, and maintainable** architecture
- Simulate **real-world ATM behavior** with proper security constraints

---

## 🧠 System Design & Architecture

### 🔹 Object-Oriented Structure

- Each screen is implemented as a **separate class**
- All screen classes inherit from a common base class: `clsScreen`
- Full separation between:
  - **UI (Screens)**
  - **Business Logic**
  - **Data Access & Files**
- All class names start with `cls`
- All private members start with `_`

This structure makes the system:
- Easy to maintain
- Easy to extend
- Safe for future modifications

---

## 🔐 Security & Safety Considerations

- Passwords are **never displayed** on any screen
- Passwords are **encrypted** in all external files
- Login is limited to **3 failed attempts**, after which the system locks
- All login attempts are logged in an external file
- All money transfers are recorded in a dedicated log file

---

## 👤 ATM vs Bank System — Design Differences

Unlike the Bank System, the ATM System:

❌ Does NOT allow:
- Adding new clients  
- Deleting clients  
- Updating client personal data  
- Viewing clients list  

✅ Allows only:
- Balance updates
- PIN code changes

### 🛑 Design Reason

Client personal data is treated as **read-only** to prevent misuse by developers using the Bank Client object and to reflect real-world ATM limitations.

---

## 🔁 Structured vs OOP Implementation

### 🧩 Old Structured Version
- Function-based design
- Weak separation of concerns
- Hard to scale and maintain

### 🧱 New OOP Version
- Unified and consistent architecture
- High readability
- Easy extensibility
- Real-world inspired behavior

---

## 🧾 Implemented Features

- Secure login system with validation
- Quick Withdraw
- Normal Withdraw
- Deposit
- Check Balance
- Change PIN Code
- Client Information Screen
- Money Transfer between accounts
- Transfer logging
- Login activity logging
- Integrated **Currency Exchange module** (from Course 11 projects)

---

## 🗂️ Global Client Management

The currently logged-in client is loaded once and stored in a **global variable**, allowing all screens to access it safely without repeated authentication.

---

## 🧪 Validation & Data Integrity

- Full validation on all user inputs
- Client existence validation
- Balance validation before withdrawals and transfers
- Controlled access to sensitive operations

---

## 📁 External Files

- `Clients.txt` → Clients database  
- `LoginRegister.txt` → Login history  
- `TransferLog.txt` → Transfer history  

> All sensitive data is stored in encrypted form.

---

## 📚 Learning Outcomes

This project applies and reinforces:

- Encapsulation
- Abstraction
- Inheritance
- Polymorphism
- Clean Code principles
- Real-world system simulation
- Proper OOP-based system design

---

## 🧑‍🏫 Instructor & Platform

- **Instructor:** Dr. Mohammed Abu-Hadhoud  
- **Platform:** Programming Advices  

Special thanks for the structured learning path, professional coding standards, and real-world inspired OOP methodology.

---

## 🚀 Final Notes

This project demonstrates how applying proper **Object-Oriented Design** transforms a procedural system into a **professional, scalable, and secure application**.

---

💻 Built with **C++** using **Object-Oriented Programming (OOP)**
