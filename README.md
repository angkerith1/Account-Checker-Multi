# Account Checker Tool v1.0

A multi-service account checker tool with colorful terminal output and batch checking support.

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

## Download

### [⬇️ Download Latest Version (t.exe)](../../releases/latest/download/checker.exe)

Or go to [Releases](../../releases) page to download.

## Installation

1. Download `t.exe` from the link above
2. Double-click to run
3. No Python or additional installation required!

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
