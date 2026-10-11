# Huuhuu Scanner

<<<<<<< HEAD
A lightweight 802.11 WiFi reconnaissance tool built with Python and Scapy.

Huuhuu Scanner captures wireless beacon frames in monitor mode and displays information about nearby wireless networks in a live terminal interface.
=======
## Understanding Wi-Fi Signal Strength (RSSI)

RSSI (Received Signal Strength Indicator) estimates the strength of a received Wi-Fi signal. It is commonly expressed in dBm, where values closer to zero generally indicate a stronger signal.
>>>>>>> 313d475 (docs: explain Wi-Fi RSSI signal strength)

| RSSI (dBm) | General interpretation |
|------------|-------------------------|
| -30 to -50 | Very strong |
| -51 to -60 | Strong |
| -61 to -70 | Moderate |
| -71 to -80 | Weak |
| Below -80 | Very weak |

<<<<<<< HEAD
- Real-time 802.11 WiFi scanning
- SSID and BSSID discovery
- RSSI / signal-strength analysis
- Basic wireless security classification
- Channel detection
- 2.4 GHz / 5 GHz band identification
- Passive client observation
- Channel hopping
- Interactive terminal interface
- Filtering by security type
- BSSID targeting
- Monitor-mode setup and cleanup

## Requirements

- Linux
- Python 3
- Scapy
- Wireless adapter supporting monitor mode
- `airmon-ng`
- `iwconfig`

Kali Linux is recommended for the lab environment.

## Installation

```bash
git clone https://github.com/paablo0x/huuhuu-scanner.git
cd huuhuu-scanner
pip install -r requirements.txt
Usage
sudo python3 huuhuu_scanner.py -i wlan0
Command-Line Options
-i, --interface    Wireless interface
--open             Show open networks
--weak             Show weak/broken/open networks
--target           Focus on a specific BSSID
How It Works

Huuhuu Scanner uses Scapy to inspect 802.11 beacon frames while a wireless interface is operating in monitor mode.

The scanner extracts:

SSID
BSSID
Channel
Signal strength
Security information

It also observes wireless traffic and performs channel hopping to discover wireless networks.

Controls
CTRL+A    Return to the menu
1         Pause / resume
CTRL+C    Exit and restore WiFi
Limitations
Requires a wireless adapter capable of monitor mode
Signal strength depends on hardware and environment
Passive client observation is not guaranteed to detect every device
Current channel hopping focuses on 2.4 GHz channels
Tested primarily on Linux-based systems
Disclaimer

This project was created for educational and security research purposes.

Use it only in environments where you have permission to perform wireless security testing.

Author

Pablo

GitHub: https://github.com/paablo0x
=======
These ranges are approximate. Actual signal quality depends on interference, obstacles, antenna characteristics, and the receiving device.

### Why RSSI Matters

RSSI helps compare nearby access points and understand Wi-Fi coverage. A stronger signal does not necessarily mean a faster connection, and RSSI alone cannot determine whether a network is secure.

>>>>>>> 313d475 (docs: explain Wi-Fi RSSI signal strength)
