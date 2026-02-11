# SE333 Code Review Lab

A Java project designed for practicing code review skills. This lab contains intentional code issues for students to identify and fix using static analysis tools and manual code review.

## Project Structure

```
src/main/java/org/example/
├── Main.java      # Entry point
├── Review1.java   # String concatenation review
├── Review2.java   # Thread safety review
├── Review3.java   # Boxing/unboxing review
├── Review4.java   # Null check review
├── Review5.java   # Resource handling review
└── Review6.java   # Exception handling review
```

## Prerequisites

- Java 25+
- Maven 3.6+

## Build & Run

```bash
# Compile the project
mvn compile

# Run static analysis (Checkstyle + SpotBugs)
mvn verify

# Run Checkstyle only
mvn checkstyle:check

# Run SpotBugs only
mvn spotbugs:check
```

## Static Analysis Tools

This project is configured with two static analysis tools:

### Checkstyle
Checks for coding style violations based on the rules defined in `checkstyle.xml`.

### SpotBugs
Detects potential bugs and code quality issues through bytecode analysis.

## Lab Instructions

1. Review each `Review*.java` file
2. Identify code issues (bugs, bad practices, style violations)
3. Run static analysis tools to verify your findings
4. Fix the identified issues
5. Re-run the analysis to confirm all issues are resolved

## Learning Objectives

- Practice identifying common code issues
- Learn to use static analysis tools (Checkstyle, SpotBugs)
