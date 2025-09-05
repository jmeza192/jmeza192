# Jesus Meza — Network Automation Portfolio

I build small, reliable network‑automation tools that turn tedious multi‑step changes into repeatable, auditable runs. This README focuses on what the repos do and the time they save in real workflows.

**Socials**

[![GitHub](https://img.shields.io/badge/GitHub-jmeza192-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/jmeza192)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-jesus%20meza-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jmeza192)

**Projects + Impact**

- **VLAN Changer + CI/CD** (`Vlan-Changer/`)
  - Problem: Moving users/devices required ARP/MAC lookups, CDP walks, and careful config/verification on access ports.
  - What it does: Locates ports by IP/MAC, traverses CDP across trunks/port‑channels, applies access/voice VLANs, verifies, saves, and can roll back. Ships with GitHub Actions for pre/post audits and reports.
  - Results: Instead of having to manually reconfigure 100s of devices per day during a divestiture project, this script allowed me to more quickly reconfigure devices saving me several hours of work everyday
  - Code: https://github.com/jmeza192/Vlan_Changer
  - Tech: Python, Netmiko, GitHub Actions

- **Wiping Config** (inside `wiping-config/`)
  - Problem: Needed to Sanitize 100s of network devices before handing them over.
  - What it does: Removes SNMP/NTP, banners, logging hosts, TACACS servers/keys, specific users, legacy TTY settings, and more with clear progress/error logs. Utilized nornir to allow to program to run on 100 devices at a time
  - Results: Allowed our team to quickly sanitize 100s of network devices saving us days of work in prepping devices to handover
  - Code: https://github.com/jmeza192/wiping-config
  - Tech: Python, Netmiko, Nornir
  - Note: Destructive by design — use intentionally and review scope.

- **Network Toolbox** (`network-toolbox-public/`)
  - Problem: Routine fleet tasks (AP discovery, serial collection, TACACS audits, config cleanup) consumed time and were error‑prone.
  - What it does: A set of targeted scripts with `.env` templates per tool. Batch operations against device lists, robust credential fallback, and clear progress/logging.
  - Results: Cuts repetitive CLI steps to a single command; easier to run at scale and hand off to teammates with templates.
  - Code: https://github.com/jmeza192/network-toolbox-public
  - Tech: Python, Netmiko, Pandas, dotenv

**Tech Stack**

![Cisco](https://img.shields.io/badge/Cisco-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![Juniper](https://img.shields.io/badge/Juniper-84B135?style=for-the-badge&logo=junipernetworks&logoColor=white)
![Aruba](https://img.shields.io/badge/Aruba-ED6F00?style=for-the-badge&logo=aruba&logoColor=white)
![Arista](https://img.shields.io/badge/Arista-003D6B?style=for-the-badge&logo=arista-networks&logoColor=white)
![Palo Alto Networks](https://img.shields.io/badge/Palo%20Alto%20Networks-F37021?style=for-the-badge&logo=paloaltonetworks&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-000000?style=for-the-badge&logo=linux&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![SolarWinds](https://img.shields.io/badge/SolarWinds-F2B01A?style=for-the-badge&logo=solarwinds&logoColor=black)
![Infoblox](https://img.shields.io/badge/Infoblox-1C3F94?style=for-the-badge&logo=infoblox&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Cisco ISE](https://img.shields.io/badge/Cisco%20ISE-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![Aruba ClearPass](https://img.shields.io/badge/Aruba%20ClearPass-ED6F00?style=for-the-badge&logo=aruba&logoColor=white)

**Quick Links**

- `Vlan-Changer/` — local code folder
- `network-toolbox-public/` — local code folder
- `jmeza192.github.io-main/` — site and `resume.pdf`
- Resume (PDF): `jmeza192.github.io-main/resume.pdf`

If you’d like a quick walkthrough or deeper technical detail on any project, feel free to reach out via LinkedIn.
