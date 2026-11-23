# The Macromancer

A 2D top-down roguelike where your survival depends on balancing **Protein**, **Carbohydrates**, and **Fats** across procedurally generated dungeons.

## How to Play
1. Go to the **[Releases](https://github.com/cosminageamanu/roguelikeexe/releases)** page and download the latest `.zip` file.
2. Extract the archive to a folder.
3. Run **`Roguelike.exe`** to play.

## Controls

| Action | Key | Notes |
| :--- | :--- | :--- |
| **Move** | `W A S D` or `Arrow Keys` | Speed scales with Carbs & Fats |
| **Basic Attack** | `Space` | Melee slash; damage scales with Protein |
| **Dash** | `Left Shift` | Phases through enemies (invulnerable); costs **3 Carbs** |
| **Cleave** | `Q` | AoE melee strike; costs **2 Protein** |
| **Piercing Beam** | `E` | Long-range spell; costs **5 Fats** |

## Core Mechanics: Macronutrients & Homeostasis
Your stats (`0–100`) drain passively as you explore and fight. Collect food pickups to replenish them and avoid metabolic malfunctions:

* **Homeostasis (`30–70` in all three):** Regenerates **+2 HP** on every metabolic tick.
* **Protein (Melee & Integrity):**
  * `50–80`: +25% melee damage.
  * `< 30`: -40% melee damage and Max HP capped at 70%.
  * `> 85`: Faster metabolic drain.
* **Carbohydrates (Speed & Dash):**
  * `< 30`: -35% movement speed and doubled dash cooldown.
  * `> 85`: -15% movement speed (sugar crash).
* **Fats (Spellcasting & Insulation):**
  * `50–80`: +25% Piercing Beam range.
  * `< 30`: Beam range reduced by 40%, random aim jitter, and 40% faster metabolic drain.
  * `> 85`: -20% movement speed.

## Gameplay Loop
* Explore 5 floors of **BSP-generated dungeons** with A* pathfinding enemies that scale in HP each level.
* Open **chests** to collect passive **Relics** that boost your stats.
* Find the **Key** on each floor to unlock the **Exit**.
* Progress, macros, and relics are automatically saved between floors—use **Continue** from the start screen to resume your run.
