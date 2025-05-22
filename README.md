# 🧽 MISTOL - Wiping Linux Logs

**MISTOL** is a simple, Bash script designed to wipe trace evidence from Linux systems. It is useful in offensive security labs, red team simulations, or forensic evasion demonstrations.

This script provides a practical example of:
MITRE ATT&CK T1070.002 — Indicator Removal on Host: Clear Linux or Mac System Logs

🔗 https://attack.mitre.org/techniques/T1070/002/

> ⚠️ **For educational and authorized use only.** Do not use on systems you do not own or have explicit permission to operate on.

## Features

* Wipes system and authentication logs (`auth.log`, `syslog`, `wtmp`, `utmp`, etc.)
* Deletes shell histories (`.bash_history`, `.zsh_history`, etc.)
* Removes cache and temp directories
* Erases application logs (Apache, Nginx, mail, etc.)
* Cleans `.git/logs`, SSH artifacts, and journald/auditd traces
* Supports `--dry-run` mode for safe preview

---

## Usage

```bash
# Launch stealth shell (auto-cleans on exit)
chmod +x ./mistol.sh
sudo  ./mistol.sh --dry-run
```
