# Python for Beginners

A learning repository for Python fundamentals. It contains two practice sets, each kept in its own file, together with screenshots that show the output of every chapter.

| File | Practice set | Screenshots |
|------|--------------|-------------|
| `python-pemula.py` | Python for Beginners (11 chapters) | `screenshots/bab01` to `bab10` |
| `python-dasar.py` | Python Basics (19 chapters) | `screenshots/dasar-bab01` to `dasar-bab19` |

## Part 1: Python for Beginners (`python-pemula.py`)

1. **Introduction & Python Installation**: checking the Python and pip versions, setting up the project and a virtual environment.
2. **Variables and Data Types**: integers, floats, strings, and booleans.
3. **Operators**: arithmetic, comparison, and logical operators (`and`, `or`, `not`).
4. **If Else Conditions**: `if`, `elif`, `else`, and indentation rules.
5. **Loops**: `for`, `while`, `break`, and `continue`.
6. **Lists and Dictionaries**: indexing, adding, updating, and removing items.
7. **Functions**: arguments, `*args`, `**kwargs`, and default values.
8. **Classes and Objects**: properties, constructors, and methods.
9. **PIP and Virtual Environments**: installing the `colorama` library inside the virtual environment.
10. **Environment/IDE Configuration**: configuring VS Code to use the interpreter from the virtual environment.
11. **README.md & Requirements.txt**: project documentation and the dependency list.

## Part 2: Python Basics (`python-dasar.py`)

1. Introduction & Python Installation
2. Basic Program Structure
3. Basic Data Types
4. Variables
5. Constants
6. Operators
7. Control Flow
8. Functions
9. List, Tuple, and Set
10. Dictionary
11. Class & Object
12. Encapsulation
13. Inheritance
14. Polymorphism
15. Abstraction
16. Exception Handling
17. File Handling
18. Modules (uses `kalkulator.py`)
19. Packages (uses the `perhitungan/` folder)

## Prerequisites

- Python 3.12 or newer
- Git
- Visual Studio Code (optional, recommended)

## Getting Started

1. Clone the repository:

   ```
   git clone https://github.com/marsya003/python-untuk-pemula.git
   cd python-untuk-pemula
   ```

2. Create and activate a virtual environment (Windows PowerShell):

   ```
   python -m venv venv
   .\venv\Scripts\Activate.ps1
   ```

   If PowerShell reports an *execution policy* error, run this once:

   ```
   Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
   ```

3. Install the dependencies:

   ```
   pip install -r requirements.txt
   ```

4. Run a program:

   ```
   python python-pemula.py
   python python-dasar.py
   ```

Both programs print their output from top to bottom, so the output of earlier chapters appears first.

## Project Structure

```
python-untuk-pemula/
├── .vscode/
│   └── settings.json     # VS Code interpreter configuration
├── perhitungan/          # package used in chapter 19 of Part 2
│   ├── __init__.py
│   └── kalkulator.py
├── screenshots/          # execution screenshots for every chapter
├── kalkulator.py         # module used in chapter 18 of Part 2
├── python-pemula.py      # Part 1 source code
├── python-dasar.py       # Part 2 source code
├── requirements.txt      # dependency list
├── .gitignore
└── README.md
```

Chapter 17 of Part 2 creates a file named `catatan.txt` when it runs. The file is generated automatically and is excluded from version control through `.gitignore`.

## Dependencies

| Library  | Purpose                        |
|----------|--------------------------------|
| colorama | Colored output in the terminal |

The exact version is pinned in `requirements.txt`. `python-dasar.py` uses only the Python standard library.

## Commit Convention

Every chapter is committed separately and pushed right after it is finished. Commit messages follow [Conventional Commits](https://www.conventionalcommits.org/), for example:

```
feat(basics): add variables and data types examples
feat(control-flow): add if, elif, and else statements
feat(dasar): implement dictionary
docs: update README
```