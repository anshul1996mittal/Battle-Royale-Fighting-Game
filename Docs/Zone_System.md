# ⭕ Zone (Safe Area) System Design

---

## 1. 🎯 Overview

Controls the shrinking play area to force player engagement.

---

## 2. 🧩 Core Components

* ZoneManager
* CircleController
* DamageSystem

---

## 3. 🔄 Flow

Match Start → Initial Zone → Timer → Shrink → New Zone → Repeat → Final Zone

---

## 4. 📍 Zone Logic

### Step 1: Initial Zone

* Random center position
* Large radius

### Step 2: Shrink Phases

* Reduce radius over time
* Move center (optional)

### Step 3: Final Zone

* Small area
* High intensity combat

---

## 5. 💥 Damage System

Players outside zone take damage:

Damage = BaseDamage × TimeMultiplier

---

## 6. 🎮 Visual Feedback

* Zone boundary indicator
* Warning UI
* Damage effects

---

## 7. 🌐 Multiplayer Sync

* Server calculates zone
* Clients interpolate movement

---

## 8. ⚡ Optimization

* Update zone in intervals (not every frame)
* Lightweight calculations

---

## 9. 🚀 Advanced Features

* Dynamic zone behavior
* Multiple safe zones
* Environmental hazards
