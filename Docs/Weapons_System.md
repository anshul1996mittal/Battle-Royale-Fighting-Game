# 🔫 Weapon System Design

---

## 1. 🎯 Overview

Handles all weapon-related logic including firing, damage, and upgrades.

---

## 2. Weapon Types

* Guns (AR, SMG, Sniper)
* Melee (Knife, Bat)
* Throwable (Grenade, Smoke)

---

## 3. Architecture

WeaponBase (Abstract)
├── GunWeapon
├── MeleeWeapon
├── ThrowableWeapon

---

## 4. Flow

Input → WeaponController → Fire()
→ Hit Detection → Damage System

---

## 5. Weapon Data

Uses ScriptableObjects:

* Damage
* Fire rate
* Range
* Ammo

---

## 6. Features

* Recoil system
* Reload system
* Attachments (scope, mag)

---

## 7. Optimization

* Object pooling (bullets)
* Raycast for instant weapons
