---
title: "Worklog Week 10"
date: 2026-06-22
weight: 10
chapter: false
pre: "<b>1.10.</b>"
---

# Worklog Week 10

## Week 10 Objectives

- Complete the top-down weapon system with multiple weapon types.
- Add visual effects for attacks, Block, Parry, and projectiles.
- Create debugging tools to visualize and tune hitboxes, block direction, and parry direction.
- Fully test online mechanics in Unity.
- Prepare the initial steps for building the game and deploying the server online on AWS.

## Tasks to be carried out this week

| Day | Work | Start date | End date | Reference |
| --- | --- | --- | --- | --- |
| Monday | Complete the Lobby and Map Lobby flow, design the flow to enter Boss Room, test online/offline player spawn, and prepare the BossRoom_Minotaur scene. | 22/06/2026 | 22/06/2026 | Unity Documentation, Netcode for GameObjects |
| Tuesday | Set up Cinemachine camera for top-down gameplay, configure camera follow for the local player, set up CameraBounds, fix the issue of Player being pushed outside the map, and test camera in offline and online modes. | 23/06/2026 | 23/06/2026 | Unity Cinemachine Documentation |
| Wednesday | Complete gameplay UI system, link Stats to Health, Mana, and Poise UI, test Weapon Pickup in offline and online modes, and fix weapon pickup and incorrect WeaponData synchronization. | 24/06/2026 | 24/06/2026 | Unity Documentation, Project source code |
| Thursday | Optimize NetworkPlayer and PlayerMove, test multiple clients in the same LobbyScene, fix NetworkManager and UnityTransport issues, and test online movement, aiming, weapon switching, and map entering. | 25/06/2026 | 25/06/2026 | Netcode for GameObjects |
| Friday | Complete multiple weapons: Sword, Spear, Bow, and Staff. Set up Spear combo and quick Parry, Bow Rapid Fire and Burst Rapid Fire, Staff homing magic bolt and heal aura, and add skill icons to WeaponData. | 26/06/2026 | 26/06/2026 | Unity Documentation, Project source code |
| Saturday | Design Slash Effect Prefab for weapons, set up Shield Wave, Hold Pulse, Spark effect for Block/Parry success, and add projectile trails for Arrow and Magic Bolt. | 27/06/2026 | 27/06/2026 | Unity Documentation, Project source code |
| Sunday | Create a hitbox debug tool for ActionHitBox, draw preview direction for Block and Parry, tune attack ranges, prepare AWS architecture with EC2, Lambda Function URL, and DynamoDB, and start handling Linux Dedicated Server build and SSH connection to EC2. | 28/06/2026 | 28/06/2026 | AWS Documentation, Unity Dedicated Server Documentation |

## Results Achieved in Week 10

- Completed the top-down weapon system with multiple weapon types: Sword, Spear, Bow, and Staff.
- Sword supports combo, Block, and Parry. Spear supports left-click two-hit combo and right-click quick Parry without hold Block.
- Bow supports Rapid Fire and Burst Rapid Fire. Staff supports homing magic bolt and healing/buff skill.
- Added skill icon support to WeaponData, including primary skill icon, secondary skill icon, primary skill name, and secondary skill name.
- Completed visual feedback for combat, including Slash Effect, Stab Effect, Shield Wave, Hold Pulse, Spark Effect, and projectile trails.
- Created debugging tools to visualize ActionHitBox, Block Direction, Parry Direction, and real attack zones triggered by animation events.
- Online testing in Unity worked well: Host/Client can enter Lobby, online players can move and aim correctly, and weapons work in the online environment.
- Prepared the initial AWS deployment direction using EC2, Lambda Function URL, DynamoDB, Unity Linux Dedicated Server, and SSH connection to EC2.

## References

- AWS Documentation
- Unity Dedicated Server Documentation
- Netcode for GameObjects
- Project source code
