# Cybersecurity Awareness Dashboard (PROG6221 POE)

A cross-platform desktop application built using the **C#** programming language, **Avalonia UI** (MVVM/Code-Behind), and **.NET 10**. This application serves as an interactive educational hub to train users in modern cybersecurity hygiene, combining a stateful Task Assistant, an interactive quiz with gamified ranking, an NLP-driven chatbot with multi-turn memory, and a real-time system audit log.

---

## 🎥 Video Presentation & Demonstration
*   **YouTube Presentation Link:** **[INSERT YOUR YOUTUBE VIDEO LINK HERE]**
*   **Scope of Video Demonstration:**
    1. **SQLite CRUD Integration:** Adding a task, reading it from the UI, updating its status to "Completed", and deleting it—demonstrating real-time database transactions.
    2. **Cyber Quiz Game:** Playing through the assessment to demonstrate correct/incorrect visual feedback, ending with a high score to show the dynamic rank evaluation (e.g., `🛡️ RANK: CYBER SENTINEL`).
    3. **NLP Chatbot:** Showing conversational context continuity (scheduling a task through dialogue) and response variation when querying for keywords.
    4. **CI/CD Pipeline:** Quick overview of the successful, passing GitHub Actions workflow.

---

## 🏗️ Architectural Overview & Technical Class Directory

The application follows a modular, single-window layout utilizing an optimized tab system. This maintains a clean separation of concerns and organizes components cleanly.

```text
ST10485361_Prog part2/              # Root repository directory
│
├── .github/
│   └── workflows/
│       └── build.yml               # GitHub Actions CI/CD workflow configuration
│
└── Prog part1/                     # Main C# project directory
    ├── bin/                        # Compiled binary executables
    ├── obj/                        # MSBuild assembly and NuGet restore caches
    │
    ├── App.axaml                   # Application-wide styles, themes, and resources
    ├── App.axaml.cs                # Global application startup and lifecycle logic
    │
    ├── MainWindow.axaml            # Core UI layout markup (Grids, TabControls, ListBoxes)
    ├── MainWindow.axaml.cs         # Principal controller and code-behind engine
    │
    ├── AudioManager.cs             # Plays interactive UI and alert audio assets
    ├── ChatBot.cs                  # Encapsulates core chatbot parsing behaviors
    ├── ChatResponses.cs            # Structured data contracts for text variations
    ├── KeywordResponder.cs         # Dictates keyword/regex mapping for NLP
    ├── SentimentDetector.cs        # Sentiment analysis engine for user input
    ├── MemoryStore.cs              # Manages conversational memory state
    │
    ├── Models.cs                   # Defines C# classes (CybersecurityTask, QuizQuestion)
    ├── Program.cs                  # Entry point for the Avalonia framework
    │
    ├── Prog part1.csproj           # MSBuild project file (Targets .NET 10.0)
    ├── Prog part1.sln              # Visual Studio Solution wrapper
    │
    └── tasks.db                    # Auto-generated SQLite local database
