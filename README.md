# Tic-Tac-Toe Game

A desktop Tic-Tac-Toe game for two local players, built with Java Swing. The interface pairs a 3 x 3 game board with player score displays and simple controls for starting a new match, resetting a round, or exiting.

## Overview

Players take turns placing X and O on the board. The game checks each move for a winning line or a draw, then announces the result in a dialog. Scores are tracked separately for each player while the application is open.

The window uses a bright blue background, a large title banner, a 3 x 3 grid on the left, and score and game controls on the right.

## Features

- Two-player, turn-based gameplay on one device
- Win detection for all rows, columns, and diagonals
- Draw detection when all nine squares are occupied
- X and O win counters for the current application session
- **New Game** clears the board and both player scores
- **Reset** clears the current board and starts the next round with X, while preserving scores
- **Exit** asks for confirmation before closing the application
- Centered Java Swing window with Nimbus look and feel when available

## Requirements

- Java Development Kit (JDK) 25 or later
- Apache NetBeans with Java and Maven support
- Apache Maven

The project uses the `AbsoluteLayout` dependency stored in the repository's `lib/` directory and configured through `pom.xml`.

## Build and Run

### Apache NetBeans

1. Open Apache NetBeans and choose **File > Open Project**.
2. Select the project folder containing `pom.xml` and allow Maven to load the project and its dependencies.
3. In the Projects panel, open `src/main/java/com/mycompany/game/TicTacToe.java`.
4. Right-click `TicTacToe.java` and choose **Run File** to launch the game.

### Command Line

From the project root, build the application with Maven:

```bash
mvn clean package
```

Launch the desktop game with Maven, specifying its main class:

```bash
mvn exec:java -Dexec.mainClass=com.mycompany.game.TicTacToe
```

The application starts in a desktop window. A graphical desktop environment is required; this is not a web or command-line game.

## How to Play

1. Player X takes the first turn.
2. Click an empty square to place the current player's mark.
3. Players alternate turns. The first player to make a line of three matching marks horizontally, vertically, or diagonally wins.
4. If the board fills without a winning line, the round ends in a draw.
5. Choose **Reset** to clear the board and keep the scores, or **New Game** to clear both the board and scores.

## Project Structure

```text
.
├── .gitignore
├── LICENSE
├── lib/
│   └── unknown/
│       └── binary/
│           └── AbsoluteLayout/
│               └── SNAPSHOT/
│                   └── AbsoluteLayout-SNAPSHOT.jar
├── pom.xml
├── src/
│   └── main/
│       └── java/
│           └── com/
│               └── mycompany/
│                   └── game/
│                       ├── TicTacToe.form
│                       └── TicTacToe.java
└── README.md
```

| Path | Description |
| --- | --- |
| `.gitignore` | Excludes Maven-generated build output from version control |
| `src/main/java/com/mycompany/game/TicTacToe.java` | Application entry point, Swing interface, and game logic |
| `src/main/java/com/mycompany/game/TicTacToe.form` | NetBeans GUI form definition |
| `lib/unknown/binary/AbsoluteLayout/SNAPSHOT/AbsoluteLayout-SNAPSHOT.jar` | Bundled AbsoluteLayout dependency |
| `pom.xml` | Maven build configuration and dependency declaration |
| `LICENSE` | MIT License terms |

## Technology

- Java 25
- Java Swing
- Apache NetBeans
- Apache Maven
- AbsoluteLayout

## License

This project is available under the [MIT License](LICENSE). Free to use, modify, and distribute with proper attribution.

## Author

**Malik Lateef**  
Software Engineering Student  
Lahore, Pakistan  
Email: [imaliklateef@gmail.com](mailto:imaliklateef@gmail.com)

> Academic portfolio project showcasing Java Swing, object-oriented programming, event-driven interfaces, and game logic.
