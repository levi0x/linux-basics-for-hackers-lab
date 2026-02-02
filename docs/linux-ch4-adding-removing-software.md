# Chapter 4 — Adding and Removing Software (apt)

## Goal
Practice installing, inspecting, and removing software safely in a Kali Linux VM using the `apt` package manager.

## Commands practiced
### Update package lists
```bash

sudo apt update

Search for a package
apt search ufw

View package details (metadata)
apt show ufw

Install a package
sudo apt install ufw

Verify install
ufw --version || ufw status || which ufw

Remove vs purge

remove = uninstall package, typically keeps configuration files

sudo apt remove ufw


purge = uninstall package + remove configuration files

sudo apt purge ufw

Cleanup unused dependencies
sudo apt autoremove

Evidence (screenshots):
See: screenshots/ch4/
ch4-01-apt-update-search-ufw.png
ch4-02-apt-show-ufw.png
ch4-03-install-verify-ufw.png
ch4-04-purge-autoremove.png

Why this matters for cybersecurity
Security tools and updates are commonly installed via package managers.
Keeping systems updated reduces exposure to known vulnerabilities.

Clean install/remove workflows help keep labs reproducible and stable (important for VM-based security testing).
