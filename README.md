# 🐍 Python Environment Setup Guide (Linux Mint)

This repository contains a basic template and guide for setting up a Python development environment on **Linux Mint** using `python3`, `venv`, and `pip`.

---

## 🚀 Getting Started

Follow these steps to create and activate a Python environment, install packages, and run Python code.

---

### 1. ✅ Check Python Installation

Open your terminal and run:

```bash
python3 --version
```

If Python is not installed, install it using:

```bash
sudo apt update
sudo apt install python3 python3-pip
```

---

### 2. 📦 Install `venv` (Virtual Environment Module)

```bash
sudo apt install python3-venv
```

---

### 3. 📁 Create a Project Directory

```bash
mkdir my-python-project
cd my-python-project
```

---

### 4. 🔒 Create and Activate a Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

After activation, your terminal should show `(venv)` as a prefix.

---

### 5. ⬆️ Upgrade `pip` and Install Packages

```bash
pip install --upgrade pip
pip install requests  # Replace with your dependencies
```

---

### 6. 📝 Create and Run Python Code

Create a file:

```bash
nano hello.py
```

Add this content:

```python
print("Hello from Linux Mint!")
```

Save and exit (`Ctrl+O`, `Enter`, then `Ctrl+X`), then run:

```bash
python hello.py
```

---

### 7. 🧼 Deactivate the Virtual Environment

When you're done working:

```bash
deactivate
```

---

## 🧠 Tips

- Always activate your virtual environment before running or installing anything.
- Use `requirements.txt` to track dependencies:

```bash
pip freeze > requirements.txt
```

To install from `requirements.txt`:

```bash
pip install -r requirements.txt
```

---

## 📎 Resources

- [Python Docs](https://docs.python.org/3/)
- [pip Docs](https://pip.pypa.io/)
- [venv Docs](https://docs.python.org/3/library/venv.html)

---

## 📌 License

MIT License
