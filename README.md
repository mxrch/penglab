# Penglab
Abuse of Google Colab for fun and profit. 🐬
https://colab.research.google.com/github/mxrch/penglab/blob/master/penglab.ipynb

**Penglab** is a ready-to-install setup on Google Colab for cracking passwords with an incredible power. *(See benchmarks below.)*
It installs by default :
* Hashcat
* John
* Hydra
* SSH (with ngrok).

You only need a Google Account to use Google Colab, and to use ngrok for SSH.

## How to use it ?
1. Go on : https://colab.research.google.com/github/mxrch/penglab/blob/master/penglab.ipynb
2. Select "**Runtime**", "**Change runtime type**", and set "**Hardware accelerator**" to **GPU**.
3. Change the config by setting "**True**" at tools you want to install.
4. Select "**Runtime**" and "**Run all**" !

## What is Google Colab ?
Google Colab is a free cloud service, based on Jupyter Notebooks for machine-learning education and research. It provides a runtime fully configured for deep learning and free-of-charge access to a robust GPU.

## Benchmarks

#### Hashcat Benchmark :
```CUDA API (CUDA 10.1)
====================
* Device #1: Tesla P100-PCIE-16GB, 16017/16280 MB, 56MCU

OpenCL API (OpenCL 1.2 CUDA 10.1.152) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: Tesla P100-PCIE-16GB, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Minimum password length supported by kernel: 0
Maximum password length supported by kernel: 55

Hashmode: 0 - MD5

Speed.#1.........: 27008.0 MH/s (69.17ms) @ Accel:64 Loops:512 Thr:1024 Vec:8

Minimum password length supported by kernel: 0
Maximum password length supported by kernel: 55

Hashmode: 100 - SHA1

Speed.#1.........:  9590.3 MH/s (48.61ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

Minimum password length supported by kernel: 0
Maximum password length supported by kernel: 55
```

#### Speedtest :

```Retrieving speedtest.net configuration...
Testing from Google Cloud (35.203.136.151)...
Retrieving speedtest.net server list...
Selecting best server based on ping...
Hosted by KamaTera INC (Santa Clara, CA) [11.95 km]: 28.346 ms
Testing download speed................................................................................
Download: 2196.68 Mbit/s
Testing upload speed......................................................................................................
Upload: 3.87 Mbit/s
```
