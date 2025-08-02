# 🛒 Super Market Billing System (C++)

The **Super Market Billing System** is a simple, console-based C++ application designed to handle basic inventory management and billing for a small retail setup. Built using core C++ concepts such as classes, file handling, and stream manipulation, this project allows users to add items to an inventory and generate bills by selecting available items and quantities.

---

## 🔧 Functionality

The system provides two main operations:

1. **Add Item to Inventory**  
   Users can add a new item by entering the item name, rate (price), and quantity available. This information is stored in a local text file (`bill text.txt`) using file I/O so the data persists between sessions.  

2. **Print Customer Bill**  
   Customers can purchase items by specifying the item name and quantity they want. The system checks if the item exists and if enough stock is available. It then calculates the amount, updates the inventory by subtracting the sold quantity, and finally displays the total bill.

---

## 📁 File Handling

- **`bill text.txt`**: Maintains the inventory with details like item name, rate, and quantity.
- **`bill temp text.txt`**: Temporarily holds updated inventory during billing, which then replaces the original file.

---

## 💡 Concepts Used

- Object-Oriented Programming (OOP)
- File input/output using `fstream`
- `stringstream` for parsing inventory data
- Windows API (`windows.h`) for screen clearing and delays

---

## ✅ Highlights

- Menu-driven interface with clear prompts
- Persistent inventory management using text files
- Simple billing logic that automatically updates stock levels
- Portable code structure with modular functions

---

## ⚠️ Limitations

- File paths are hardcoded and specific to Windows
- No input validation (e.g., invalid quantities or non-existent items)
- Dependent on console environment (`system("cls")`, `Sleep()`)

---

## 🔮 Future Enhancements

- Make file paths dynamic or user-configurable
- Cross-platform support (remove Windows-specific code)
- Add GUI using frameworks like Qt or GTK
- Use databases like SQLite for better data handling
- Include features like item deletion, search, or transaction history

---

> 🎓 This project is ideal for beginners learning C++ and file handling.  
> Feel free to fork or improve it!
