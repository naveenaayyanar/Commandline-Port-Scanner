# 🔍 Python Port Scanner

A fast, multithreaded TCP port scanner written in Python.
This tool checks which ports on a target machine are open and accepting connections.

---

## 📌 Features

* Scans all **65,535 TCP ports**
* Uses **multithreading** for speed
* Works with **IP addresses and domain names**
* Displays all **open ports**
* Simple, lightweight, and easy to modify

---

## 🛠 Requirements

* Python **3.7+**
* Works on **Windows, Linux, and macOS**
* No external libraries required

---

## ▶️ Installation

1. Download or copy `scanner.py`
2. Open a terminal or command prompt in the file’s directory

---

## ▶️ Usage

```bash
python scanner.py <target>
```

### Examples

Scan a website:

```bash
python scanner.py scanme.nmap.org
```

Scan your router:

```bash
python scanner.py 192.168.1.1
```

Scan your own PC:

```bash
python scanner.py localhost
```

---

## 📤 Example Output

```
--------------------------------------------------
Scanning target 192.168.1.1
Time started: 2026-02-15 13:22:10
--------------------------------------------------
Port 22 is open
Port 80 is open
Port 443 is open

Scan completed!
```

---

## ⚠️ Legal Disclaimer

This tool is for **educational and authorized testing only**.

You may only scan:

* Systems you own
* Networks you administer
* Targets where you have written permission

Unauthorized port scanning is considered **illegal** in many countries and may result in:

* IP bans
* Legal action
* Criminal charges

The developer is **not responsible** for misuse.

---

## 🚨 Performance Warning

This scanner creates **one thread per port (65,535 threads)**, which can:

* Crash Python
* Freeze your system
* Trigger firewalls

It is recommended to limit the number of threads for real-world use.

---

## 📚 How it works

The scanner:

1. Resolves the target hostname to an IP
2. Attempts a TCP connection to each port
3. If a connection succeeds, the port is marked **open**

---

## 🧑‍💻 Author
Naveena
