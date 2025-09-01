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

1. **Input Bank Details**
   - Enter the number of banks.  
   - For each bank, provide:  
     - Bank name  
     - Number of supported payment modes  
     - List of payment modes  

2. **Input Transactions**
   - Enter the number of transactions.  
   - For each transaction, provide:  
     ```
     <SenderBank> <ReceiverBank> <Amount>
     ```

3. **Compute Net Balances**
   - The system calculates each bank’s **net amount**:  
     - Positive → Bank should receive money  
     - Negative → Bank needs to pay money  
     - Zero → No dues  

4. **Match Transactions**
   - Payers and receivers are matched:  
     - If they **share a common payment mode**, the transaction is settled directly.  
     - If **no payment mode matches**, the system routes the transaction via the **World Bank** (which supports all payment modes).  

5. **Minimize Transactions**
   - The algorithm ensures that the **fewest number of transactions** are made while clearing all dues.  

6. **Display Results**
   - The system prints the **final minimized list of transactions** with payment modes used.
  
