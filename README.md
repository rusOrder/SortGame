Stack Sorting Game - Unity Implementation
https://screenshot.png (Note: Add actual screenshot later)

Table of Contents
Description

Features

Installation

How to Play

Game Rules

Technical Details

License

Description
Stack Sorting Game is a puzzle game where players need to sort colored chips into homogeneous stacks. The game challenges your logical thinking and problem-solving skills as you work to organize mixed stacks of colored chips into perfectly sorted towers.

Features
Colorful Visuals: Attractive 3D chips with different colors

Adjustable Difficulty: Customize stack height and number of colors

Intuitive Controls: Simple click-and-drag mechanics

Move Counter: Track your progress toward the optimal solution

Win Condition: Automatic detection when all stacks are sorted

Restart Option: Reset the game at any time

Installation
Unity Version: Requires Unity 2020.3 or later

Clone the repository:

bash
git clone https://github.com/yourusername/stack-sorting-game.git
Open in Unity:

Launch Unity Hub

Add the cloned project folder

Open the project

Run the game:

Open the main scene

Click Play in the Unity Editor or build for your target platform

How to Play
Select a chip: Click on the top chip of any stack to pick it up

Move the chip: Click on another stack to place the chip there

Sort all chips: Arrange all chips so each stack contains only one color

Win the game: Complete all stacks to win!

Game Rules
Movement Rules:

Only the top chip of any stack can be moved

You can place a chip only:

On an empty stack, or

On top of another chip of the same color

Stack Completion:

A stack is complete when it's full and contains only one color

Completed stacks are locked and cannot be modified

Winning:

The game is won when all color groups form complete stacks

Technical Details
Architecture
The game follows a clean architecture with these main components:

GameManager: Central controller managing game state

InputManager: Handles player input and chip movement

GameStack: Represents each stack container with its logic

Chip: Individual colored chip objects

Scripts Overview
GameSettings.cs: Configurable game parameters

Chip.cs: Chip behavior and visuals

GameStack.cs: Stack logic and completion detection

InputManager.cs: Player input handling

GameManager.cs: Main game logic and flow

Extensions.cs: Utility methods

Customization
You can easily modify game parameters in the GameSettings:

csharp
[Serializable]
public class GameSettings
{
    public int stackCapacity = 4; // Max chips per stack
    public int colorsCount = 4;   // Number of colors
    public int stacksCount = 6;   // Total stacks (must be > colorsCount)
}
License
This project is licensed under the MIT License - see the LICENSE file for details.

Enjoy the game! For any questions or suggestions, please open an issue in the repository.
