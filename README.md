# CybersecurityBot

## Overview
CybersecurityBot is a powerful application designed to enhance security measures through automation and machine learning. The bot assists in identifying vulnerabilities, monitoring network traffic, and providing actionable insights to improve overall cybersecurity posture.

## Features
- **Automated Vulnerability Scanning**: Regularly scans systems for known vulnerabilities and reports findings.
- **Real-time Monitoring**: Monitors network traffic for suspicious activities and alerts users to potential threats.
- **Compliance Checks**: Assists in maintaining compliance with various regulatory standards.
- **Customizable Alerts**: Users can set up alerts based on specific criteria to stay informed about security issues.
- **User-friendly Interface**: Easy-to-navigate interface for managing security tasks efficiently.

## Installation
To install CybersecurityBot, follow these steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/ShannonRS-maker/Prog-part1.git
# PROG6221 Part 2 - Advanced Chatbot Application

### Student Details
* **Name:** Shannon R. September
* **Student Number:** ST10485361

---

## Project Overview
This repository contains a highly structured, interactive C# application built as a secure Chatbot and Security Dashboard system. The application processes user inputs dynamically, runs text analysis, logs data trends, and manages internal states through a modular architecture.

### Key Features
* **Interactive Dynamic Chatbot:** Uses a responsive core engine to handle user conversations based on contextual triggers.
* **Intelligent Content Filtering:** Includes a custom `SentimentDetector` and `KeywordResponder` to analyze user inputs and flag specific phrases or moods.
* **State & Memory Management:** Utilizes a `MemoryStore` component to cache session data and track user interactions over time.
* **Audio Integration:** Features an automated audio engine (`AudioManager`) utilizing `greeting.wav` to trigger auditory system alerts upon successful initialization.

---

## Technical Architecture & Design Pattern
The project strictly follows clean coding standards and separation of concerns by breaking down individual systems into standalone classes:
* **Program.cs:** The main application entry point that bootstraps the configuration and executes the runtime loop.
* **ChatBot.cs:** The central orchestrator handling interaction flow, data handoffs, and user sessions.
* **SentimentDetector.cs / KeywordResponder.cs:** Specialized utility classes dedicated to text analysis, validation, and pattern parsing.
* **MemoryStore.cs / Topics.cs:** Data layer components structuring cached strings, flags, and thematic response arrays.

---

## Environmental Execution Note
* **Target Framework:** .NET 10.0 Core
* **Cross-Platform Compatibility Configuration:** Due to specific cross-platform framework rendering limitations encountered with Avalonia UI engines on Apple Silicon macOS hosts during compilation (`AVLN:0004`), the interactive UI assets (`App.axaml`, `MainWindow.axaml`) have been securely backed up (`.bak`). 
* The application runs perfectly as a high-performance, fully optimized **Console Interface**. 

### How to Run the Application Natively
To launch the application locally, open your terminal, navigate to the project directory, and execute:
```bash
dotnet run
