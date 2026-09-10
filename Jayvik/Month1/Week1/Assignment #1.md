# **Assignment \#1 \- Basic Cybersecurity Risk Assessment**

SCENARIO: BrightLayer Stores (simulated, 8 employees) uses: employee email accounts, shared computers, a company website, cloud storage with invoices, user passwords, and a public Wi-Fi router.

SUBMISSION TEMPLATE (use exactly this structure):
1. FIVE IMPORTANT ASSETS - list each asset and why it matters to the business.
2. THREE POTENTIAL THREATS - for each: who/what is the threat actor or event?
3. THREE VULNERABILITIES - for each: what is the exact weakness?
4. ASSOCIATED RISKS - link each threat+vulnerability pair to a potential loss (impact).
5. SECURITY RECOMMENDATIONS - at least 5 improvements, each mapped to a risk above.

RULES: Use the standard asset -> threat -> vulnerability -> risk -> recommendation flow. 400-700 words. Think like a junior analyst preparing their first risk memo.

## **1\. FIVE IMPORTANT ASSETS**

**1\. Employee Email Accounts** – Email is used for business communication and may contain sensitive information, customer details, invoices, and login/reset links. Compromised email accounts could allow attackers to access other business systems.

**2\.** **Cloud Storage with Invoices** – The cloud storage contains financial and business records such as invoices. Loss, theft, or unauthorized modification of these files could cause financial and operational problems.

**3\. Company Website** – The website represents BrightLayer Stores publicly and may be important for communicating with customers and generating business. Website compromise could damage the company's reputation or interrupt services.

**4\. Shared Computers** – Employees use shared computers to perform daily business activities. These systems may contain locally stored business information, browser sessions, and access to company accounts.

**5\. User Passwords and Credentials** – Passwords protect employee accounts and access to company resources. If credentials are stolen or reused, an attacker could gain unauthorized access to multiple systems.

## **2\. THREE POTENTIAL THREATS**

**1\. Phishing/Credential Theft** –A cybercriminal could send employees a fraudulent email containing a malicious link or fake login page to steal their credentials.

**2\.** **Malware/Ransomware** – A malicious program could infect a shared computer through a downloaded file, malicious attachment, or compromised website. It could steal, encrypt, or destroy business data.

**3\. Unauthorized Access to the Public Wi-Fi** – An attacker near the business could attempt to access the public Wi-Fi network and use weak security settings to gain unauthorized network access or intercept poorly protected traffic.

## **3\. THREE VULNERABILITIES**

**1\. Weak or Reused Passwords** – Employees may use simple or reused passwords across different accounts, making credential attacks more effective.

**2\.** **Insufficient Endpoint Protection** – Shared computers may not have adequate antivirus/endpoint protection, regular patching, or restricted user privileges, increasing the chance that malware can execute successfully.

**3\. Poorly Secured Wi-Fi Network** – The public Wi-Fi router may use weak security settings, an easily guessed administrator password, or may not properly separate guest/public users from business devices.

## **4\. ASSOCIATED RISKS**

**1\. Phishing \+ Weak/Reused Passwords** – Stolen credentials could allow an attacker to access employee email and cloud storage, resulting in data theft, invoice exposure, account compromise, and financial loss.

**2\.** **Malware/Ransomware \+ Insufficient Endpoint Protection** – Malware could infect shared computers and potentially encrypt or destroy business files, causing business disruption, data loss, recovery costs, and reputational damage.

**3\. Wi-Fi Attack \+ Poorly Secured Wi-Fi Network** – Unauthorized network access could expose business systems or allow attackers to intercept network traffic, potentially resulting in credential theft, unauthorized access, and compromise of company information.

## **5\. SECURITY RECOMMENDATIONS**

**1\. Enable Multi-Factor Authentication (MFA)** for email, cloud storage, and other important accounts to reduce the impact of stolen passwords.  
*Mapped risk: Phishing \+ weak/reused passwords.*

**2\.** **Implement a strong password policy** and encourage employees to use unique passwords with a reputable password manager.  
*Mapped risk: Credential theft and account compromise.*

**3\. Install and maintain endpoint protection** on all shared computers and enable automatic security updates and regular patching.  
*Mapped risk: Malware/ransomware.*

**4\. Provide basic phishing-awareness training** so employees can identify suspicious emails, links, attachments, and fake login pages.  
*Mapped risk: Phishing and credential theft.*

**5\. Secure and segment the Wi-Fi network** by using strong WPA2/WPA3 security, changing the default router administrator password, and keeping guest/public Wi-Fi separated from business devices.  
*Mapped risk: Unauthorized Wi-Fi access.*

**6\. Maintain regular backups of important business data and invoices** and ensure backups cannot be easily modified or deleted by a compromised account.  
*Mapped risk: Ransomware and data loss.*

**7\. Use least-privilege access** so employees only have access to the files and systems required for their jobs.  
*Mapped risk: Unauthorized access and data exposure.*

