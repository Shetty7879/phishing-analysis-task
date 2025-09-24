# 📧 Phishing Email Analysis – Cyber Security Internship Task 2

## 📖 Description
Cyber Security Internship Task 2: Analyzed a phishing email sample to identify spoofed domains, suspicious links, urgent language, and social engineering tactics. Includes sample email, analysis report, and screenshots.

---

## 📧 Sample Phishing Email

From: PayPal Support support@paypa1-security.com

To: user@example.com

Subject: URGENT: Your Account Will Be Suspended!
Date: Mon, 23 Sep 2025 08:32:15 +0000

Dear Customer,

We have detected suspicious activity in your PayPal account.
To avoid suspension, you must verify your account within 24 hours.

Click the link below to confirm your details:
http://secure-paypal-login.verify-account.ru

Failure to act will result in permanent account suspension.

Thank you for your prompt attention.

Sincerely,
PayPal Security Team


---

## 📝 Analysis Report

### 1. Sender Analysis
- Claimed sender: `support@paypa1-security.com`  
- Legitimate PayPal emails come from `@paypal.com`.  
- Attacker used **`paypa1` (number “1” instead of letter “l”)** → Spoofed domain.

---

### 2. Header Analysis
- `From:` shows `support@paypa1-security.com`.  
- `Reply-To:` points to an unrelated address.  
- Sent from a **non-PayPal mail server**.  
- **Discrepancy:** Sender name says “PayPal Support” but domain is fake.

---

### 3. Content Indicators
- **Urgent language:** “Your account will be suspended in 24 hours.”  
- **Fear tactic** to force immediate action.  
- **Generic greeting:** “Dear Customer” instead of real name.  
- **Spelling trick:** `paypa1` instead of `paypal`.

---

### 4. Links & Attachments
- Link text: “verify your account”  
- Real link (hovered): `http://secure-paypal-login.verify-account.ru`  
- Domain `.ru` indicates foreign/untrusted origin.  
- No attachment here, but phishing emails often include malicious files.

---

### 5. Phishing Traits Identified ✅
- Spoofed sender domain  
- Suspicious/mismatched URLs  
- Urgent/threatening language  
- Generic greeting (not personalized)  
- Foreign/untrusted domain  

---

### 6. Conclusion
This email is a **phishing attempt**.  
It relies on **email spoofing**, **mismatched URLs**, and **social engineering (urgency + fear)** to trick users into entering PayPal credentials on a fake website.

---

## 📷 Screenshots

### 1. Email Header Analysis (Detailed View)
![Header Analysis](https://drive.google.com/uc?export=view&id=1Ygh_41oI8pWkn5sBb5RrTSpn_OeWFlx5)

### 2. Header Analyzed Summary
![Header Summary](https://drive.google.com/uc?export=view&id=1bjCa7ak8oxp6SwAlBusNZwNSBG1Eef-A)



---

## 📂 Repository Structure
