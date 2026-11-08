# COMP3180 – Narrative Design
## AI-Powered Fantasy RPG Narrative System

### Project Overview

This project explores the use of locally hosted AI to create interactive fantasy RPG storytelling experiences. Using a custom GPT-OSS 20B model through Ollama, the project aims to create an AI Game Master capable of narrating adventures, developing fictional worlds, introducing characters and responding to player decisions.

Rather than following a fixed storyline, players can interact with the AI through natural language, make their own decisions and influence how the adventure unfolds. The AI is designed to support fantasy role-playing campaigns inspired by traditional tabletop RPGs such as Dungeons & Dragons.

The project uses a custom model configuration to give the AI specific narrative instructions, guiding its behaviour as a Game Master and helping establish a consistent fantasy RPG experience.

### Inspirations and References

The project draws inspiration from several existing creators and games:

- **DougDoug** – Inspiration for entertaining AI interactions and experimenting with AI-driven experiences.
- **Dungeons & Dragons (D&D)** – The main inspiration for fantasy role-playing, player choice, world-building and the Game Master approach to storytelling.
- **The Stanley Parable** – Inspiration for interactive storytelling, narrative experimentation and the relationship between player decisions and the story.
- **Detroit: Become Human** – Inspiration for branching narratives and the impact of player choices on story progression.

---

## Technologies Used

- **Ollama** – Used to download, manage and run AI models locally.
- **GPT-OSS 20B** – The base language model powering the narrative system.
- **Custom Modelfile** – Contains the system instructions that configure the AI's storytelling behaviour.
- **PowerShell / Windows Terminal** – Used to create, configure and interact with the custom model.

---

## Installation and Setup

Follow these instructions to set up and run the project on a Windows computer.

### 1. Install Ollama

Download and install Ollama from its official website:

https://ollama.com/download/windows

Once installed, open PowerShell and check that Ollama is working:

```powershell
ollama --version
```

### 2. Download the Base AI Model

The project uses GPT-OSS 20B as its base model.

Download it using:

```powershell
ollama pull gpt-oss:20b
```

This downloads the model files required to run the AI locally. The download may take some time and requires sufficient storage space and system memory.

### 3. Download the Project

Clone this GitHub repository:

```powershell
git clone [INSERT REPOSITORY URL]
```

Navigate into the downloaded project folder:

```powershell
cd COMP3180-Narrative-Design
```

Alternatively, download the repository as a ZIP file from GitHub and extract it.

### 4. Create the Custom AI Model

The repository contains a `Modelfile` that defines the custom storytelling instructions for the AI.

Make sure the `Modelfile` is located in your current project directory.

Create the custom model using:

```powershell
ollama create Comp3180-NarrativeAI -f Modelfile
```

This creates a new model called `Comp3180-NarrativeAI`, using GPT-OSS 20B as its base and applying the project's custom narrative instructions.

**Important:** The base GPT-OSS 20B model must already be downloaded before creating the custom model.

### 5. Run the Narrative AI

Once the model has been created, launch it using:

```powershell
ollama run Comp3180-NarrativeAI
```

You can now interact with the AI directly through the terminal and begin your fantasy RPG adventure.

---

## Project Structure

The repository contains the files required to configure and run the custom narrative AI.

```text
COMP3180-Narrative-Design/
│
├── Modelfile
│
├── README.md
│
└── [Additional story files and documentation]
```

---

## Usage

Once the model is running, players can interact with the AI by describing their character's actions, asking questions or making decisions within the story.

For example:

**Player:**
"I enter the tavern and look around for someone who might have information about the missing wizard."

**AI:**
The tavern is filled with the sound of conversation and clinking tankards. A hooded figure sits alone in the corner, watching you carefully. What would you like to do?

The player can then continue interacting with the AI to develop the adventure.

---

## Current References

- DougDoug
- Dungeons & Dragons Campaigns
- The Stanley Parable
- Detroit: Become Human

---

## Project Purpose

The goal of this project is to explore how locally hosted language models can be used to create more flexible and interactive narrative experiences. By combining AI-generated storytelling with traditional fantasy RPG mechanics, the project investigates how players can become active participants in shaping a story rather than simply following a predetermined narrative.
