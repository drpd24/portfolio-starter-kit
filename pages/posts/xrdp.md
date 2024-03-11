---
title: A Step-by-Step Guide to Installing XRDP on Ubuntu
date: 2024/3/08
description: Explore the world of remote desktop access on Ubuntu with our concise guide to installing XRDP. This step-by-step tutorial covers prerequisites, installation, service startup, firewall configuration, and connection setup.
tag: dev
author: Davindra Ramadhan
---

# Introduction

XRDP provides a convenient way to access your Ubuntu machine remotely through a graphical user interface. This guide will walk you through the step-by-step process of installing XRDP on an Ubuntu system

### Prerequisites

Before proceeding, ensure you have the following:

An Ubuntu machine (tested on Ubuntu 22.04 LTS).
sudo (administrator) privileges.
Basic knowledge of command line.

## Installation Steps

### Step 1: Update Package Repositories

Open a terminal and update the package repositories to ensure you have the latest information about available packages.

```bash
sudo apt update && sudo apt upgrade -y
```

### Step 2: Install XRDP Package

```bash
sudo apt install xrdp -y
```
### Step 3: Start XRDP Service

After installation, start the XRDP service

```bash
sudo systemctl start xrdp
```

### Step 4: Configure Firewall

If you have the UFW (Uncomplicated Firewall) disabled enter "sudo ufw enable" in the command line, allow traffic on the XRDP port (default is 3389):

```bash
sudo ufw allow 3389/tcp
```

### Step 5: Verify XRDP Installation

Check if XRDP is running and listening on the default port:

```bash
sudo systemctl status xrdp
```

### Step 6: Connect to the Remote Desktop

Open the Remote Desktop Client on your local machine

Enter the IP address or hostname of your Ubuntu machine.

Provide your Ubuntu username and password when prompted.
