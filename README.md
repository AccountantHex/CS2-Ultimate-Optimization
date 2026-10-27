# CS2 Ultimate Optimizer

Console-based optimization tool for **Counter-Strike 2**, built with a modular engine architecture.

This project is designed for **competitive players**, **benchmarking**, and **low-latency system tuning**, while keeping all tweaks **reversible and safe**.

---

## 🔧 Features

### Optimization Modes
- **SAFE Mode**
  - Daily-use optimizations
  - Low latency without aggressive system changes

- **PERFORMANCE Mode**
  - Higher priority scheduling
  - GPU-specific optimizations
  - Reduced background interference

- **BENCHMARK Mode**
  - Maximum performance configuration
  - Intended for short test sessions only
  - Revert recommended after use

---

### Engine Architecture
- Frontend: `CS2_Optimizer.bat`
- Backend: modular scripts inside `/scripts`
- All system tweaks are isolated and reversible

---

### Hardware Detection
- Automatic detection of:
  - GPU vendor (NVIDIA / AMD / Intel)
  - CPU core count
  - Installed RAM
- Applies GPU-specific optimizations when supported

---

### FPS Benchmark (IMPORTANT)

FPS benchmark **requires CS2 console output**.

The optimizer automatically launches CS2 with:

-condebug

⚠️ **You MUST enable the CS2 developer console in-game:**

Settings → Game → Enable Developer Console (~) → ON


During the benchmark:
1. Join a match or play offline
2. Play for **at least 30–60 seconds**
3. **Close CS2 completely**
4. The optimizer will automatically parse FPS data

❗ No manual console commands are required, but the console **must be enabled**.


---

### Timer Resolution
- Uses `SetTimerResolution.exe` if available
- Safe fallback via Windows Multimedia scheduling
- Activated automatically during CS2 launch / benchmark

---

### Revert System
- Full revert option
- Restores:
  - Network stack
  - Power plan
  - GameDVR settings
  - GPU overrides
- Designed as a safe “panic button”

---

## 📁 Project Structure

CS2-ULTIMATE-OPTIMIZATION/
├── CS2_Optimizer.bat
├── config.txt
├── console.log
├── /scripts
│ ├── detect_hardware.bat
│ ├── windows_fps_latency_optimizer.bat
│ ├── timer_resolution_launcher.bat
│ ├── nvidia_optimizer.bat
│ ├── amd_optimizer.bat
│ ├── fps_parser.bat
│ ├── revert_optimizer.bat
│ └── install_all.bat
├── /logs
├── README.md
└── CHANGELOG.md


---

## ▶️ Usage

1. Run `CS2_Optimizer.bat` **as Administrator**
2. Set CS2 executable path (first run only)
3. Choose optimization mode or benchmark
4. Use **Revert** option when needed

---

## ⚠️ Disclaimer

- Use at your own risk
- Benchmark mode should not be used for daily play
- Always revert if unexpected behavior occurs

---

## 📜 License

[MIT License](https://badgen.net/github/license/Precision-Optimize/CS2-Ultimate-Optimization)
