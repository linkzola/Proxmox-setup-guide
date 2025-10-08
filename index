# 🧠 Proxmox GPU Integration & NVIDIA Driver Setup Guide

Welcome to the **Proxmox GPU Integration Project** — a step-by-step guide to installing and configuring **NVIDIA GPU drivers** for **Proxmox VE** environments, with full support for **GPU passthrough** to virtual machines and containers.

---

## 🚀 Overview

This project provides:

- ✅ Clean and reliable **NVIDIA driver installation** on Proxmox VE  
- ⚙️ Steps to **disable the open-source nouveau driver**  
- 🔍 Methods to **verify GPU detection and functionality**  
- 💻 Guidance for **GPU passthrough setup**  
- 🧩 Troubleshooting tips for common errors  

Whether you’re using your GPU for **machine learning**, **CUDA workloads**, or **virtualized compute**, this guide ensures your Proxmox system runs NVIDIA GPUs efficiently.

---

## 📑 Table of Contents

1. [About the Project](#about-the-project)  
2. [System Requirements](#system-requirements)  
3. [Installation Guide](#installation-guide)  
4. [Verification and Testing](#verification-and-testing)  
5. [GPU Passthrough](#gpu-passthrough)  
6. [Troubleshooting](#troubleshooting)  
7. [References](#references)  
8. [Author](#author)

---

## 🧰 About the Project

**Proxmox VE** is a powerful open-source virtualization platform.  
This guide integrates **NVIDIA GPU support**, allowing high-performance GPU workloads inside virtual machines (VMs) and containers.

You’ll learn to:
- Detect GPU hardware  
- Disable `nouveau` drivers  
- Install proprietary NVIDIA drivers  
- Test driver functionality  
- Configure GPU passthrough  

---

## 🧩 System Requirements

| Requirement | Description |
|--------------|-------------|
| Proxmox VE | Version **7.x** or **8.x** |
| GPU | Any modern **NVIDIA GPU** |
| Access | **Root or sudo** privileges |
| Internet | Required for driver installation |
| Kernel Headers | Installed using: `apt install pve-headers-$(uname -r)` |

---

## ⚙️ Installation Guide

The full installation and setup instructions are available here:  
👉 [**NVIDIA GPU Driver Installation and Verification on Proxmox VE**](./NVIDIA_GPU_Installation.md)

This document includes:
- Disabling nouveau
- Installing NVIDIA DKMS modules
- Rebuilding initramfs and GRUB
- Validating GPU functionality
- Preparing passthrough settings for virtual machines

---

## 🧪 Verification and Testing

Once installed, validate with:

```bash
nvidia-smi
lsmod | grep nvidia
cat /proc/driver/nvidia/version
