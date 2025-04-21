
# 💳 Banking App

A simple command-line banking system built with Python and SQLite that simulates the basic operations of a banking application. It uses the **Luhn algorithm** to validate card numbers and provides features like balance check, money transfer, and account management.

---

## 🚀 Features

- ✅ **Create Account** with auto-generated card number and PIN using Luhn algorithm.
- 🔐 **Login** with card number and PIN verification.
- 💰 **Check Balance** and **Add Income** to your account.
- 🔄 **Money Transfer** to other card numbers (Luhn check included).
- ❌ **Close Account** permanently.
- 🧠 **Persistent Storage** using `sqlite3` to safely manage user data.

---

## 🛠 Technologies Used

- **Python 3**
- **SQLite3** – For storing card details.
- **Luhn Algorithm** – To validate card numbers.

---

## 📦 Installation & Running

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/banking-app.git
   cd banking-app
   ```

2. **Run the app:**
   ```bash
   python3 "Python Proj.py"
   ```

> ⚠️ Make sure `sqlite3` is available in your Python environment.

---

## 🧪 Sample Usage

```bash
1. Create an account
2. Log into account
0. Exit

# After login:
1. Balance
2. Add income
3. Do transfer
4. Close account
5. Log out
0. Exit
```

---

## 🛡 Security

- Card numbers are generated and validated using **Luhn algorithm**.
- All sensitive actions are protected with PIN-based authentication.

---

## 📁 Database Info

The app creates a database file named `card.s3db` with a table `card`:
```sql
CREATE TABLE IF NOT EXISTS card(
    id INTEGER PRIMARY KEY,
    number TEXT,
    pin TEXT,
    balance INTEGER DEFAULT 0
);
```

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).
