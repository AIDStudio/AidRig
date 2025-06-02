AIDRig

AIDRig is a high-performance, custom-optimized XMRig fork built specifically for Android devices and Linux SBCs. Designed to take full advantage of big.LITTLE CPU architectures, it features advanced CPU core affinity handling, efficient thread scheduling, and significant power-performance optimizations.

⚙️ Features

Native fork of XMRig, tuned for Android and SBCs

Prioritizes big CPU cores (4–7 on octa-core)

Fine-tuned scheduler and thread affinity

Lower power usage and temperature

Up to 3x faster hash rate on Android (vs stock XMRig)

Optimized for RandomX algorithm (GhostRider supported, but not optimized)


💻 Supported Platforms

✅ Android (ARM64 via Termux)

✅ Linux x86_64

✅ Linux ARMHF (e.g. Raspberry Pi)

✅ Linux AARCH64 (e.g. Orange Pi 5, Rock 5B)

⏳ Windows (planned)


📦 Precompiled Binaries

Download the latest aidrig builds here:

👉 GitHub Releases

📲 Quick Start (Android via Termux)

```
pkg install unrar
unrar x android.rar
cd android
chmod +x aidrig
./aidrig -a rx -o stratum+ssl://rx.unmineable.com:443 -u XMR:YOUR_WALLET.YOUR_WORKER -p x -k -t2 --cpu-affinity 4-7
```

> NOTE: You may need to install missing shared libraries via pkg install libuv.



🧠 About the Algorithm

AIDRig is optimized for RandomX only. Other algorithms like GhostRider are functional but not fine-tuned.

📌 License

AIDRig is based on XMRig (GPLv3). Due to significant independent development, some internal logic is not currently shared as open-source, but GPL compliance is under evaluation.

📣 Feedback & Contributions

This is a dev/test build! Feedback is highly appreciated. Let us know:

Your platform and device

Hashrate and pool stats

Stability and performance





Thanks for trying AIDRig! 🔥
