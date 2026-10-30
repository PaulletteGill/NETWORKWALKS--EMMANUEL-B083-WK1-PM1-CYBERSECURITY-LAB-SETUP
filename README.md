# NETWORKWALKS--EMMANUEL-B083-WK1-PM1-CYBERSECURITY-LAB-SETUP
# WK1-PM1: Cybersecurity Lab Setup (VirtualBox + Kali Linux)

## Objective
Set up a cybersecurity testing lab on my laptop with the following requirements:

- VirtualBox as the base (latest recommended version)
- Kali Linux as the attacking machine
- NAT Network on subnet `10.0.0.0/24`
- Clipboard and drag-and-drop enabled (Bidirectional)
- Shared folder: host `Downloads` folder shared with the VM
- Kali IP address: `10.0.0.2/24`
- Full internet access from Kali

## Environment

| Item | Value |
|---|---|
| Host OS | Windows 11 |
| Hypervisor | Oracle VirtualBox |
| Guest OS | Kali Linux 2026.3 (pre-built VirtualBox image, amd64) |
| VM RAM / CPUs | 2048 MB / 2 |
| Virtual disk | 80.09 GB (.vdi) |
| NAT Network name | `NATNetwork` (`10.0.0.0/24`, DHCP enabled) |
| Kali static IP | `10.0.0.2/24` |
| Gateway | `10.0.0.1` |
| DNS | `8.8.8.8` |


# Step 1: Install VirtualBox and 7-Zip
# Step 2: Switch VirtualBox to Expert Mode
# Step 3: Create the NAT Network (10.0.0.0/24)
# Step 4: Download and extract the Kali VM image

> **Issue encountered:** My first attempt imported the VM before extraction, so the disk showed as **"Normal, Inaccessible"** with a yellow warning triangle. The `.vdi` was still inside the compressed archive. After extracting, I removed the VM (**Remove Only**) and re-added it.


# Step 5: Import the VM into VirtualBox
# Step 6: Configure VM network (Settings → Network)
# Step 7: Enable clipboard and drag-and-drop
# Step 8: Configure the shared folder
# Step 9: Start Kali and log in
# Step 10: Set the static IP to 10.0.0.2/24
# Step 11: Verify the configuration


## Conclusion
The lab is complete. Kali Linux runs in VirtualBox on a custom NAT Network (`10.0.0.0/24`) with a static IP of `10.0.0.2/24`, working internet access, shared clipboard and drag-and-drop, and a shared Downloads folder. A snapshot was taken as a clean restore point for future labs.
