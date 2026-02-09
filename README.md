# Account Checker Tool v1.0

A multi-service account checker tool with colorful terminal output and batch checking support.

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Platform](https://img.shields.io/badge/Platform-Windows-green)
![License](https://img.shields.io/badge/License-Free-brightgreen)

## Features

- **Multi-Service Support**: Check accounts across multiple VPN services
  - Novi AI
  - SYMLEX VPN
  - ZenVPN

- **Check Modes**:
  - Single account check
  - Batch check from file (multi-threaded)
  - Multi-service batch check

- **Output Options**:
  - Save valid accounts in `email:pass` format
  - Save with full subscription details
  - Colorful terminal output

- **Auto Dependency Checker**: Automatically checks and installs required packages

## Installation

### Option 1: Run as Python Script

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/account-checker.git
cd account-checker
```

2. Install requirements:
```bash
pip install requests
```

3. Run the script:
```bash
python t.py
```

### Option 2: Run as Executable (.exe)

1. Download `t.exe` from [Releases](../../releases)
2. Double-click to run

## Usage

### Main Menu
```
======================================================================
                    ACCOUNT CHECKER TOOL v1.0
               Developer: @RITH
                  Multi-Service Account Checker
======================================================================

============================================================
MAIN MENU
============================================================
1. Single Account Check
2. Batch Check from File
3. Multi-Service Batch Check
4. View Saved Results
5. Settings
0. Exit
============================================================
```

### Account Format
Use `email:password` format:
```
user@example.com:password123
another@email.com:mypassword
```

### Batch Check
1. Create a text file with accounts (one per line in `email:pass` format)
2. Select "Batch Check from File" from menu
3. Enter the filename
4. Results will be saved to `accounts/` or `results/` folder

## Output Folders

| Folder | Description |
|--------|-------------|
| `accounts/` | Valid accounts in `email:pass` format |
| `results/` | Valid accounts with full details |
| `checker_results/` | General check results |

## Building from Source

### Requirements
- Python 3.10+
- PyInstaller

### Build Command
```bash
pip install pyinstaller requests
pyinstaller --onefile --console --hidden-import=requests --hidden-import=urllib3 --hidden-import=charset_normalizer --hidden-import=certifi --hidden-import=idna t.py
```

The executable will be created in the `dist/` folder.

## Settings

- **Timeout**: Connection timeout (default: 30 seconds)
- **Thread Count**: Number of threads for batch checking (default: 10, max: 50)
- **Colors**: Enable/disable colored output

## Screenshots

```
[Novi AI] Checking: user@example.com
============================================================
NOVI AI CHECK RESULT
============================================================
Account: user@example.com
Status: VALID
────────────────────────────────────────
Member Id: 12345
Name: John
============================================================
```

## Disclaimer

This tool is for educational purposes only. Use responsibly and only check accounts you own or have permission to check.

## Developer

**@RITH**

## License

This project is free to use.

---

⭐ Star this repo if you find it useful!
