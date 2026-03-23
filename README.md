# lotst.github.io
**Living Off The Security Tools (LOTST)**

---

## ⚠️ Warning

This project highlights a potential attack technique that is not yet widely used by adversaries. The goal is to raise awareness before attackers weaponize it.

---

## 🔹 Concept of LOTST

Security tools such as IDS (Intrusion Detection Systems), endpoint agents, and monitoring dashboards are designed to protect organizations. These agents are legitimate, signed, and distributed by trusted vendors. They are not malware by themselves.

However, attackers can exploit the trust model in a subtle way:

- **Social engineering scenario**:  
  A victim is told, *“I will install an IDS agent to monitor your organization. By downloading this agent, I will report incidents and attacks to you.”*

- **Reality**:  
  The agent is legitimate, but the attacker registers their own account in the vendor’s infrastructure (e.g., a monitoring dashboard). Once the victim connects their systems to the attacker’s account, the attacker gains visibility and control through the trusted platform.

- **Abuse potential**:  
  - The attacker can use the dashboard to launch attacks against the victim’s environment.  
  - Sensitive data such as passwords can be stolen while remaining undetected.  
  - The attacker can still report valid attacks from other hackers to appear legitimate, while hiding their own malicious activity.  
  - Over time, the victim believes the attacker is a helpful “blue teamer” monitoring their organization, when in fact they are the threat.
  - Example **Bitdefender Total Security** cannot flag **Bitdefender GravityZone Agent** Because those tools are provided by Bitdefender, So that will evade antiviruses 100%

---

## 🔹 Why This Matters

- **Legitimate tools abused**: The agent is not malware, but trust in the vendor infrastructure is exploited.  
- **Long-term stealth**: Attackers can remain undetected for years by blending in with normal monitoring activity.  
- **False sense of security**: Victims may believe they are protected, while in reality they are being surveilled and compromised.  

---

## 🔹 Purpose of This Repository

- Document the risks of LOTST.  
- Provide examples and case studies to help defenders recognize potential abuse.  
- Encourage proactive detection and hardening before attackers adopt this technique.  

---

## 🔹 Forensics Trap

- Forensics analysts will just use the vendor dashboard and go to recent events and they see nothing, Than they say that hack is fake but it is real, The attacker are abusing the security monitoring security software itself

## 🔹 Example Tools to abuse
[Bitdefender Gravity Zone](/lotst.github.io/bitdefender-gravity-zone.html)

## ✅ Takeaway

**LOTST is a warning, not a weapon.**  
By understanding how attackers could exploit trusted security tools and vendor infrastructures, organizations can prepare defenses and avoid being blindsided by techniques that leverage the very systems meant to protect them.
