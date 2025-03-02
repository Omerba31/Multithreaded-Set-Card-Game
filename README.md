# Multithreaded Set Card Game

## Overview
This project is a **Java-based multithreaded implementation** of the classic **Set card game**. It demonstrates concurrency by using multiple threads for game management and player actions, ensuring efficient handling of game logic.

## Features
✅ Multi-threaded dealer and players for concurrency simulation  
✅ Swing-based graphical user interface (GUI)  
✅ Configurable game settings via `config.properties`  
✅ Unit tests using JUnit  
✅ Maven-based build system  

## Project Structure
```
Multithreaded-Set-Card-Game/
├── src/
│   ├── main/java/bguspl/set/        # Core game logic
│   │   ├── Config.java
│   │   ├── Env.java
│   │   ├── Main.java
│   │   ├── Dealer.java
│   │   ├── Player.java
│   │   ├── Table.java
│   │   ├── UserInterfaceSwing.java
│   │   ├── WindowManager.java
│   │   ├── ThreadLogger.java
│   ├── resources/
│   │   ├── config.properties        # Game settings
│   │   ├── cards/                   # Card images for GUI
│   ├── test/java/bguspl/set/ex/     # Unit tests
│   │   ├── PlayerTest.java
│   │   ├── TableTest.java
├── pom.xml                           # Maven build configuration
├── README.md                         # Project documentation
├── .gitignore                         # Ignore unnecessary files
```

## Installation & Build
### Prerequisites
- Java 8+ installed
- Maven installed

### Steps to Build
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/Multithreaded-Set-Card-Game.git
   cd Multithreaded-Set-Card-Game
   ```
2. Build the project using Maven:
   ```sh
   mvn clean install
   ```

## Running the Game
To run the game:
```sh
mvn exec:java -Dexec.mainClass="bguspl.set.Main"
```

## Configuration
Modify `src/main/resources/config.properties` to adjust game settings such as:
```
# Number of players
numPlayers=4

# Game speed (in ms)
gameSpeed=100
```

## Running Tests
To run unit tests:
```sh
mvn test
```

## Contributing
1. Fork the repository
2. Create a new branch (`git checkout -b feature-name`)
3. Commit changes (`git commit -m "Added feature"`)
4. Push branch (`git push origin feature-name`)
5. Submit a pull request

## License
[MIT License] - Free to use and modify.

## Author
Developed as part of a **Software Programming Laboratory (SPL) Assignment**.

