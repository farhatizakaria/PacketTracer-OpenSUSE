# Cisco Packet Tracer Installation Script for openSUSE

This script automates the installation and uninstallation of **Cisco Packet Tracer** on **openSUSE Linux**. The only requirement is that the **Packet Tracer `.deb` installer** file must be located in any directory on `/home` using the default filename.

## Prerequisites ⚙️

1. **openSUSE Linux** (tested on openSUSE Tumbleweed-Slowroll).
2. The **Cisco Packet Tracer `.deb` installer** file should be placed in your **`/home`** directory.

## Installation Steps 🛠️

### 1. Download Cisco Packet Tracer 💻

Download the **Cisco Packet Tracer `.deb` installer** from one of the following sources:

- [NetAcad - Packet Tracer Download](https://www.netacad.com/portal/resources/packet-tracer)
- [Skills For All](https://skillsforall.com/resources/lab-downloads) (login required)

Make sure the `.deb` file is saved to your **`/home`** directory.

### 2. Clone the Script 📂

Clone this repository or download the script directly to your system:

```bash
git clone https://github.com/yourusername/packet-tracer-install-script.git
```

### 3. Run the Script ▶️

Now, you can run the script. This will automatically install Cisco Packet Tracer by:

- Searching for the .deb installer in the /home directory.
- Installing necessary dependencies.
- Extracting and installing Cisco Packet Tracer.

```bash
chmod +x script2.sh
./script2.sh
```
The script will automatically handle everything. It will search for the .deb file, uninstall any existing version of Packet Tracer, install the required dependencies, and set up Cisco Packet Tracer for you.

### 4. Uninstall Cisco Packet Tracer 🧹
If you need to uninstall Cisco Packet Tracer later, simply run the script with the --uninstall flag. This will remove Cisco Packet Tracer and all related files from your system:

```
./script2.sh --uninstall
```

The script will:

- Remove Packet Tracer from /opt/pt.
- Clean up the desktop entries and other configuration files.
- Uninstall the necessary dependencies and restore your system to its previous state.
- No additional configuration is needed. The script handles everything.
