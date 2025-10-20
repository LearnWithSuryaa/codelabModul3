# Java Demo Project

This is a Java project that requires Java 21 (LTS) to run.

## Prerequisites

Before you begin, ensure you have the following installed:
- Java 21 (LTS)
- Maven
- Git (optional, for version control)

## Installation Guide

### 1. Install Java 21

#### For macOS:
```bash
# Using Homebrew
brew install openjdk@21

# Set up system-wide Java symlink (requires admin password)
sudo ln -sfn /usr/local/opt/openjdk@21/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk-21.jdk

# Add Java 21 to your PATH (for zsh shell)
echo 'export PATH="/usr/local/opt/openjdk@21/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

#### For Windows:
1. Download OpenJDK 21 from [Adoptium](https://adoptium.net/)
2. Run the installer
3. Add JAVA_HOME environment variable
4. Add Java to your PATH

#### For Linux:
```bash
# Ubuntu/Debian
sudo apt update
sudo apt install openjdk-21-jdk

# Fedora
sudo dnf install java-21-openjdk-devel
```

### 2. Verify Java Installation
```bash
java -version
# Should show Java 21
```

### 3. Clone the Project (if using Git)
```bash
git clone [repository-url]
cd demo
```

### 4. Build the Project
```bash
mvn clean install
```

### 5. Run the Project
```bash
java -cp target/demo-1.0-SNAPSHOT.jar com.codelab.Main
```

## Project Structure
```
demo/
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/
│   │           └── codelab/
│   │               └── Main.java
│   └── test/
│       └── java/
└── pom.xml
```

## Development

This project uses:
- Java 21 (LTS)
- Maven for dependency management and building
- Standard Java project structure
-next