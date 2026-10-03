# oracle-recovery-tools
Read-only Oracle recovery tool. Repair corrupted Oracle database files and damaged backup files, supports Oracle 10g–23c.
# Oracle Recovery Tool

A read-only Oracle recovery utility for corrupted database files and damaged backup files.

## Overview

Oracle Recovery Tool performs offline, read-only analysis on Oracle database files and backup files. It parses corrupted data file structures directly, extracts usable table data from broken DBF files, and salvages records from damaged backup exports without writing any changes to your source evidence.

All scanning operations run in **read-only mode** — your original database files and backup files remain untouched.

## Supported Versions

- Oracle 7~10g
- Oracle 11g
- Oracle 12c
- Oracle 18c
- Oracle 19c
- Oracle 21c
- Oracle 23c
- Oracle 26AI
## Core Capabilities

- Repair and recover data from corrupted Oracle data files (`.dbf`, `.ora`)
- Recover data from damaged Oracle export backup files (`.dmp`, exp / expdp format)
- Extract table data from broken, unmountable or inconsistent database files
- Preview recoverable table data before export
- **100% read-only scan**: source files will never be modified

## Use Cases

- Oracle database file corruption
- Damaged or broken export backup files (exp/expdp .dmp)
- Database file cannot be mounted or opened
- Data rescue from corrupted DBF files
- Recovery from damaged DMP backup files

## How It Works

1. The tool scans the corrupted Oracle data file or backup file in read-only mode.
2. It parses internal database block structures directly.
3. Recoverable tables and records are identified and extracted.
4. Recoverable data is displayed in a preview view.
5. Verified data can be exported after preview.

## Important Notice

This is an offline forensic analysis tool.

We do **not** write or modify the original database files or backup files during scanning. Always work on copies of your source files for evidence safety.

## Download

Get the latest Windows binary release on GitHub Releases.

> Pre-built Windows x64 zip package, contains the read-only Oracle recovery client.

## Antivirus Note

> ⚠️ The Windows binary is protected with VMProtect for anti-tampering. Some antivirus software may incorrectly flag it as malware (false positive). This tool works in fully read-only mode and will not modify your database source files.

## Contact

For technical feedback, bug reports or feature requests, please open a GitHub issue.
