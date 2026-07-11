# Network Reconnaissance Scanner

A lightweight, Python-based network reconnaissance tool designed for automated port scanning, banner grabbing, and vulnerability detection. This tool combines standard Python socket programming for fast initial discovery with the power of the Nmap Scripting Engine (NSE) for deep vulnerability analysis.

## Features

* **Custom Port Scanning:** Uses Python's built-in `socket` library to identify open TCP ports within a user-defined range.
* **Banner Grabbing:** Automatically attempts to grab service banners from discovered open ports to identify running services and versions.
* **Automated Vulnerability Scanning:** Integrates with `python-nmap` to run OS fingerprinting, version detection, and Nmap's default vulnerability scripts (`--script=vuln`) against the target.

## Prerequisites

Before running the script, ensure you have the following installed on your system:

1. **Python 3.x**
2. **Nmap:** The core system network mapper must be installed on your host machine.
   * On Linux/Ubuntu: `sudo apt-get install nmap`
   * On Windows: Download from [Nmap.org](https://nmap.org/download.html)
3. **Python-Nmap Library:** The Python wrapper used by the script.
   * `pip install python-nmap`

## Installation

Clone the repository and navigate into the directory:

```bash
git clone [https://github.com/yourusername/network-scanner.git](https://github.com/yourusername/network-scanner.git)
cd network-scanner
