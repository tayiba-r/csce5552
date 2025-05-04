# csce5552
CSCE 5552.001 Cybersecurity Essentials - Lab submission

# HTB Challenge: Execute

**Course:** CSCE 5552 - Spring 2025  
**Contributors:** Harry Fu, Hollie King, Tanesha Hollingshed, Tayiba Raheem

## 🧠 Challenge Summary

The **"Execute"** challenge from Hack The Box presents a binary that filters input based on a blacklist. The objective is to bypass this filter, execute a shell, and retrieve a flag.

### 🔍 Provided Files

- `exe` – Compiled binary to analyze
- `blacklist` – Byte values to avoid in input
- `flag.txt` – Flag file (available locally and remotely)

---

## ⚙️ Program Behavior

- Reads 60 bytes into a buffer
- Checks input against a blacklist using `check()`
- If any blacklisted character is found, the program exits immediately

### 📛 Blacklist Highlights

```text
\x3b\x54\x62\x69\x6e\x73\x68\xf6\xd2\xc0\x5f\xc9\x66\x6c\x61\x67

