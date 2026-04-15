# 🎮 Game Hacking — Cheat Engine Tables

Personal collection of `.CT` cheat tables for various games.  
All scripts use AOB injection or Lua — tested with **Cheat Engine 7.x**.

---

## 📋 Table of Contents

- [Unreal Tournament GOTY (1999)](#unreal-tournament-goty-1999)
- [Streets of Rogue (v98)](#streets-of-rogue-v98)
- [Plants vs. Zombies GOTY](#plants-vs-zombies-goty)
- [The Binding of Isaac: Repentance+](#the-binding-of-isaac-repentance)

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

## Plants vs. Zombies GOTY

| Feature | Type | Notes |
| :--- | :--- | :--- |
| Infinite Sun | AOB Inject | Forces sun count to 999 |
| Instant Recharge | AOB Inject | Skips seed packet cooldowns |
| Immortal Plants | AOB Inject | Nullifies zombie damage to plants |
| One Hit Kill | AOB Inject | Instakills Normal and Conehead zombies |
| Infinite Money | AOB Inject | Sets Crazy Dave's shop coins to 999,990 |
| Speed Controller | Lua Script | Custom UI dropdown for game speedhack |

**File:** `PlantsVsZombies.CT`  
**Engine:** 32-bit (x86), PopCap Framework (`popcapgame1.exe`)

---

## The Binding of Isaac: Repentance+

| Feature | Type | Notes |
| :--- | :--- | :--- |
| Infinite Resources | AOB Inject | Locks Money, Bombs, and Keys to 99 |
| Infinite Health | AOB Inject | Locks Red and Armor Hearts to maximum |
| Inf Item Charges | AOB Inject | Active item bypasses recharge cycle |
| Stats AOB Lock | AOB Inject | Overrides room-transition resets for DMG, Speed, and Tears |
| Player Structure | Data Structure | Fully mapped `Entity_Player` float offsets |

**File:** `IsaacRepentance.CT`  
**Engine:** 32-bit (x86), Custom Engine (`isaac-ng.exe`)

---

## ⚙️ Requirements

- [Cheat Engine 7.5+](https://www.cheatengine.org/)
- Run CE as **Administrator**
- Attach to game process before enabling entries

## 📌 Notes

- All tables cleaned of personal metadata before publishing
- AOB signatures may break on game updates — re-scan if needed
- Author: **deavers**
