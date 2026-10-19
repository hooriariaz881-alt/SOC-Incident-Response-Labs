🛡️ SOC & Incident Response Portfolio

This is my hands-on incident investigation portfolio where I will provide my practical labs write-ups, SIEM log analysis, and threat containment.
🧰 Security Tools & Technologies
![Splunk](https://img.shields.io/badge/Splunk-000000?style=for-the-badge&logo=splunk&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-167EC1?style=for-the-badge&logo=wireshark&logoColor=white)
![Sysmon](https://img.shields.io/badge/Sysmon-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

 📂 Hands-On Incident Investigation Labs

 📍 Lab 1: Haxcamp Incident Breakdown (INC-2026-0001)
- Alert: Possible Malware Activity regarding `eicar.com` in workstation `NEX-NYC-LT-001`.
- Log Source: Win Event Log (`Microsoft-Windows-Sysmon/Operational`).
- Investigation Process:
  1. Evaluated the incident graph to determine the compromised host and user (`aisha.khan`).
  2. Queried Splunk logs using SPL to determine the file creation incident.
  3. Identified Sysmon Event ID 11 (File Create), internal application `ValidationRunner.exe` creates `eicar.com` at `C:\ProgramData\NexoraPackages`.
  4. Confirmed Sysmon Event ID 22 (DNS Query) for `validation.nexoratech.com`.

- Conclusion: The alert is considered a false positive as `eicar.com` is a commonly used benign test file to validate the security controls.

<img width="944" height="425" alt="Screenshot 2026-10-12 122504" src="https://github.com/user-attachments/assets/b93e4031-46bc-47a8-b487-aebd6f15f397" />
<img width="608" height="293" alt="Screenshot 2026-10-12 122041" src="https://github.com/user-attachments/assets/dd0f7c63-9565-43c1-97e0-8fb906509c07" />

