---
layout: post
title: How to Ubuntu with Qemu command line.
date: 2024-01-04 11:12:00-0400
description: A simple notes on how to run Ubuntu with Qemu

# Install Ubuntu

Suppose you have followed the steps in https://www.jwillikers.com/virtualize-ubuntu-desktop-on-macos-with-qemu

# Run Ubuntu

```bash 
qemu-system-x86_64 \
    -machine type=q35,accel=hvf \
    -nographic      \
    -cpu Nehalem    \
    -smp 4          \
    -hda ubuntu-20.04.6-desktop-amd64.qcow2 \
    -m 4G \
    -usb \
    -device usb-tablet \
    -net nic    \
    -net user,hostfwd=tcp::8888-:22
```

Following command will ssh into the VM:

```bash
ssh -p 8888 username@localhost
```
---
