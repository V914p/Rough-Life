---
title: "Worklog Week 9"
date: 2026-06-15
weight: 9
chapter: false
pre: "<b>1.9.</b>"
---

# Worklog Week 9

## Week 9 Objectives

- Complete the top-down gameplay foundation for the 2D co-op boss fight game project.
- Convert older systems from platformer to top-down, especially movement, aim, combat, and weapon systems.
- Build the Minotaur boss system with multiple states, multiple skills, and interaction with knockback, block, and parry systems.
- Perform initial multiplayer testing using Unity Netcode for GameObjects.

## Tasks to be carried out this week

| Day | Work | Start date | End date | Reference |
| --- | --- | --- | --- | --- |
| Monday | Analyze the current Unity project again, define the direction for converting the game from platformer to top-down co-op boss fight, set up top-down player movement, and configure owner-based player control in the online environment. | 15/06/2026 | 15/06/2026 | Unity Documentation, Netcode for GameObjects |
| Tuesday | Build the Minotaur boss foundation. Design the boss state machine including Move, ChooseSkill, Attack, and Stun, and add boss data such as phase, movement speed, cooldown, and damage multiplier. | 16/06/2026 | 16/06/2026 | Unity Documentation, Project source code |
| Wednesday | Integrate the Core combat system for Boss and Player. Connect Stats, Health, Poise, DamageReceiver, and KnockBackReceiver, test Boss knockback on Player, and handle stun behavior when Poise reaches 0. | 17/06/2026 | 17/06/2026 | Project source code |
| Thursday | Convert the Weapon system from platformer to top-down. Design one main weapon with two skills: left mouse and right mouse. Set up Sword with normal attack, Block, and Parry, and fix Block/Parry direction according to top-down aim. | 18/06/2026 | 18/06/2026 | Unity Documentation, Project source code |
| Friday | Debug Block and Parry mechanics. Fix null reference issues related to TopDownAim, DamageReceiver, and KnockBackReceiver, test Block/Parry window using animation events, and ensure Player is not continuously knocked back. | 19/06/2026 | 19/06/2026 | Project source code |
| Saturday | Complete initial test weapons such as Sword, Bow, and Staff. Test left mouse and right mouse input and tune animation events for AttackAction, EnterAttackPhase, and AnimationFinished. | 20/06/2026 | 20/06/2026 | Unity Documentation, Project source code |
| Sunday | Perform combined testing for offline gameplay and local online gameplay. Check Player movement, aim direction, animation sync, and combat interactions, and record issues for the following week. | 21/06/2026 | 21/06/2026 | Netcode for GameObjects, Project source code |

## Results Achieved in Week 9

- Completed the foundation of Player top-down movement, including four-direction Rigidbody2D movement and mouse aiming.
- Synchronized movement direction and aim direction in the online environment, and ensured only the owner can control their own player.
- Built the Minotaur boss state machine with Move, ChooseSkill, Attack, Stun, and phase transition.
- Implemented a two-phase Minotaur boss with skills such as Melee Attack, AOE Attack, Range Attack, Dash Attack, and Defend.
- Integrated Boss with the Core combat system, including Health, Poise, DamageReceiver, KnockBackReceiver, ParryReceiver, and Death handling.
- Converted the Weapon system to top-down with left mouse main skill and right mouse secondary skill.

## References

- Unity Documentation
- Netcode for GameObjects
- Project source code
