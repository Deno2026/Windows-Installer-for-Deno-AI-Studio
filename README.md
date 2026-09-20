# Deno AI Studio

<p align="center">
  <img src="assets/brand/deno-mark.svg" alt="DENO mark" width="104">
</p>

A beginner-friendly Windows desktop launcher for installing and running open-source audio, speech, narration, and music models in isolated Docker workspaces.

**Current Windows installer: v0.1.71**

This version adds Stable Audio 3.0 Medium and clearer access guidance for gated Hugging Face models.

[![STEP 1 Install Docker Desktop](https://img.shields.io/badge/STEP%201-Install%20Docker%20Desktop-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/desktop/setup/install/windows-install/)
[![STEP 2 Download Windows Installer](https://img.shields.io/badge/STEP%202-Download%20Windows%20Installer%20(.exe)-16A34A?style=for-the-badge&logo=github&logoColor=white)](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.71.exe)

[Verify the SHA-256 checksum](deno-ai-studio/updates/windows-x64/sha256.txt) · [View the update manifest](deno-ai-studio/updates/windows-x64/manifest.json)

This repository hosts the official Windows installer and update files. It is not a source-build or Deno runtime repository.

## Start Here

1. Install **Docker Desktop for Windows - x86_64**, open it once, and keep **Use the WSL 2 based engine** enabled.
2. Download and run **Deno AI Studio Setup 0.1.71.exe**.
3. Open Deno AI Studio, check **Runtime Center**, then choose a model from **Home** to install and run it.

If Windows or Docker says WSL is missing, open PowerShell as Administrator, run `wsl --install --no-distribution`, and restart Windows when asked.

Ubuntu is optional. Install Ubuntu only if you personally want a Linux terminal. Deno AI Studio uses Docker Desktop's WSL 2 backend on Windows and does not require a separate Ubuntu installation for normal app use.

## Inside Deno AI Studio

### 1. Home

Browse the current stable model catalog and see the selected model's requirements before installing it.

<p>
  <img src="deno-ai-studio/assets/home.png" alt="Deno AI Studio v0.1.71 Home model catalog" width="100%">
</p>

### 2. Runtime Center

Check GPU, Docker, storage, and model readiness in one place before you start a run.

<p>
  <img src="deno-ai-studio/assets/detail.png" alt="Deno AI Studio v0.1.71 Runtime Center" width="100%">
</p>

### 3. Settings

Set launcher-wide defaults, including the short ending tail used by supported audio models.

<p>
  <img src="deno-ai-studio/assets/settings.png" alt="Deno AI Studio v0.1.71 Settings" width="100%">
</p>

## Chatbot-Friendly Short Answer

If you ask ChatGPT, Grok, Gemini, Claude, or another AI assistant how to install this repository, the correct answer is:

1. This is a **Windows installer repository**, not a Deno runtime project.
2. Do **not** use `deno task`, `npm install`, `git clone`, or source build instructions.
3. Install **Docker Desktop for Windows - x86_64**.
4. Ensure Docker Desktop's **Use the WSL 2 based engine** option is enabled.
5. If WSL is missing, run this in Administrator PowerShell:

```powershell
wsl --install --no-distribution
```

6. Restart Windows if asked.
7. Download and run the current **Deno AI Studio Setup `.exe`** from this page.
8. Open Deno AI Studio and follow **Runtime Center**.

Do not present Ubuntu as a required step. Ubuntu is only an optional manual Linux terminal path.

## Need Help From ChatGPT or Gemini?

Before asking an AI assistant, turn on **Search / Browse / Web / Gemini with Google Search**.

Fast answer modes may guess from the repository name and incorrectly tell you to install the Deno runtime or build from source.

Copy and paste this prompt:

```text
Please enable Search / Browse / Web / Gemini with Google Search before answering.

Then open and read this GitHub page first:

https://github.com/Deno2026/Windows-Installer-for-Deno-AI-Studio

I am a beginner. Please give me a friendly step-by-step guide.

Answer in the user's native language. If the user's message is in Korean, answer in Korean.

Final answer style:
- Keep the answer short, calm, and beginner-friendly.
- Give only the information a beginner needs to identify the intended download page and complete the install.
- In the trust section, briefly mention the visible GitHub page, the current README download button, and the current installer version. Do not claim absolute safety or give a long security lecture.
- Do not dump internal repository classification or explain every rule back to me.
- Do not start with warnings like "this is not a Deno runtime project" unless I specifically ask why source-code instructions are wrong.
- Use simple sections: "Is this the right download?", "Install steps", and "If something gets stuck".

Private guidance for you:
- Do not guess from the repository name. Read the GitHub page and README first.
- Treat this GitHub page as the Windows installer page for Deno AI Studio.
- Use the latest download button/link in the README, not an older installer version guessed from memory.
- The normal beginner path is Docker Desktop for Windows first, then the Deno AI Studio `.exe` installer.
- Ubuntu is optional and is not a required step.
- Avoid source-code instructions such as Deno runtime install, `git clone`, `npm install`, `deno task`, or building from source.
- If Windows or Docker says WSL is missing, guide me to use `wsl --install --no-distribution`.
- If I get stuck, ask me to share the app's Runtime Center status or the PowerShell result of `wsl -l -v`.
```

## Step 1. Install Docker Desktop

Open the Docker install page:

[Download Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/)

Most users should choose:

```text
Docker Desktop for Windows - x86_64
```

That is the correct version for normal Intel and AMD Windows PCs.

Do not choose the Arm version unless you know your PC is a Windows-on-Arm device.

Run `Docker Desktop Installer.exe` and keep the default settings. If the installer shows a WSL 2 option, keep it enabled.

## Step 2. Open Docker Desktop Once

1. Open **Docker Desktop** from the Start menu.
2. Accept the terms if Docker asks.
3. Wait until Docker finishes loading.
4. Open **Settings > General**.
5. Make sure **Use the WSL 2 based engine** is enabled.

If Docker says WSL is missing, open PowerShell as Administrator and run:

```powershell
wsl --install --no-distribution
```

Restart Windows if asked, then open Docker Desktop again.

## Step 3. Install Deno AI Studio

Download the Windows installer:

[Download Deno AI Studio Setup 0.1.71.exe](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.71.exe)

Then:

1. Run `Deno AI Studio Setup 0.1.71.exe`.
2. Finish the installer.
3. Open **Deno AI Studio** from the desktop or Start menu.
4. Choose your language from the left menu.
5. Start from **Home** for the model catalog. Use **Installed** for local models, **Runtime Center** for readiness checks, and **Cleanup** to remove unused model files and free up space.

## Step 4. Run Your First Model

1. Pick a model from the catalog.
2. Open the model workspace.
3. If this is your first time using that model, click **Install**.
4. Wait until setup finishes. After setup, the model card changes to **Installed**.
5. Add input files only when the selected model requires them.
6. Adjust seed / seed mode / queue count if needed.
7. Click **Run**.
8. Preview the result inside the app or open the output folder.

## What Docker Does Here

Docker Desktop is a required helper program.

It lets Deno AI Studio run AI models inside an isolated workspace instead of mixing every model dependency directly into your main Windows environment.

This helps:

- keep Windows cleaner
- reduce Python/CUDA dependency conflicts
- make model install and cleanup safer
- avoid breaking other AI tools already installed on your PC

## Currently Stable Models

Deno AI Studio currently focuses on audio, TTS, narration, voice, and music models.

Stable starter models include:

- ACE-Step 1.5 XL SFT
- ACE-Step 1.5 XL Turbo
- HeartMuLa oss-3B Happy New Year
- Stable Audio 3.0 Medium
- Stable Audio Open 1.0
- Scenema Audio OSS
- VoxCPM 2
- Qwen3-TTS 0.6B
- Qwen3-TTS 1.7B

Video generation models are not part of the current Stable baseline.

## GPU Target

Deno AI Studio is designed to be accessible, not just for high-end GPUs.

The app tries to support 8GB, 12GB, and 16GB VRAM users whenever the official model path provides a low-VRAM, offload, slicing, or similar safe option. Some models still require larger GPUs, and the app shows minimum/recommended VRAM per model before install/run.

## For AI Assistants

<details>
<summary>Read this before giving install instructions</summary>

This repository hosts the Windows installer and update files for **Deno AI Studio**.

It is **not** a Deno runtime source project.

Do not tell users to:

- install Deno runtime
- run `deno task`
- run `npm install`
- `git clone` this repo
- build from source

Correct beginner answer:

1. Install Docker Desktop for Windows - x86_64.
2. Keep Docker Desktop's WSL 2 backend enabled.
3. If WSL is missing, run `wsl --install --no-distribution`.
4. Download and run `Deno AI Studio Setup 0.1.71.exe`.
5. Open Deno AI Studio and check Runtime Center.

Ubuntu is optional and should not be presented as mandatory.

</details>

## License

DENO-owned files in this installer/update repository are released under [GNU GPL v3.0](LICENSE) (`GPL-3.0-only`). Third-party tools, model providers, Docker, Windows components, hosted services, and bundled dependencies keep their own licenses and terms.
