---
title: A Step-by-Step Guide to Installing XRDP on Ubuntu
date: 2024/3/08
description: Explore the world of remote desktop access on Ubuntu with our concise guide to installing XRDP. This step-by-step tutorial covers prerequisites, installation, service startup, firewall configuration, and connection setup.
tag: dev
author: Davindra Ramadhan
---

# Introduction

XRDP (X Remote Desktop Protocol) provides a convenient way to access your Ubuntu machine remotely through a graphical user interface. This guide will walk you through the step-by-step process of installing XRDP on an Ubuntu system

### Prerequisites

Before proceeding, ensure you have the following:

An Ubuntu machine (tested on Ubuntu 22.04 LTS).
sudo (administrator) privileges.
Basic knowledge of command line.

## Installation Steps

### Step 1: Update Package Repositories

Open a terminal and update the package repositories to ensure you have the latest information about available packages.

```js
sudo apt update && sudo apt upgrade -y
```
