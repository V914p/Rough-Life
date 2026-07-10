---
title: "Worklog Week 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " 1.11. "
---

# Worklog Week 11

## Week 11 Objectives:

- Complete the final development tasks of the RoughLife game project before the reporting phase.
- Fix and synchronize important online gameplay effects such as death particles and player states.
- Complete the revive mechanic for online mode so that players can support each other after being downed.
- Retest offline/online gameplay, boss rooms, combat, weapons, and UI.
- Start applying AWS server deployment to the project, focusing on the dedicated server model and Amazon GameLift.
- Prepare AWS deployment evidence to include in the internship report and project documentation.

## Tasks to be completed this week:

| Day | Task | Start Date | Completion Date | References |
|---|---|---:|---:|---|
| Mon | - Review the entire RoughLife project after completing the main gameplay systems.<br>- Check important systems including Player, Boss, Weapon, UI, Lobby, and Boss Room.<br>- Identify remaining issues before entering the final polishing stage. | 29/06/2026 | 29/06/2026 | Project source code, Unity Documentation |
| Tue | - Complete and synchronize the **death particle** effect in the online environment.<br>- Test the effect when a Player is downed on both Host and Client.<br>- Ensure that the death effect is not only displayed locally but also synchronized correctly for other players.<br>- Fix issues where particles do not appear or appear at the wrong position when the character dies. | 30/06/2026 | 30/06/2026 | Unity Netcode for GameObjects, Project source code |
| Wed | - Complete the **revive** mechanic for online Players.<br>- Implement logic so that a downed Player enters a waiting-for-revive state.<br>- Allow other Players to approach and perform the revive action.<br>- Test health recovery after a successful revive.<br>- Ensure that revive states are synchronized between Host and Client. | 01/07/2026 | 01/07/2026 | Unity Documentation, Netcode for GameObjects |
| Thu | - Test death, revive, and return-to-Lobby mechanics in the Boss Room.<br>- Check the case where all Players are downed.<br>- Fix issues where offline/online Players may get stuck in the Boss Room.<br>- Ensure gameplay remains stable after revive or after the boss fight ends. | 02/07/2026 | 02/07/2026 | Project source code |
| Fri | - Start applying AWS server deployment to the project.<br>- Study the dedicated server model for Unity online games.<br>- Prepare the Unity Linux Dedicated Server Build.<br>- Study Amazon GameLift, Fleet, Anywhere Fleet, Alias, and Game Session Queue.<br>- Decide on a suitable deployment direction based on AWS Free Tier limitations and current quota. | 03/07/2026 | 03/07/2026 | AWS Documentation, Amazon GameLift Documentation, Unity Dedicated Server Documentation |
| Sat | - Test AWS configuration steps for the game server.<br>- Prepare evidence related to GameLift, Fleet/Alias/Queue, or alternative approaches when quota is limited.<br>- Check the connection between the Unity Client and the server build.<br>- Record issues that occur during AWS server setup. | 04/07/2026 | 04/07/2026 | AWS Console, Amazon GameLift Documentation |
| Sun | - Perform an overall test of the project after completing death particles, revive, and the initial AWS server setup.<br>- Collect all evidence screenshots that have been prepared.<br>- Note the sections that need to be added to the report, including gameplay, online co-op, revive, server architecture, and AWS deployment. | 05/07/2026 | 05/07/2026 | Project source code, AWS Console |

## Week 11 Results:

- Completed additional final features of the RoughLife project before the reporting phase.
- Synchronized the **death particle** effect in the online environment, making downed Player states clearer between Host and Client.
- Completed the **revive** mechanic for online Players, allowing players to support each other during boss fights.
- Tested and fixed issues related to death state, revival, returning to Lobby, and handling the case where all Players are downed.
- Improved the stability of offline/online gameplay, especially in Boss Room, combat, weapon, and UI systems.
- Started applying AWS server deployment to the project using the dedicated server approach.
- Studied and tested AWS components related to Amazon GameLift, Fleet, Anywhere Fleet, Alias, and Game Session Queue.
- Prepared initial evidence for the game server deployment on AWS.
- Identified important limitations when deploying GameLift, especially quota and AWS Free Tier scope.

## References:

- https://cloudjourney.awsstudygroup.com
- https://unity.com
- AWS Documentation
- Amazon GameLift Documentation
- Unity Netcode for GameObjects Documentation
