# Huuhuu Scanner

A lightweight 802.11 WiFi reconnaissance tool built with Python and Scapy.

Huuhuu Scanner captures wireless beacon frames in monitor mode and displays information about nearby wireless networks in a live terminal interface.

## Features

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
- airmon-ng
- iwconfig

Kali Linux is recommended for the lab environment.

## Installation

```bash
git clone https://github.com/paablo0x/huuhuu-scanner.git
cd huuhuu-scanner
pip install -r requirements.txt
