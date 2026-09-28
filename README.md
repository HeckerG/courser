# Coursera Assistant

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Platform](https://img.shields.io/badge/platform-Chrome%20MV3-blue)

A focused Coursera companion for video, reading, discussion, dialogue, and AI-assisted quiz workflows.

> **Disclaimer:** Quiz Automation provides AI-generated assistance powered by your personal Google Gemini API key. Answers are intended for educational and study reference; always review submissions for accuracy.

---

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [How to Use](#how-to-use)
- [Feature Details](#feature-details)
  - [Video Completion / Skip Video+](#video-completion--skip-video)
  - [Reading Material](#reading-material)
  - [Discussion Automation](#discussion-automation)
  - [Interactive Dialogue](#interactive-dialogue)
  - [AI Quiz Solver](#ai-quiz-solver)
  - [Shareable Link](#shareable-link)
- [Settings & Configuration](#settings--configuration)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Author](#author)

---

## Features

| Feature | Description | Status |
| :--- | :--- | :--- |
| **Video Completion** | Marks video lectures as completed with progress tracking and event dispatch | 🟢 Active |
| **Reading Material** | Automatically completes reading items and course supplements | 🟢 Active |
| **Discussion** | Submits relevant responses to course discussion forum prompts | 🟢 Active |
| **Dialogue** | Automates interactive dialogue coach sessions with native conclusion | 🟢 Active |
| **Quiz Solver** | AI-driven quiz assistance with live persistent progress window | 🟢 Active |
| **Shareable Link** | Captures and persists peer-review assignment submission URLs | 🟢 Active |

---

## Installation

1. Download or clone this repository to your local machine.
2. Open Google Chrome and navigate to `chrome://extensions/`.
3. Enable **Developer mode** using the toggle switch in the top-right corner.
4. Click the **Load unpacked** button.
5. Select the extension directory (containing `manifest.json`).
6. The extension is now installed and active in Chrome.

---

## How to Use

1. Navigate to your course on [Coursera](https://www.coursera.org).
2. Click the extension icon in the Chrome toolbar to open the popup.
3. Choose the desired automation action:
   - **Reading Material**: Automatically marks reading assignments as finished.
   - **Discussion**: Generates and posts discussion forum responses.
   - **Dialogue**: Navigates and concludes interactive dialogue items.
   - **Video Completion**: Completes all video lectures in the current course.
   - **Solve Quiz**: Solves the questions on an active quiz attempt page.

---

## Feature Details

### Video Completion / Skip Video+
Scans course syllabus for video lecture items, registers full viewing progress via Coursera's progress API, and verifies completion state.

### Reading Material
Identifies supplement and reading material items, marks them as read through Coursera's completion endpoints, and provides real-time toast feedback.

### Discussion Automation
Fetches discussion questions from course forums, crafts relevant responses, and submits them with configurable pacing delay to ensure natural interaction.

### Interactive Dialogue
Engages in structured conversational turns with Coursera's interactive Coach Dialogue system, maintaining dialogue context and concluding natively with completion verification.

### AI Quiz Solver
Parses quiz draft questions directly from the page, analyzes questions via Google Gemini API, selects the correct answer options in the DOM, and displays real-time execution stages in a dedicated persistent Quiz Solver window.

Supported Gemini models (Google Free Tier):
- `gemini-3-flash-preview` *(Default / Recommended)*
- `gemini-3.8-flash`
- `gemini-3.5-flash`

### Shareable Link
Copies and persists peer-graded assignment submission links across tabs and page reloads for seamless submission sharing.

---

## Settings & Configuration

Click the gear icon in the extension popup or open the Chrome extension options page (`dist/settings.html`) to configure:

- **Discussion Delay**: Pacing delay in milliseconds between discussion forum responses (default: 5000 ms).
- **Gemini API Key**: Your personal Google AI Studio Gemini API key (stored securely in local extension storage; never sent to third-party servers).
- **Gemini Model**: Select from approved free-tier Gemini models.
- **Auto Quiz**: Automatically initiate quiz solving upon navigating to a quiz attempt page.

---

## Keyboard Shortcuts

- `Alt + B` or `Alt + W`: Open extension popup.

---

## Author

- **Mayank Bisht**

---

> ⚠️ *This extension is an independent productivity tool and is not affiliated with, endorsed by, or sponsored by Coursera Inc.*
