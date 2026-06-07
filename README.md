# Java Pipeline

Dedicated GitHub Actions pipeline for building and running Java-based applications.

## Features

- Build Java applications using Maven
- Run Java applications
- Support for Java 11, 17, and 21
- Configurable via workflow dispatch
- Can be triggered from other repositories

## Usage

### Trigger Manually

Go to Actions tab → Select "Java Build and Run Pipeline" → Click "Run workflow"

### Trigger from Another Repository

Use repository_dispatch or workflow_dispatch events

## Configuration

The pipeline accepts the following inputs:
- `java_version`: Java version to use (11, 17, or 21)
- `maven_goals`: Maven goals to execute (default: clean install)
- `run_application`: Whether to run the application after build (true/false)
