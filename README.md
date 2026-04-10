# 🛡️ HZT Guardian Monitor V1.0

**HZT Guardian Monitor** is a high-performance, real-time server monitoring tool designed specifically for Windows-based file servers. It provides a sleek, modern widget interface to keep track of system health while ensuring data security through an active defense system.

## 🚀 Key Features

- **Live System Metrics:** Smoothly animated monitoring for CPU, RAM, and GPU usage.
- **Multi-Storage Visualizer:** Automatic detection and health monitoring (Pie Chart) for all connected SSDs and HDDs.
- **Network Traffic Tracker:** Real-time upload and download speed monitoring.
- **Active Defense Security:** - **MAC Whitelisting:** Only authorized devices can access protected directories.
    - **Auto-Sever System:** Automatically terminates unauthorized SMB sessions attempting to access sensitive folders.
    - **Protected Paths:** Custom folder protection for payroll, database, and internal files.
- **Modern UI/UX:** - Frameless, rounded-corner design.
    - Draggable and "Always on Top" widget mode.
    - Informative, color-coded security logs.

## 🛠️ Built With

- **Language:** Python 3.14
- **Framework:** PySide6 (Qt for Python)
- **Libraries:** psutil, GPUtil

## 📥 Installation

1. Go to the [Releases](https://github.com/hizpro/HZT-Guardian-Monitor/releases) page.
2. Download the `hzt_guardian.exe`.
3. Run the application as **Administrator** (Required for network management features).

## 🔒 Security Configuration

On the first run, the application will generate a `whitelist.json` file. Add your authorized MAC addresses to this file to grant access to protected zones.

```json
{
  "approved": ["00:15:5D:01:20:AF", "AA:BB:CC:DD:EE:FF"]
}
