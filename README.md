# 🔎 Cybersecurity Internship — Password Cracking Labs

![Program](https://img.shields.io/badge/Program-Cybersecurity%20Internship-6C63FF?style=flat-square)
![Week](https://img.shields.io/badge/Week-3-FF6B6B?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-2ECC71?style=flat-square)

Personal lab notes from my cybersecurity internship, covering hands-on password auditing and hash-cracking exercises.

> ⚠️ All work below was carried out on files/systems I was explicitly authorized to test, inside a supervised training environment.

---

## 🧭 At a Glance

| | |
|---|---|
| **Intern** | Saud Ur Rehman Abbasi |
| **Program** | Networkwalks |
| **Mentor** | Waqas Karim (CCIE) |
| **Week** | 3 |
| **Focus Area** | Password cracking & hash analysis |
| **Labs Completed** | 2 |

---

## 🗂️ Labs

<summary><b>Lab 1 — John the Ripper + Johnny GUI</b></summary>

**Goal:** Recover the password on a protected PDF using John the Ripper and its GUI front-end, Johnny.

**Tools:**
- John the Ripper
- Johnny GUI
- PDF hash extractor

**Steps:**
1. Downloaded and extracted John the Ripper.
2. Installed Johnny GUI and pointed it at `john.exe`.
3. Extracted the PDF's password hash and saved it to `hash.txt`.
4. Loaded the hash into Johnny.
5. Ran a dictionary attack.

**Outcome:** `good-luck`


<summary><b>Lab 2 — Networkwalks Online Tools</b></summary>

**Goal:** Recover the password on a protected PDF using Networkwalks' online hash calculator and password cracker.

**Tools:**
- Networkwalks Hash Calculator
- Networkwalks Password Cracker

**Steps:**
1. Uploaded the PDF to the Hash Calculator and generated its hash.
2. Copied the hash into the Password Cracker.
3. Ran the built-in dictionary attack.

**Outcome:** `password1`


---

## 🖼️ Evidence

<summary><b>Lab 1 — JTR + Johnny screenshots</b></summary>

**Johnny configured**
![Johnny configured](screenshots/johnny-settings.png)

**Hash extracted from PDF**
![Hash extracted from PDF](screenshots/hash-extracted.png)

**Hash loaded into Johnny**
![Hash loaded into Johnny](screenshots/hash-loaded.png)

**Password cracked**
![Password cracked](screenshots/password-cracked.png)

**PDF before unlocking**
![PDF before unlocking](screenshots/locked-pdf.png)

**PDF after unlocking**
![PDF after unlocking](screenshots/unlocked-pdf.png)


<summary><b>Lab 2 — Networkwalks Tools screenshots</b></summary>

**Hash Calculator**
![Hash Calculator](screenshots/hash-calculator.png)

**Password Cracker**
![Password Cracker](screenshots/password-cracker.png)

**Password cracked**
![Password cracked](screenshots/password-cracked1.png)

**PDF before unlocking**
![PDF before unlocking](screenshots/locked-pdf1.png)

**PDF after unlocking**
![PDF after unlocking](screenshots/unlocked-pdf1.png)

---

## 🏁 Flags

| Lab | Flag |
|---|---|
| Lab 1 — JTR + Johnny | nw{cybersecurity_flag_captured_2608} |
| Lab 2 — Networkwalks Tools | nw{networkwalks_flag1_jtr_270521_1} |

---

## 💡 Takeaways

**Hashing vs. Encryption**
Hashing is a one-way transformation — it turns data into a fixed-length value that can't be reversed back to the original. Encryption is two-way: anything encrypted can be decrypted again with the right key. This distinction matters for password storage, since passwords should be hashed, not encrypted.

**Why weak passwords fail**
Both labs cracked their target passwords (`good-luck`, `password1`) using a simple dictionary attack — trying words from a predefined wordlist rather than brute-forcing every combination. Predictable, common, or short passwords fall to this kind of attack almost immediately.

**What good password hygiene looks like**
- [ ] Long, unique passphrases
- [ ] Mixed case, numbers, symbols
- [ ] No reuse across accounts
- [ ] MFA enabled wherever possible
- [ ] Managed via a password manager

---

## 📎 Resources

| Resource | Link |
|---|---|
| John the Ripper | https://www.openwall.com/john/ |
| Johnny GUI | https://openwall.info/wiki/john/johnny |
| Networkwalks | https://networkwalks.com/ |

---

## ⚖️ Disclaimer

This repository documents training exercises performed only against authorized files and systems as part of a supervised cybersecurity internship. Do not attempt password cracking or hash analysis against systems you do not own or have explicit permission to test.
