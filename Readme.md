# 💸 Financial Settlement Engine (Splitwise Logic)

A high-performance Command Line Interface (CLI) application designed to optimize and simplify group debts. Using advanced graph-based algorithms, this engine minimizes the total number of transactions required to settle balances among multiple parties.

---

## 🚀 Key Features

* Algorithmic Optimization: Implements a Greedy/Min-Flow approach to simplify complex debt webs.
* Interactive CLI: Uses pynput for smooth keyboard-based menu navigation.
* Structured Data Visualization: Generates clean, formatted settlement reports using `prettytable`.
* Validation Logic: Handles edge cases such as circular debts and multi-currency inputs.

---

🧠 The Algorithm (JPMC Technical Focus)

Most basic splitting apps use $O(N^2)$ complexity. This engine is designed to focus on **Efficiency**:

1.  Net Balance Calculation: First, the system calculates the net amount owed to or by every person.
2.  Greedy Settlement: Utilizing a Min-Heap and Max-Heap approach, the algorithm matches the largest creditor with the largest debtor.
3.  Path Compression: This reduces the total number of transactions from $N(N-1)$ to a maximum of $N-1$ transactions, where $N$ is the number of people.

---

🛠️ Tech Stack

* Language: Python 3.x
* Libraries:
     prettytable: For formatted terminal output.
    pynput: For interactive menu navigation.
    colorama: For enhanced UI/UX in the terminal.


## ⚙️ Installation & Setup

1. Clone the repository
   git clone https://github.com/RAHUL-TRIPATHI07/Splitwise

   cd Financial-Settlement-Engine
   
3. Install dependencies:
   pip install -r requirements.txt

3.Run the application:
  python main.py


📈 Challenges & Learnings

State Management: Learned to manage real-time updates of net balances as users add or remove expenses.
Error Handling: Implemented robust input validation to prevent system crashes during malformed numeric entries.
Optimization: Focused on reducing algorithmic time

