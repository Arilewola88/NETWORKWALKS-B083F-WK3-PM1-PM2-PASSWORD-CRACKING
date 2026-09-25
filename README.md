# NETWORKWALKS-B083F-WK3-PM1-PM2-PASSWORD-CRACKING

A hands-on internship project covering password recovery of a protected PDF file using two approaches: **John the Ripper (JTR)** software, and the **Networkwalks Hash Calculator & Password Cracker** 
![Skill](https://img.shields.io/badge/Skill-Cybersecurity-red)
![John the Ripper](https://img.shields.io/badge/John%20the%20Ripper-JTR-blue)
![Networkwalks](https://img.shields.io/badge/Networkwalks-Tools-informational)
![Skill](https://img.shields.io/badge/Skill-Password%20Cracking-red)
![Skill](https://img.shields.io/badge/Skill-Hash%20Extraction-red)
![Ethical Hacking](https://img.shields.io/badge/Ethical%20Hacking-orange)
![Author](https://img.shields.io/badge/Author-Arilewola%20Abdulrokeeb-red)
---

## 📌 About This Project

This project documents two practical exercises completed during Week 3 of my Cybersecurity internship at Networkwalks: cracking the password of a protected PDF file using two different methods:

1. **John the Ripper (JTR)** — run using the JTR software
2. **Networkwalks Hash Calculator & Password Cracker** — free browser-based tools

Both methods target the same locked PDF supplied for the lab, and both successfully recovered the password and captured the same flag.

---

## ⚖️ Liability Disclaimer

All password-cracking activity in this project was carried out only against a PDF file explicitly supplied by Networkwalks for training purposes, within my own personal lab environment. This is for educational purposes only — nothing here should be used against any system, file or account you do not own or do not have explicit written permission to test. Misuse can lead to criminal charges, heavy fines, and a permanent record. In most countries unauthorised access is a crime even when nothing is damaged.

---

## 🛠️ Tools Used

- **John the Ripper (JTR)** — password cracking software
- **Networkwalks Hash Calculator** — extracts a crackable hash from a protected PDF
- **Networkwalks Password Cracker** — runs a dictionary attack against the extracted hash

## 🖥️ Lab Environment

| Component | Details |
|---|---|
| Host machine | Windows 11, HP laptop |
| JTR software | John the Ripper (with hash loaded via the JTR interface) |
| Browser tools | Networkwalks Hash Calculator & Password Cracker |
| Target file | `My Locked PDF1.pdf` (supplied by Networkwalks) |

## 🧩 Method 1 — John the Ripper + Johnny GUI

**Target file:** `My Locked PDF1.pdf`

**Steps:**
1. I download John the Ripper (jumbo build) and Johnny GUI
2. Extracted the PDF's password hash
3. Loaded the hash into the John the Ripper software and ran the attack
4. John the Ripper recovered the password

Johnny loaded,ready to attack:
<img width="1918" height="1072" alt="johnny loaded" src="https://github.com/user-attachments/assets/40f3117c-8d0c-48dd-893a-3e32c9b8ab77" />


**Result:** password `password1`
<img width="1917" height="1078" alt="password recovered" src="https://github.com/user-attachments/assets/c0c1e616-766c-443e-b571-cdfd998efb12" />


**Flag captured:** nw{networkwalks_flag1_jtr_270521_1}
<img width="1907" height="1031" alt="flag captured" src="https://github.com/user-attachments/assets/1c8d0dda-cbec-42c9-9269-8a99b1fd602a" />



---

## 🧩 Method 2 — Networkwalks Hash Calculator & Password Cracker

**Target file:** `My Locked PDF1.pdf`
**Environment:** Browser, no installation required

**Steps:**
1. I uploaded the PDF to the Networkwalks Hash Calculator to extract a crackable hash
2. Pasted the extracted hash into the separate Networkwalks Password Cracker tool
3. The tool successfully cracked the password on the first attempt

Hash extracted | Hash loaded into cracker:
<img width="1917" height="1078" alt="hash extracted" src="https://github.com/user-attachments/assets/f3b1bea8-709b-4be6-a673-4fded549cff9" />

**Result:**
<img width="1916" height="1075" alt="crack success" src="https://github.com/user-attachments/assets/78a3a657-7545-441f-8440-59577f6a17a3" />
`password `password1

**Flag captured:**
<img width="933" height="1030" alt="image" src="https://github.com/user-attachments/assets/3dfc4a0b-947a-43f9-b408-3a25ff9803e9" />
nw{networkwalks_flag1_jtr_270521_1}


---

---

## 📊 Results

| Method | Target File | Tool | Password Found | Flag |
|---|---|---|---|---|
| 1 — John the Ripper | `My Locked PDF1.pdf` | John the Ripper | `password1` | `nw{networkwalks_flag1_jtr_270521_1}` |
| 2 — Networkwalks Tools | `My Locked PDF1.pdf` | Hash Calculator + Password Cracker | `password1` | `nw{networkwalks_flag1_jtr_270521_1}` |

Both methods successfully recovered the same password and captured the same flag, confirming the weak password used on the target PDF.

---

## ⚖️ Comparing the Two Approaches

| Criteria | Method 1: John the Ripper | Method 2: Networkwalks Tools |
|---|---|---|
| Setup effort | Requires downloading and setting up the JTR software | Low — nothing to install, fully browser-based |
| Speed to result | Fast once the hash is loaded | Fast, worked on the first attempt |
| Skill required | Basic familiarity with the JTR software | None — fully guided UI |
| Transparency of process | High — you see every step of the attack yourself | Medium — hash extraction and cracking are separate guided steps |
| Best for | Learning how password cracking actually works under the hood | Quick checks with no installation needed |

**Takeaway:** John the Ripper gives more direct, hands-on understanding of how a password hash is attacked. The Networkwalks tools make the same result achievable without any setup, which is useful for quick verification.

---

## 🎓 Key Learning Outcomes

- Learned how a password hash is extracted from a protected PDF, and that it's the hash — not the file itself — that a cracking tool attacks
- Understood how a dictionary-based attack works, and why the strength of a password directly determines how fast it can be cracked
- Got hands-on experience with both a dedicated cracking tool (John the Ripper) and a browser-based tool (Networkwalks Hash Calculator & Password Cracker) achieving the same result
- Reinforced why weak, common passwords like `password1` are cracked almost instantly, which is the core lesson this lab is designed to teach

---

##  Ethical and Legal Scope

All password-cracking activity in this project was performed only against a PDF file explicitly supplied by Networkwalks for training purposes, within my own personal lab environment.

- No real, production, or third-party systems, accounts, or files were targeted
- All tools were used strictly for educational, authorised lab work
- This repository is intended as a learning record, not a how-to guide for unauthorised access
- Password cracking against any system, file, or account you do not own or do not have explicit written authorisation to test is illegal in most jurisdictions and a violation of ethical hacking principles

---

## 👤 Author

**Arilewola Abdulrokeeb**
Cybersecurity Intern — Networkwalks Academy (Batch B083F)
LinkedIn: [Arilewola Abdulrokeeb](https://www.linkedin.com/in/abdulrokeeb-arilewola-363bbb20a)

---

**Program:** Cybersecurity at Networkwalks | **Week:** 03 | **Project:** Password Cracking | **Repository:** GitHub

-End-
