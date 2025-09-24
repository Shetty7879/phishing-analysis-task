# 📧 Phishing Email Analysis – Cyber Security Internship Task 2

## 🔍 Objective
The goal of this task is to analyze a phishing email sample and identify suspicious indicators such as spoofed senders, mismatched URLs, and social engineering tactics.

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
- Legitimate PayPal emails only come from `@paypal.com`.  
- Here, the attacker used **`paypa1` (number “1” instead of letter “l”)** → Spoofed domain.

---

### 2. Header Analysis
- `From:` shows `support@paypa1-security.com`.  
- `Reply-To:` points to an unrelated email address.  
- Email originates from a **non-PayPal server** (detected via header analyzer).  
- **Discrepancy:** Sender name says “PayPal Support” but domain is fake.

---

### 3. Content Indicators
- **Urgent language:** “Your account will be suspended in 24 hours.”  
- **Fear tactic** to force immediate action.  
- **Generic greeting:** “Dear Customer” instead of personalized name.  
- **Spelling trick:** Domain uses “paypa1” instead of “paypal”.  

---

### 4. Links & Attachments
- Link text: “verify your account”  
- Real link (hovered): `http://secure-paypal-login.verify-account.ru`  
  - Domain `.ru` indicates foreign/untrusted origin.  
- No attachments here, but phishing emails often include malicious `.zip` or `.exe` files.

---

### 5. Phishing Traits Identified ✅
- Spoofed sender domain  
- Suspicious/mismatched URLs  
- Urgent and threatening language  
- Generic greeting (not personalized)  
- Foreign/untrusted domain  

---

### 6. Conclusion
This email is a **phishing attempt**.  
It relies on **email spoofing**, **mismatched URLs**, and **social engineering (urgency + fear)** to trick users into entering PayPal credentials on a fake website.

---

## 📂 Repository Structure
