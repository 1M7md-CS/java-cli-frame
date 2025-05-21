# Java CLI Utils

[![CLI](https://img.shields.io/badge/CLI-blue.svg)](https://en.wikipedia.org/wiki/Command-line_interface)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Java](https://img.shields.io/badge/Java-24-red.svg)](https://www.oracle.com/java/)
[![GitHub issues](https://img.shields.io/github/issues/1M7md-CS/java-cli-utils)](https://github.com/1M7md-CS/java-cli-utils/issues)

A simple Java utility for rendering styled console menus and exit messages with customizable borders and ANSI colors. This project is designed for CLI applications to create professional-looking console interfaces.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Menu Example](#menu-example)
- [Exit Message Example](#exit-message-example)
- [Frames](#frames)
- [License](#license)
- [Author](#author)

## Features

- Render menu frames with 8 different border styles.
- Support for colored text using ANSI escape codes for titles, options, and frames.
- Center-aligned text for clean and organized output.

## Installation

   ```bash
   1. Clone the repository:
   git clone https://github.com/1M7md-CS/java-cli-utils.git
   
   2. Navigate to project directory:
   cd java-cli-utils
   
   3. Ensure you have Java 24 or higher installed.
   
   4. Include 'Frame.java' and 'ConsoleColors.java' in your Java project under the cli package.
   ```

## Menu Example

1. Initial title and options

```java
String title = "My Title";

String[] options = {"Option 1", "Option 2", "Option 3", "Option 4"};
```

2. use 'Frame' class to call 'printMenuFrame' method.

```java
'printMenuFrame' method takes 3 parameters:

1. String title = "Menu Title";
2. String[] lines = {"Option 1", "Option 2", "Option 3", "Option 4"};
3. int longestLineLength // The longest length of lines[] and title
4. int frameStyle // There's 8 different frame style for now pick one of them

call method:
Frame.printMenuFrame(title, lines, 83, 1);

```

## Exit Message Example

```java

String exitMessage = "Thank you for using our application!";

Frame.printExitMessage(exitMessage, 2);

```

 
## Frames

```
1:                             2:                                  3:
╒───────────────────╕          ┌───────────────────┐               ╔═══════════════════╗
│    Menu Title     │          │    Menu Title     │               │    Menu Title     │
╞───────────────────╡          ├───────────────────┤               ╠═══════════════════╣
│  Option 1         │          │  Option 1         │               │  Option 1         │
│  Option 2         │          │  Option 2         │               │  Option 2         │
│  Option 3         │          │  Option 3         │               │  Option 3         │
│  Option 4         │          │  Option 4         │               │  Option 4         │
╘───────────────────╛          └───────────────────┘               ╚═══════════════════╝

4:                             5:                                  6:
╒═══════════════════╕          ╔───────────────────╗               ╔═══════════════════╗
║    Menu Title     ║          ║    Menu Title     ║               ║    Menu Title     ║
╞═══════════════════╡          ╟───────────────────╢               ╠═══════════════════╣
║  Option 1         ║          ║  Option 1         ║               ║  Option 1         ║
║  Option 2         ║          ║  Option 2         ║               ║  Option 2         ║
║  Option 3         ║          ║  Option 3         ║               ║  Option 3         ║
║  Option 4         ║          ║  Option 4         ║               ║  Option 4         ║
╘═══════════════════╛          ╚───────────────────╝               ╚═══════════════════╝

```


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author
Mohammad Hammad - [GitHub](https://github.com/1M7md-CS)






