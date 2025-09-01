# 💰 Cash Flow Minimizer System

This project implements a **Cash Flow Minimization System** in C++ that reduces the number of transactions among multiple banks.  
It ensures that banks settle debts efficiently while considering different payment modes.  
If no direct payment mode is shared between two banks, a **World Bank (intermediary)** is used for settlement.

---

## 📌 Features
- Minimizes the **total number of transactions** among banks.
- Handles **multiple banks** with different payment modes.
- Supports a **World Bank** with all available payment modes to act as an intermediary.
- Uses **graph data structures** (adjacency matrix) to represent transactions.
- Computes **net amount per bank** (debit/credit balance).
- Matches banks based on **common payment modes**; if none exist, transactions are routed via the World Bank.
- Prints the **final minimized transaction list**.

---

## 🛠️ Tech Stack
- **Language:** C++  
- **Data Structures:** Graphs, Sets, Vectors, Maps  
- **Algorithm:** Greedy-based settlement of debts with payment mode matching  

---

## 🚀 How It Works
1. Input the number of banks.
2. Provide each bank’s:
   - Name  
   - Number of supported payment modes  
   - The list of payment modes
3. Input the number of transactions.
4. Provide each transaction in the format:  
