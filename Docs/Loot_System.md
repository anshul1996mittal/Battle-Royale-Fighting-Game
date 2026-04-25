# 🎁 Loot System Design

---

## 1. 🎯 Overview

Handles spawning, distribution, and rarity of items across the map.

---

## 2. 📦 Loot Types

* Weapons
* Ammo
* Health Items (Medkits, Boosts)
* Armor
* Attachments

---

## 3. 🎨 Rarity System

* Common
* Rare
* Epic
* Legendary

Each rarity affects:

* Spawn chance
* Item strength

---

## 4. 🧩 Architecture

LootManager
├── SpawnController
├── LootTable
├── PickupHandler

---

## 5. 🔄 Flow

Spawn Points → Random Selection → Spawn Item → Player Pickup → Inventory

---

## 6. 🎲 Spawn Logic

* Weighted random system
* Zone-based spawning (high-risk = better loot)

---

## 7. 📍 Spawn Types

* Static (fixed locations)
* Dynamic (randomized per match)

---

## 8. ⚙️ Optimization

* Object pooling for loot objects
* Disable distant loot rendering

---

## 9. 🔐 Multiplayer Sync

* Server controls loot spawn
* Clients receive synchronized state

---

## 10. 🚀 Future Scope

* Airdrops (high-value loot)
* Event-based loot
* Dynamic loot balancing
