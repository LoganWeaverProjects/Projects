# Password Cracking & Authentication Security Analysis
**Tools:** `Johnny (John the Ripper)` | `Ophcrack` | `CrackStation` | `Kali Linux`

### Objective
To evaluate the security of various password storage methods (Linux shadow files and Windows SAM files) and demonstrate the speed at which weak or moderately complex hashes can be compromised using automated tools.

### Key Skills
* **Hash Cracking:** Extracting and cracking Linux `/etc/shadow` and Windows `SAM` files.
* **Security Policy Analysis:** Evaluating password strength against **NIST Special Publication 800-63B** standards.
* **Tool Proficiency:** Using rainbow tables (Ophcrack) and dictionary-based attacks (John the Ripper).
* **Vulnerability Assessment:** Identifying the risks of password reuse and the limitations of "leetspeak" complexity.

### Project Summary
In this project, I utilized a Kali Linux environment to practice cracking different types of password files. I successfully cracked simple passwords (e.g., "airforce", "redbox") in **under five minutes** using Johnny and compromised moderately complex passwords in **under one minute** using Ophcrack.

A major focus of this analysis was the transition from traditional complexity requirements to **length-based passphrases**. I documented how modern cracking tools easily bypass common substitutions (like `3` for `e`) and advocated for the implementation of NIST-compliant policies, such as a **15-character minimum length** and breached-password checks.

---

### Technical Highlights
* **Linux Shadow Analysis:** Demonstrated how Linux restricts sensitive password information to administrative users via `sudo` access.
* **Cross-Platform Cracking:** Compared local tool results with cloud-based hash databases (CrackStation) to verify the accessibility of cracking resources to potential attackers.
* **Policy Recommendations:** Developed a set of improvements for organizational password policies, including the removal of unnecessary forced resets in favor of unique, long passphrases.
