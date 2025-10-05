# Freeze Monster and Space Invaders

## Overview

This project contains two Java-based games: Freeze Monster and Space Invaders. Each game has its own logic and uses the Factory Method design pattern to create instances of objects [...]

## Project Structure

- **`BadnessBoxSprite.java`**: Container for `BadSprite` objects, allowing multiple bad sprites to be grouped.
- **`BadSprite.java`**: Abstract class representing a generic bad sprite with basic behaviors and properties.
- **`FreezeBeam.java`**: Implements a specific type of `BadSprite` that represents a freezing ray.
- **`Slime.java`**: Implements a specific type of `BadSprite` that represents slime.
- **`Woody.java`**: Extends the `Player` class to represent the player character Woody.
- **`FreezeMonsterBoard.java`**: Manages the game logic of "Freeze Monster".
- **`Bomb.java`**: Implements a specific type of `BadSprite` that represents a bomb.
- **`BomberSprite.java`**: Extends `BadnessBoxSprite` to represent a bomber sprite.
- **`Shot.java`**: Implements a specific type of `BadSprite` that represents a shot fired by the player.
- **`SpaceInvadersBoard.java`**: Manages the game logic of "Space Invaders".
- **`Player.java`**: Represents a generic player character.
- **`MainFrame.java`**: Configures the game's main window.
- **`Sprite.java`**: Base class for all sprites.
- **`Commons.java`**: Interface that defines constants used throughout the project.
- **`FreezeMonsterGame.java`**: Main class that initializes the "Freeze Monster" game.
- **`SpaceInvadersGame.java`**: Main class that initializes the "Space Invaders" game.
- **`AbstractBoard.java`**: Abstract class that defines the basic structure of a game board.

## Factory Method Pattern

The Factory Method pattern is used to create instances of game objects without specifying the exact class of the object to be created, promoting flexibility and code reuse.

### Main Classes

- **`AbstractBoard`**: Defines abstract methods `createPlayers` and `createPlayer`.
- **`FreezeMonsterBoard`**: Implements `createPlayer` to create an instance of `Woody`.
- **`MainFrame`**: Defines the abstract method `createBoard`.
- **`FreezeMonsterGame`**: Implements `createBoard` to create an instance of `FreezeMonsterBoard`.
- **`SpaceInvadersGame`**: Implements `createBoard` to create an instance of `SpaceInvadersBoard`.

## Games

### Freeze Monster

In the Freeze Monster game, the player controls the character Woody to navigate the board, avoiding or interacting with various sprites such as freezing rays, slimes, and bombs.

#### How to Run

1. Clone the repository to your local machine.
2. Open the project in IntelliJ IDEA.
3. Make sure all dependencies are resolved.
4. Run the `FreezeMonsterGame` class to start the Freeze Monster game.

#### Controls

- **Arrow Keys**: Move Woody up, down, left, or right.

### Space Invaders

In the Space Invaders game, the player controls a cannon to shoot at space invaders descending down the board.

#### How to Run

1. Clone the repository to your local machine.
2. Open the project in IntelliJ IDEA.
3. Make sure all dependencies are resolved.
4. Run the `SpaceInvadersGame` class to start the Space Invaders game.

#### Controls

- **Arrow Keys**: Move the cannon left or right.
- **Spacebar**: Fires shots.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
