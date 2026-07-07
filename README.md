# Complete Java Guide on Termux

Technical Documentation | Platform: Android (Termux) | Date: June 19, 2026

---

## 📋 Table of Contents

- [1. Introduction](#1-introduction)
- [2. Installing Java on Termux](#2-installing-java-on-termux)
- [3. Creating Your First Java File](#3-creating-your-first-java-file)
- [4. Java Basic Structure](#4-java-basic-structure)
- [5. Compile & Run Program](#5-compile--run-program)
- [6. Example Program (Loops)](#6-example-program-loops)
- [7. Most Common Errors](#7-most-common-errors)
- [8. Java Basic Pattern to Remember](#8-java-basic-pattern-to-remember)
- [9. Quick Workflow on Termux](#9-quick-workflow-on-termux)
- [10. Next Level](#10-next-level)

---

## 1. Introduction

### What is Java?

Java is a popular, stable, and widely used programming language in enterprise applications, Android development, and backend systems.

### Why Learn Java on Termux?

| Advantage | Description |
|-----------|-------------|
| **No Laptop Needed** | Learn Java directly from your phone |
| **Portable** | Carry it anywhere, practice anytime |
| **Lightweight** | Termux + OpenJDK 21 doesn't burden your phone |
| **Complete** | Can compile, run, and even build small projects |

---

## 2. Installing Java on Termux

### Step 1: Update & Upgrade

```bash
pkg update && pkg upgrade
```

### Step 2: Install OpenJDK 21

```bash
pkg install openjdk-21
```

### Step 3: Verify Installation

Check if Java is installed correctly:

```bash
java --version
javac --version
```

#### Expected Output

| Command | Example Output |
|---------|-----------------|
| `java --version` | `openjdk version "21.0.x"` |
| `javac --version` | `javac 21.0.x` |

✅ **If both commands display version numbers, Java is ready to use.**

---

## 3. Creating Your First Java File

### Step 1: Open Editor on Termux

```bash
nano Main.java
```

### Step 2: Type Java Code

Type the code below (explanation provided in the next section).

### Step 3: Save File

| Key | Function |
|-----|----------|
| `CTRL + O` | Save file |
| `Enter` | Confirm file name |
| `CTRL + X` | Exit nano editor |

---

## 4. Java Basic Structure (MANDATORY)

### Basic Code

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello Faris");
    }
}
```

### Explanation of Each Part

| Code Part | Function |
|-----------|----------|
| `public class Main` | Creates a class named Main — file name must match class name! |
| `public static void main(String[] args)` | Main method — entry point of all Java programs. Mandatory! |
| `System.out.println("...");` | Command to print text to the screen |
| `{ }` | Marks a code block (start & end) |
| `;` | Ends each statement |

⚠️ **Important Rule:** The `.java` file name MUST match the class name inside it. 

**Example:** `Main.java` → `class Main`

---

## 5. Compile & Run Program

### Compile (Convert Code to Program)

```bash
javac Main.java
```

**Result:** If successful, a new file named `Main.class` will appear (Java bytecode file).

### Run Program

```bash
java Main
```

#### Output

```
Hello Faris
```

💡 **Tip:** Run with `java` without `.class` or `.java` — just the class name.

---

## 6. Example Program (Loops)

### Code

```java
public class Main {
    public static void main(String[] args) {
        for (int i = 0; i <= 5; i++) {
            System.out.println(i);
        }
    }
}
```

### Output

```
0
1
2
3
4
5
```

### Explanation

| Code Part | Function |
|-----------|----------|
| `for (int i = 0; i <= 5; i++)` | Loop from 0 to 5 |
| `System.out.println(i);` | Print value of `i` each iteration |

---

## 7. Most Common Errors

### ❌ Case Sensitivity Error

**Wrong (lowercase):**

```java
system.out.println("Hello");
```

**✅ Correct (uppercase):**

```java
System.out.println("Hello");
```

📌 **Lesson:** Java is case-sensitive — uppercase and lowercase are distinguished!

### Other Common Errors

| Error | Cause | Solution |
|-------|-------|----------|
| `class Main is public, should be declared in a file named Main.java` | File name doesn't match class name | Rename file or class to match |
| `cannot find symbol` | Typo in method/variable name | Double-check code spelling |
| `';' expected` | Missing semicolon `;` at end of statement | Add `;` |
| `incompatible types` | Wrong data type assignment | Check variable types match |

---

## 8. Java Basic Pattern to Remember

| Element | Example | Function |
|---------|---------|----------|
| **class** | `class Main` | Wraps all code |
| **main method** | `public static void main` | Program entry point |
| **print** | `System.out.println` | Print to screen |
| **curly braces** | `{ }` | Open & close code block |
| **semicolon** | `;` | End statement |
| **parentheses** | `( )` | Group parameters |

---

## 9. Quick Workflow on Termux

```bash
# 1. Create file
nano Main.java

# 2. Compile (convert to program)
javac Main.java

# 3. Run
java Main
```

---

## 10. Next Level

After mastering the basics, Faris will learn:

| Topic | Function |
|-------|----------|
| **Scanner** | Receive keyboard input |
| **if-else** | Branching (decisions) |
| **while loop** | Loops with conditions |
| **Array** | Store multiple data |
| **Method** | Create your own functions |
| **OOP** | Object-Oriented Programming (class & object) |

---

## 📊 Command Summary

| Command | Function |
|---------|----------|
| `pkg install openjdk-21` | Install Java |
| `java --version` | Check Java version |
| `javac Main.java` | Compile Java file |
| `java Main` | Run program |
| `nano Main.java` | Create/edit Java file |
| `ls` | List files in directory |
| `rm Main.class` | Delete compiled file |
| `clear` | Clear terminal screen |

---

## 💡 Key Points for Faris

### Remember These Rules

1. **File name = Class name** — Always match them
2. **Case sensitive** — `System` ≠ `system`
3. **Semicolons required** — End each statement with `;`
4. **Curly braces** — Always use matching `{` and `}`
5. **main() is mandatory** — Every Java program needs it

### Three Steps Always

```
Write Code (nano) → Compile (javac) → Run (java)
```

---

## ✅ Final Status

| Component | Status |
|-----------|--------|
| Java on Termux | ✅ Installed (openjdk-21) |
| Main.java File | ✅ Can be created |
| Compile javac | ✅ Runs normally |
| Run java | ✅ Runs normally |
| Hello Program | ✅ Output matches |
| Loop Example | ✅ Works correctly |
| Error Handling | ✅ Common errors documented |

---

## 🎯 Your First Steps

1. **Install Java** → `pkg install openjdk-21`
2. **Create Main.java** → `nano Main.java`
3. **Compile** → `javac Main.java`
4. **Run** → `java Main`
5. **See output** → "Hello Faris"

**Congratulations!** You've just written and executed your first Java program on your phone! 🎉

---

**Last Updated:** June 19, 2026
