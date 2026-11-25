# Money Heist: The Bank Escape

## Team Members & Responsibilities

| Member | Primary Responsibility |
|---|---|
| Isabella Soriano | Core Gameplay & Integration |
| Jason Ventura | Level Design & Environment |
| Jaeli Tilley | Obstacles & Animation |
| Marvee | UI, Menus & Testing |

Responsibilities may be adjusted as development progresses.

Video Demo #1 : https://github.com/JAVENT12/3D-Runner/issues/1

## Game Overview

The player controls a robber attempting to escape a bank while avoiding police officers and security lasers. The objective is to survive as long as possible and earn points by traveling through the bank and collecting cash.

The game focuses on a continuous gameplay loop, randomized hallways, increasing difficulty and a bank-themed environment.

## Planned Gameplay Features

- **Movement:** Automatic forward movement with three-lane switching.
- **Jumping:** Avoid low obstacles using a basic jump mechanic.
- **Randomized hallways:** Straight, left-turn and right-turn hallway prefabs generate continuously, with at least two straight hallways between turns.
- **Safe starting area:** The first two hallways contain no obstacles or cash, giving the player time to prepare. Turning hallways also remain clear.
- **Obstacles:** Stationary and moving hazards with collision detection.
- **Increasing difficulty:** Running speed gradually increases and eligible straight hallways can spawn up to two obstacles.
- **Scoring:** Distance-based score tracking.
- **Camera:** Third-person camera that follows the player.
- **Game States:** Main menu, active gameplay and game-over screen with restart functionality.

## Planned Controls

| Input | Action |
|---|---|
| Left Arrow | Move left |
| Right Arrow | Move right |
| Space | Jump |

## Technical Requirements

- **Two lighting types:** Directional lighting and point lights in the bank environment.
- **Camera movement:** Third-person following camera that rotates with hallway turns.
- **Character or obstacle animation:** Script-based robber and police limb animations, plus floating and rotating cash.
- **Moving obstacles:** Patrolling police, approaching police and security lasers
- **Functional menus:** Main menu, options, live score display and game-over screen.


## Development Tools

- **Game Engine:** Unity
- **Programming Language:** C#
- **Version Control:** Git / GitHub
- **Target Platform:** PC

  
## Main Scripts
| Script  | Purpose| 
|---|---|
| PlayerController.cs  | Forward movement, lane switching, jumping, turning and speed progression.| 
|CameraController.cs |  Follows the player and rotates during turns.  |
|GroundSpawner.cs  |  Generates and removes hallway tiles.  |
|HallwayTile.cs  |  Stores the connection point for the next hallway.  |
|TileExit.cs  |  Triggers additional hallway generation.  |
|TurnTrigger.cs  |  Detects approaching turns.  |
|ObstacleSpawner.cs  |  Randomly generates police and lasers.|
|Obstacle.cs  |  Detects player collisions and triggers game over.  |
|PoliceMovement.cs  |  Controls approaching police and laser detection. |
|PolicePatrol.cs  |  Moves police between lanes. |
|RobberAnimation.cs  |  Animates the robber's running motion. |
|PoliceAnimation.cs  |  Animates police movement.  |
|CashSpawner.cs  |  Randomly generates cash bundles.  |
|CashCollectible.cs  |  Animates cash and awards points on collection. |
|GameManager.cs  |  Manages scoring, game-over state, best score and restarting. |
|MainMenu.cs  |  Manages menu navigation, volume and scene loading.  |


## Development Approach

The project builds on an existing Unity prototype. Development will focus on integrating the team's contributions, implementing the required gameplay systems and maintaining a stable, playable build.

Additional features will be considered only after the core mechanics and project requirements are functional.


## Future Improvements
- Creating a more immersive experience.
- Add more bank environments and obstacle variations.
- Add sound effects and background music if not already configured.

