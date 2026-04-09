# 🎮 Game Hacking — Cheat Engine Tables

Personal collection of `.CT` cheat tables for various games.  
All scripts use AOB injection or Lua — tested with **Cheat Engine 7.x**.

---

## 📋 Table of Contents

- [Unreal Tournament GOTY (1999)](#unreal-tournament-goty-1999)
- [Streets of Rogue (v98)](#streets-of-rogue-v98)

---

## Unreal Tournament GOTY (1999)

| Feature | Type | Notes |
|---|---|---|
| Infinite HP | AOB Inject | God mode, nullifies incoming damage |
| Infinite Ammo | Lua freeze | Freezes all child ammo entries to 999 |
| One Shot Kill | AOB Inject | Smart filter — skips timers/coords |
| Player Base | Pointer | `Engine.dll+002EAC38` base chain |

**File:** `UnrealTournament.CT`  
**Engine:** 32-bit (x86), `Engine.dll` / `Core.dll` / `Render.DLL`

---

## Streets of Rogue (v98)

| Feature | Type | Notes |
|---|---|---|
| Infinite HP | Lua freeze | Freezes all child HP entries to 999 |
| Infinite Money | AOB Inject | `UnityPlayer.dll` offset |
| Infinite Ammo | AOB Inject | `UnityPlayer.dll` offset |
| 999999 EXP | AOB Inject | Triggers on EXP gain event |
| 99 Potatoes | AOB Inject | Item count override |

**File:** `StreetsOfRogue_v98.CT`  
**Engine:** 64-bit (x64), Unity — `UnityPlayer.dll`

---

<!-- TEMPLATE ДЛЯ НОВОЙ ИГРЫ — скопируй блок ниже
## Название Игры (версия)

| Feature | Type | Notes |
|---|---|---|
| Функция 1 | AOB Inject / Lua freeze / Pointer | Описание |

**File:** `НазваниеФайла.CT`  
**Engine:** 32/64-bit, движок, модули
-->

---

## ⚙️ Requirements

- [Cheat Engine 7.5+](https://www.cheatengine.org/)
- Run CE as **Administrator**
- Attach to game process before enabling entries

## 📌 Notes

- All tables cleaned of personal metadata before publishing
- AOB signatures may break on game updates — re-scan if needed
- Author: **deavers**
