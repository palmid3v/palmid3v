# PC Specifications

> System specifications captured from **DirectX Diagnostic Tool (DxDiag)** on **September 29, 2026**.

## System

| Property | Value |
|---|---|
| Operating System | Windows 10 Pro 64-bit |
| OS Build | 10.0, Build 19045 |
| Language | English |
| System Manufacturer | ASUS |
| System Model | System Product Name |
| BIOS | 3636 |
| Processor | AMD Ryzen 5 5500 |
| CPU Cores / Threads | 12 logical processors (as reported by DxDiag) |
| CPU Clock | ~3.6 GHz |
| RAM | 32 GB (32768 MB) |
| DirectX Version | DirectX 12 |
| DxDiag Version | 10.00.19041.5794 64-bit Unicode |

## Graphics

### AMD Radeon RX 6600

| Property | Value |
|---|---|
| GPU | AMD Radeon RX 6600 |
| Manufacturer | Advanced Micro Devices, Inc. |
| Chip Type | AMD Radeon Graphics Processor (0x73FF) |
| DAC Type | Internal DAC (400MHz) |
| Device Type | Full Display Device |
| Approx. Total Memory | 24,426 MB |
| Dedicated VRAM | 8,147 MB |
| Shared System Memory | 16,279 MB |
| DirectDraw Acceleration | Enabled |
| Direct3D Acceleration | Enabled |
| AGP Texture Acceleration | Enabled |
| Direct3D DDI | 12 |
| Driver Model | WDDM 2.7 |
| Driver Version | 32.0.21045.5002 |
| Driver Date | August 16, 2026 |
| WHQL Logo'd | Yes |

### Driver

The DxDiag screenshot shows the AMD display driver beginning with:

```text
atidxx64.dll, amdxx64.dll, amdxx...
```

The full driver filename list is truncated in the screenshot and is therefore not recorded here as a complete value.

### DirectX Feature Levels

DxDiag reports support including:

```text
12_1, 12_0, 11_1, 11_0, 10_1, 10_0, 9_3, ...
```

The screenshot truncates the remaining feature-level list.

## Audio Devices

### Headphones — BKD-11 Pro Audio Device

| Property | Value |
|---|---|
| Device Name | Headphones (BKD-11 Pro Audio Device) |
| Hardware ID | USB\VID_31B2&PID_0011&REV_0100&MI_00 |
| Default Device | No |
| Driver | USBAUDIO.sys |
| Driver Version | 10.0.19041.5794 |
| Driver Date | April 6, 2025 |
| WHQL Logo'd | Yes |
| Provider | Microsoft |
| Problems Reported | None |

### Headset — G435 SE Wireless Gaming Headset

| Property | Value |
|---|---|
| Device Name | Headset Earphone (G435 SE Wireless Gaming Headset) |
| Hardware ID | USB\VID_046D&PID_0ACB&REV_0009&MI_00 |
| Default Device | Yes |
| Driver | USBAUDIO.sys |
| Driver Version | 10.0.19041.5794 |
| Driver Date | April 6, 2025 |
| WHQL Logo'd | Yes |
| Provider | Microsoft |
| Problems Reported | None |

## Diagnostic Status

All displayed DxDiag pages report:

```text
No problems found.
```

## Hardware Summary

| Component | Specification |
|---|---|
| CPU | AMD Ryzen 5 5500 |
| RAM | 32 GB |
| GPU | AMD Radeon RX 6600 |
| GPU VRAM | 8 GB dedicated |
| Shared GPU Memory | ~16 GB |
| OS | Windows 10 Pro 64-bit |
| DirectX | DirectX 12 |
| GPU Driver | AMD 32.0.21045.5002 |
| GPU Driver Date | 2026-08-16 |
| Audio | G435 SE Wireless Gaming Headset + BKD-11 Pro Audio Device |

## Notes

- Memory values are reproduced from DxDiag and may include system-reserved/shared memory.
- The **24,426 MB Approx. Total Memory** reported for the GPU should not be interpreted as 24 GB of physical VRAM. The screenshot separately reports approximately **8 GB dedicated VRAM** and **16 GB shared system memory**.
- The Ryzen 5 5500 is reported by DxDiag as having **12 logical processors**.
- Driver and hardware information reflects the state of the system at the time of the DxDiag capture.
- This document is intended to serve as a version-controlled hardware reference for the PC and can be updated whenever major hardware, operating system, or driver changes are made.

---

## Source

Information transcribed from screenshots of **Microsoft DirectX Diagnostic Tool (DxDiag)** supplied for this document.

**Capture date:** 2026-09-29
