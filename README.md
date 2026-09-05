# Reverse-Engineering-Journey

> A public log of my reverse-engineering practice — from game hacking to low-level binary analysis. Every experiment is documented with the same write-up format so progress is verifiable, not claimed.

## What this is

I'm a CS student at VŠB-TUO (FEI) focusing on cybersecurity and digital forensics. This repository is where I practice the craft: taking binaries apart, understanding what they do, and writing it down so others (and future me) can reproduce it.

## Write-up format

Every solved task follows a fixed five-part template:

1. **Given** — file type, alphabet of content, magic bytes
2. **Hypothesis** — what I think the protection/encoding is before touching tools
3. **Tool** — Ghidra / gdb+pwndbg / CyberChef / binwalk / exiftool / steghide
4. **Command & observation** — exact steps, key output
5. **Conclusion** — what it actually was, what I learned

## Repository layout

```
Course_Solutions/    write-ups of course/training tasks
Crackmes_and_CTF/    crackmes and CTF challenges (picoCTF & co.)
Game_Hacking/        local, offline experiments with process memory of old games
Tools_and_Scripts/   helpers written along the way (Python/Bash)
```

## Toolbox

`Ghidra` · `gdb / pwndbg` · `CyberChef` · `binwalk` · `exiftool` · `steghide` · `zbar` — on EndeavourOS (KDE/Wayland) and Windows 11

## Progress log

| Date | Task | Category | Key technique |
|---|---|---|---|
| 2026 | _Hidden Cipher 1_ (picoCTF) | RE / packing | UPX unpack + XOR key extraction |
| 2026 | _Binary Digits_ (picoCTF) | Forensics | binary → bytes → JPEG (JFIF signature) |
| 2026 | _Gatekeeper_ (picoCTF) | RE | hex-gate validation, deobfuscation |

## Ground rules

- All experiments are local and offline (own binaries, CTF targets, old offline games)
- No live services, no third-party servers, no anti-cheat bypassing
- Write-ups teach the method, not just the answer
