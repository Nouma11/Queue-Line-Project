# Queue Management System (C++) 🚀

A **Queue Management System** implemented in **C++**, designed to simulate a ticket-based queue system for businesses such as **banks, offices, and customer service centers**. The system allows for **issuing tickets, serving customers, and tracking queue status efficiently**.

## 📌 Features
✅ **Queue Ticketing System** with unique ticket IDs  
✅ **Serve Next Customer** functionality  
✅ **Track Waiting & Served Clients**  
✅ **Display Queue in LTR (left-to-right) & RTL (right-to-left)**  
✅ **Estimate Service Time for Waiting Customers**  

## 📂 Project Structure

## 📜 Implemented Class: `clsQueueLine`
| Method | Description |
|--------|------------|
| `IssueTicket()` | Issues a new ticket and adds it to the queue. |
| `ServeNextClient()` | Serves the next client and removes them from the queue. |
| `WhoIsNext()` | Returns the **next ticket number** in the queue. |
| `WaitingClients()` | Returns the number of waiting clients. |
| `ServedClients()` | Returns the number of clients who have been served. |
| `PrintTicketsLineLTR()` | Displays the queue **from first to last (→)**. |
| `PrintTicketsLineRTL()` | Displays the queue **from last to first (←)**. |
| `PrintAllTickets()` | Prints **detailed ticket information**. |
| `PrintInfo()` | Displays queue statistics (total, served, waiting clients). |

## 🛠 Installation & Setup
### 1️⃣ Clone the Repository
```sh
git clone https://github.com/YOUR_GITHUB_USERNAME/Queue_System.git
cd Queue_System
g++ -o main src/main.cpp
./main

#include <iostream>
#include "clsQueueLine.h"

using namespace std;

int main() {
    clsQueueLine PayBillsQueue("A0", 10);
    
    PayBillsQueue.IssueTicket();
    PayBillsQueue.IssueTicket();
    PayBillsQueue.IssueTicket();

    cout << "\nQueue Info:\n";
    PayBillsQueue.PrintInfo();

    PayBillsQueue.PrintTicketsLineRTL();
    PayBillsQueue.PrintTicketsLineLTR();

    PayBillsQueue.PrintAllTickets();

    PayBillsQueue.ServeNextClient();
    cout << "\nAfter Serving One Client:\n";
    PayBillsQueue.PrintInfo();

    return 0;
}
Queue Info:
    Prefix: A0
    Total Tickets: 3
    Served Clients: 0
    Waiting Clients: 3

Tickets: A01 <-- A02 <-- A03 <--

       ---Tickets---
       A01
       Waiting Clients = 3
       Serve Time In: 30 Minutes

After Serving One Client:
    Waiting Clients: 2
    Served Clients: 1

---

### 📌 What This README Provides:
✔ **Documents `clsQueueLine` queue system**  
✔ **Provides setup & compilation instructions**  
✔ **Shows example usage & expected output**  
✔ **Structured & professional documentation**  

This will make your **GitHub project look polished and easy to understand!** 🚀🔥
