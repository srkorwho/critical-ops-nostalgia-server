# Cops Custom Server

Basic custom server implementation for Cops. This project uses SQLite for data management and simulates Photon/ENet protocols for gameplay.

## Technical Details

- **High-Performance Multiplayer Sync:** Optimized real-time synchronization for player actions.
- **Runtime State Updates:** Fast 60Hz player position and rotation tracking.
- **Action Packets:** Robust handling for shoot and reload packet broadcasting.
- **Binary Serialization:** Manual Protocol 16 implementation handling complex types (Hashtables, Dictionaries, ObjectArrays) at byte level.
- **Network Stability:** Kernel-level UDP socket reset handling via IOControl to prevent connection resets on Windows.
- **Sync Optimization:** Multi-event packing for efficient initial world state synchronization.
- **Database:** Full skin registration and user data management via SQLite.
- 
<img width="1248" height="649" alt="image" src="https://github.com/user-attachments/assets/421f53a8-8ec9-40da-96ee-3832e4f9ec45" />

## Features

- Automatic guest account creation.
- Case opening system.
- Username change support.
- Room creation and joining.

## Requirements

Recommended to use a decent server if you plan to host for more than 5 players.

## Setup

1. Change the LocalIP in Program.cs to your server IP.
2. Set the AssetFolderPath to your assets directory.
3. Compile and run.
4. The database (referans.db) will be created automatically.

## Skinpack Rates

Tier 1-2: 5% | Tier 3: 20% | Tier 4: 25% | Tier 5: 20% | Tier 6: 15% | Tier 7: 10%
