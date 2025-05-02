# System Status Reporter

A Python script that prints a clear and structured terminal dashboard with key information about the current status of a Linux system. It uses the `psutil`, `subprocess`, `socket`, and `rich` libraries to display live system metrics such as memory usage, disk space, network interfaces, and core systemd services.

## Features

The script displays the following system information:

- Hostname, current date and time, uptime, and kernel version
- Disk usage for the top 3 most utilized mount points
- RAM and swap memory statistics
- Network interface names and their assigned IP addresses
- List of currently logged-in users
- Status of selected systemd services

The output is presented in a readable, color-formatted layout using the `rich` library.

## Requirements

- Python 3.7 or newer
- Python packages:
  - `psutil`
  - `rich`
  - `socket` and `subprocess` are builtin in python already


## Installation
```bash
git clone <repository_url>
cd <directory>
```

You can install the required packages with:

```bash
pip install -r requirements.txt
```

Better way to install following requirements is to create new virtual environment
Inside directory where you cloned this project:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Usage
If you choose to install required modules into system python:

```bash
chmod +x 99-custom-python
./99-custom-python
```

If you are using virtual environment:

```bash
source <directoroy>/.venv/bin/activate
python3 99-custom-python
```

## Use Cases

This script is useful for:
	•	Quickly assessing system health after logging in via SSH
	•	Performing routine checks on system resource usage
	•	Generating a terminal-based system summary for administrators or developers
    •	Creating a colorful, informative MOTD (message of the day)

