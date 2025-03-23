# PEASS-ng

---

PEASS-ng Privilege Escalation Scripts

This repository contains privilege escalation enumeration scripts for Linux, macOS, and Windows. The scripts help identify potential vulnerabilities and misconfigurations that could lead to privilege escalation.


---

📂 Directory Structure

linux/ → Contains linPEAS for Linux privilege escalation checks.

macOS/ → Contains linPEAS for macOS to analyze privilege escalation vectors in macOS.

windows/ → Contains winPEAS for Windows privilege escalation enumeration.



---

🔹 Linux (linPEAS)

File: linpeas.sh

Usage:

1. Grant execution permission:

chmod +x linpeas.sh


2. Run the script:

./linpeas.sh


3. If you don’t have execution permissions, use:

bash linpeas.sh



Notes:

Works on any Linux distribution.

Requires bash and standard Linux commands.

If some commands are missing, certain checks may fail.



---

🔹 macOS (linPEAS for macOS)

Files: linpeas_darwin_amd64.bin, linpeas_darwin_arm64.bin

Usage:

1. Grant execution permission:

chmod +x linpeas_darwin_amd64.bin  # For Intel Macs
chmod +x linpeas_darwin_arm64.bin  # For M1/M2 Macs


2. Run the appropriate binary:

./linpeas_darwin_amd64.bin
./linpeas_darwin_arm64.bin



Notes:

macOS may block execution due to security settings.

If you see a warning, go to System Preferences > Security & Privacy and allow the script.

If execution is still blocked, run:

sudo ./linpeas_darwin_amd64.bin

(Requires administrator password if prompted)



---

🔹 Windows (winPEAS)

File: winPEASany.exe

Usage:

1. Open Command Prompt (cmd.exe) or PowerShell.


2. Run the script:

winPEASany.exe



Notes:

Works on Windows 32-bit and 64-bit.

If Windows Defender blocks it, you might need to bypass the security checks.

Running as Administrator provides more detailed results.



---

⚠️ Disclaimer

This repository is intended for educational purposes only. Do not use these tools on unauthorized systems. The author is not responsible for any misuse.


---
