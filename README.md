# Microsoft Office 2024: Install, Update, Repair, And Activation Troubleshooting

This gist is a practical checklist for installing [Microsoft Office 2024](https://softwarelegit.com/product/microsoft-office-2024-pro-plus/), fixing common setup problems, running a clean repair, and resolving the most common activation issues without using risky tools.

---

## 1) Before Installing: Quick Checks That Prevent Most Issues

**Do these first. They save time.**

- Restart Windows
- Install pending Windows updates
- Confirm enough free disk space (aim for 10 GB or more)
- Sign in with the Microsoft account that owns the license
- Temporarily pause third party antivirus if it blocks installers (turn it back on after)

If Office was installed before, remove old versions to avoid conflicts.

---

## 2) Uninstall Old Office Cleanly

### Option A: Normal uninstall
Settings → Apps → Installed apps → Microsoft 365 / Office → Uninstall

Restart after uninstall.

### Option B: If uninstall fails
Use Microsoft Support and Recovery Assistant (SaRA).  
Search: **Microsoft SaRA Office uninstall tool**  
Run the Office uninstall option, then restart.

---

## 3) Install Microsoft Office 2024

### If you have a subscription style license
Install from the Microsoft account portal or Microsoft 365 installer page used for the purchase.

### If you have a one time purchase
Download using the official source tied to your product key or account.

**Tip:** Avoid random “offline installers” from unknown sites. They are the #1 reason for broken installs and activation loops.

---

## 4) Fix “Office Can’t Install” Or Install Stops

### Common causes
- Old Office leftovers
- Corrupted Windows system files
- Installer blocked by proxy, VPN, DNS filters
- Disk or permission issues

### Step 1: Repair Windows system files
Open Command Prompt as Administrator:

```cmd
DISM /Online /Cleanup-Image /RestoreHealth
sfc /scannow
