# Shopping System

This project is a simplified shopping system designed to provide a hands-on experience in building a robust and maintainable software application while incorporating SOLID principles and design patterns.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Running the Application](#running-the-application)
- [Running Tests](#running-tests)
- [Design Patterns and SOLID Principles](#design-patterns-and-solid-principles)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## Overview

This system allows customers to:
- Browse products
- Add items to their shopping cart
- Place orders
- Simulate the payment process

## Prerequisites

To run this application, you need the following:
- Java Development Kit (JDK) 11 or higher
- Apache Maven 3.6.3 or higher
- JavaFX 11 or higher

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/VisheshThanki/Shopping-System.git
   cd shopping-system
2. Install dependencies:
Ensure you have JavaFX libraries. You can download them from the JavaFX website.

3. Configure JavaFX:
Update your pom.xml with the correct JavaFX dependencies. An example configuration is already provided.

Running the Application

Run the application:
You need to specify the JavaFX modules in the java command. Here's an example:

bash
Copy code
mvn exec:java -f pom.xml -Dexec.mainClass="edu.depaul.app.MainView" -Dexec.args="--module-path /path/to/javafx-sdk-11/lib --add-modules javafx.controls,javafx.fxml"
Replace /path/to/javafx-sdk-11/lib with the actual path to your JavaFX SDK.

Design Patterns and SOLID Principles
This project implements several design patterns and adheres to SOLID principles:

Singleton Pattern: Ensured by the ShoppingCart class.
Factory Pattern: Implemented in the ProductFactory class.
Builder Pattern: Can be observed in the Order creation process.
Single Responsibility Principle (SRP): Each class has a single responsibility.
Open/Closed Principle (OCP): Classes are open for extension but closed for modification.
Liskov Substitution Principle (LSP): Subclasses can replace their base classes without affecting the program.
Interface Segregation Principle (ISP): Specific interfaces are used for different functionalities.
Dependency Inversion Principle (DIP): Higher-level modules depend on abstractions.

Contributing
Contributions are welcome! Please follow these steps to contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes.
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature-branch).
Create a new Pull Request.
