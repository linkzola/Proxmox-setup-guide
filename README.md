# NVIDIA GPU Driver Installation and Verification on Proxmox VE

[![Proxmox](https://img.shields.io/badge/Proxmox-VE-blue)](https://www.proxmox.com/)
[![NVIDIA](https://img.shields.io/badge/NVIDIA-Driver-green)](https://www.nvidia.com/)

---

## Table of Contents
1. [Overview](#overview)
2. [Prerequisites](#prerequisites)
3. [Step 1: Verify GPU Hardware Detection](#step-1-verify-gpu-hardware-detection)
4. [Step 2: Disable the Nouveau Driver](#step-2-disable-the-nouveau-driver)
5. [Step 3: Verify Nouveau is Disabled](#step-3-verify-nouveau-is-disabled)
6. [Step 4: Install NVIDIA Drivers](#step-4-install-nvidia-drivers)
7. [Step 5: Verify Driver Installation](#step-5-verify-driver-installation)
8. [Step 6: Test GPU Functionality](#step-6-test-gpu-functionality)
9. [Step 7: Integrate with Proxmox VE](#step-7-integrate-with-proxmox-ve)
10. [Step 8: Optional – GPU Passthrough for VM](#step-8-optional--gpu-passthrough-for-vm)
11. [Troubleshooting](#troubleshooting)
12. [Validation Checklist](#validation-checklist)
13. [References](#references)

---

## Overview
This guide provides a **step-by-step procedure** to install, configure, and test NVIDIA GPU drivers on **Proxmox VE**.  

It includes:

- Disabling the open-source `nouveau` driver  
- Installing proprietary NVIDIA drivers  
- Verifying GPU functionality  
- Enabling GPU passthrough for VMs  

---

## Prerequisites
Ensure the following before proceeding:

- **Proxmox VE** version ≥ 7.x or 8.x  
- Internet access  
- Root or sudo privileges  
- An NVIDIA GPU  
- Kernel headers installed:

```bash
apt install pve-headers-$(uname -r)
