# Converter Suite

A Java Swing desktop application that combines three practical utilities in one project: an age calculator, a temperature converter, and a weight converter. Each tool is designed to be easy to use, fast to understand, and ideal for educational or personal productivity projects.

## Overview

This project provides a compact desktop utility suite for everyday calculations. Users can calculate age from a selected birth date, convert values between major temperature units, and switch between common weight measurements without leaving the application.

The interface uses a clean, beginner-friendly Swing layout with clear labels, combo boxes, input fields, and result displays, making the app suitable for students, beginners, and quick utility use.

## Features

- Age calculator with month, day, and year selection
- Automatic calculation of years, months, and days lived
- Temperature conversion between Celsius, Fahrenheit, Kelvin, and Rankine
- Weight conversion between kilogram, gram, pound, and ounce
- Simple input and output fields for each tool
- Clear button to reset the current calculation
- Responsive Java Swing desktop interface
- Beginner-friendly design built with Apache NetBeans GUI forms

## Requirements

- Java Development Kit (JDK) 25 or later
- Apache NetBeans with Java and Maven support
- Apache Maven

The project uses the `AbsoluteLayout` dependency stored in the repository's `lib/` directory and configured in `pom.xml`.

## Build and Run

### Apache NetBeans

1. Open Apache NetBeans and choose **File > Open Project**.
2. Select the project folder containing `pom.xml`.
3. Allow Maven to load the project and dependencies.
4. Open one of the main classes:
   - `src/main/java/com/mycompany/converter/Age.java`
   - `src/main/java/com/mycompany/converter/TEMPERATURE.java`
   - `src/main/java/com/mycompany/converter/weight.java`
5. Right-click the file and choose **Run File** to launch the selected tool.

### Command Line

From the project root, build the project with Maven:

```bash
mvn clean package
```

Run the individual desktop tools by targeting their main classes:

```bash
mvn exec:java -Dexec.mainClass=com.mycompany.game.Age
mvn exec:java -Dexec.mainClass=com.mycompany.game.TEMPERATURE
mvn exec:java -Dexec.mainClass=com.mycompany.game.weight
```

A graphical desktop environment is required to view and interact with the Swing app.

## How to Use

### Age Calculator
1. Select the birth month, day, and year.
2. Click **Calculator**.
3. The program displays total years, months, and days.

### Temperature Converter
1. Choose the source temperature unit.
2. Enter the value to convert.
3. Choose the target unit and view the converted result.

### Weight Converter
1. Select the source weight unit.
2. Enter the value.
3. Choose the target unit and view the converted result.

## Project Structure

```text
.
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
│                   └── converter/
│                       ├── Age.form
│                       ├── Age.java
│                       ├── TEMPERATURE.form
│                       ├── TEMPERATURE.java
│                       ├── weight.form
│                       └── weight.java
├── README.md
└── .gitignore
```

| Path | Description |
| --- | --- |
| `src/main/java/com/mycompany/converter/Age.java` | Age calculator GUI and logic |
| `src/main/java/com/mycompany/converter/TEMPERATURE.java` | Temperature conversion tool |
| `src/main/java/com/mycompany/converter/weight.java` | Weight conversion tool |
| `src/main/java/com/mycompany/converter/*.form` | NetBeans-generated GUI form files |
| `pom.xml` | Maven build configuration and dependency setup |
| `lib/.../AbsoluteLayout-SNAPSHOT.jar` | Swing layout dependency |
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

> A compact Java desktop utility project for practical calculation tasks in everyday life.
