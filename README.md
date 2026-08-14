# :car: RaceAR - AR Racing Game

An augmented reality racing game built in Unity, demonstrating how to create compelling AR racing experiences. Originally built using AR Foundation to showcase AR Meshing LiDAR, the project has evolved to support both **Lightship ARDK** and **AR Foundation**. It provides different scenes for each technology, allowing developers to explore and compare AR implementations.

## 🌟 Key Features
- **Dual AR Support**: Fully functional scenes utilizing Lightship ARDK (Niantic) and AR Foundation (Unity).
- **Advanced Car Physics & Controls**: Includes a custom-built physics-based `CarController` simulating wheel colliders, torque, steering, and braking.
- **Mission System**: A dynamic, ScriptableObject-based mission manager that makes creating new objectives and challenges seamless.
- **AR Placement & Interaction**: Logic for detecting planes and seamlessly placing your AR vehicles into the real world.
- **Standalone Testing**: A standalone scene dedicated to tuning and testing car physics without the need to deploy to an AR-capable device.

## 🎮 Demos
| | |
|---|---|
|<img src="https://github.com/dilmerv/ARRacingGame/blob/master/docs/images/demo_1.gif" width="300">|<img src="https://github.com/dilmerv/ARRacingGame/blob/master/docs/images/demo_2.gif" width="300">|
|<img src="https://github.com/dilmerv/ARRacingGame/blob/master/docs/images/demo_3.gif" width="300">|<img src="https://github.com/dilmerv/ARRacingGame/blob/master/docs/images/demo_4.gif" width="300">|

## 📁 Scenes Included
1. **`MainGameAR_ARDK.unity`** - Niantic Lightship ARDK AR Racing Game demo scene.
2. **`MainGameAR_AR_Foundation.unity`** - AR Foundation AR Racing Game demo scene.
3. **`MainGameAR_Standalone.unity`** - Standalone scene designed for rapid testing of car physics and controls outside of AR.

## 🛠 Project Structure Overview
- **`Assets/Scripts/`**: Core gameplay logic.
  - `CarController.cs` / `CarWheel.cs`: Vehicle physics and movement behavior.
  - `PlayerControls.cs` / `PlayerInputController.cs`: Handles touch and keyboard/gamepad inputs.
  - `PlayerMissionManager.cs` / `GameManager.cs`: Orchestrates game state and mission progression.
  - `ARPlacementReticle.cs`: Handles the UI reticle for placing objects in AR space.
- **`Assets/Scriptables/Missions/`**: Contains the ScriptableObjects that define in-game missions. 


## ⚙️ Getting Started
1. Clone this repository to your local machine.
2. Open the project in Unity (ensure you have the appropriate AR build support modules installed).
3. If testing AR features, build and deploy to a compatible iOS or Android device.
4. For quick iteration, open `MainGameAR_Standalone.unity` and press Play in the Editor!
