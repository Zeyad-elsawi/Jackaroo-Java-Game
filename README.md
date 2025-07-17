
![image](https://github.com/user-attachments/assets/7b9bbfd5-8ef2-4351-8f80-b4997b1c9623)
# Jackaroo Java Game

A strategic card game where players compete to move their marbles around the board using playing cards with special abilities.

---

## Game Files

Download the game files for the best experience:
[Download Game Files](https://drive.google.com/file/d/1xEStqFRyrrj3SGF4W7-zosbdiKT924Hd/view?usp=sharing)

## Gameplay

Watch the gameplay demo:
[Gameplay Video](https://drive.google.com/file/d/13SRTS8yHRUVVbRUT6kDLSzcZ4NvuA0QU/view?usp=sharing)

## Game Overview

Jackaroo is a multiplayer card game that blends strategy with luck. Players use a special deck of cards to move their marbles around a themed board, each card enabling specific movement rules or actions.

## Features

* Multiplayer support for human and AI players
* Strategic, card-driven gameplay
* Unique card abilities for each rank
* Marble movement mechanics with zones (Safe/Home)
* Western-themed board and animations
* Wild West Story Mode: Immerse yourself in a narrative-driven campaign with themed scenarios and objectives
* Responsive and interactive user interface
* Draw and discard system

## Card Abilities

| Card              | Ability                                                             |
| ----------------- | ------------------------------------------------------------------- |
| **Ace**           | Field a marble from the Home Zone or move one marble 1 step forward |
| **Two**           | Move one marble 2 steps forward                                     |
| **Three**         | Move one marble 3 steps forward                                     |
| **Four**          | Move one marble 4 steps backward                                    |
| **Five**          | Move any marble 5 steps forward                                     |
| **Six**           | Move one marble 6 steps forward                                     |
| **Seven**         | Move two marbles a total of 7 steps or one marble 7 steps forward   |
| **Eight**         | Move one marble 8 steps forward                                     |
| **Nine**          | Move one marble 9 steps forward                                     |
| **Ten**           | Discard a random card from next player or move 10 steps forward     |
| **Jack**          | Swap marbles or move 11 steps forward                               |
| **Queen**         | Discard a random card from a random player or move 12 steps forward |
| **King**          | Field a marble or move 13 steps forward (killing marbles in path)   |
| **Marble Burner** | Send an opponent's marble home                                      |
| **Marble Saver**  | Move your marble to a random safe zone                              |

## Installation

### IntelliJ IDEA

1. **Extract zip file and open the project**:

   * Navigate to **File > Open...** and select the project directory.
   * Ensure JDK 11 or higher is selected.
2. **Set up JavaFX**:

   * Download the JavaFX SDK from the [Gluon JavaFX download page](https://gluonhq.com/products/javafx/).
   * Extract the SDK.
   * Go to **File > Project Structure... > Libraries** and add the `lib` directory.
   * Add VM options under **Run > Edit Configurations...**:

     ```
     --module-path /path_to_javafx_lib --add-modules javafx.controls,javafx.fxml,javafx.media
     ```
3. **Build and run**:

   * Build: **Build > Build Project**
   * Run: Select the main class and click **Run**

### Eclipse

1. **Import zip file into Eclipse**:

   * Go to **File > Import... > Existing Projects into Workspace**
   * Choose the zip directory
2. **Set up JavaFX**:

   * Follow the same JavaFX SDK setup as above
   * Go to **Project > Properties > Java Build Path > Modulepath > Add External JARs...** and add JARs from `lib`
   * Add VM options under **Run > Run Configurations...**:

     ```
     --module-path /path_to_javafx_lib --add-modules javafx.controls,javafx.fxml,javafx.media
     ```
3. **Build and run**:

   * Right-click project > **Build Project**
   * Select the main class and click **Run**

## Dependencies

* **JavaFX**: UI framework, required for visuals and media
* **JDK 11 or higher**: Required to build and run the project

(Refer to the Bro Code JavaFX Playlist for detailed JavaFX setup guidance.)

## How to Play

1. Launch the game and choose the number of players
2. Each player gets a hand of cards and a set of marbles
3. On each turn:

   * Play a card
   * Apply the card's movement rule
   * Draw a new card
4. The winner is the first to move all marbles into the Safe Zone

### Controls

* **Mouse Click**: Select cards, buttons, and interact with UI
* **Marble Selection**: Enter target cell index in "Select Marbles" panel
* **F Key**: Field a marble instantly (when playing Ace or King)
* **X Key**: Terminate the current game session

## Technical Details

### Core Technologies

* **Java 23** for application logic
* **JavaFX**:

  * FXML layouts
  * CSS styling
  * MediaPlayer integration
  * Animation and graphics APIs

### Architecture & Design Patterns

* **MVC Architecture**:

  * Model: Game logic and state
  * View: UI built with JavaFX
  * Controller: Handles input and game flow
* **OOP Principles**:

  * Inheritance, polymorphism, encapsulation, abstraction

### Feature Implementation

* **Exception Handling**:

  * Custom game errors
  * Validation for moves and inputs
* **Concurrency**:

  * Multithreaded AI players
  * Background task execution
* **Data Management**:

  * Game state serialization
  * Configurations and player stats

### UI/UX Components

* **Custom Controls**:

  * Card viewer
  * Animated marble transitions
* **Effects**:

  * Card flips, marble kills
  * Endgame animations
* **Responsive Design**:

  * Dynamic scaling and multi-resolution support

### AI Behavior

* **Strategic Planning**:

  * Risk evaluation
  * Turn-based decision trees

### Testing & QA

* **Unit Testing** with JUnit
* **Integration Testing** for game flow and multiplayer
* **Performance Optimization**:

  * Efficient memory usage
  * Smooth animations

## Contributing

We welcome community contributions! You can:

* Submit issues and bug reports
* Open Pull Requests with improvements

Please follow Java coding best practices and include documentation where needed.

## Credits

Developed for CSEN401 at the German University in Cairo.

### Game Development Team

* Zeyad Ahmed Elsawi
* Mark Raymond Takla
* Jonathan Maged Daksis
* Aly Ahmed Aly

## Contact

* **Mark**: [LinkedIn](https://www.linkedin.com/in/mark-takla/)
* **Zeyad**: [LinkedIn](https://www.linkedin.com/in/zeyad-elsawi-0a0063284/)
