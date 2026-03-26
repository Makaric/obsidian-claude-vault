# Obsidian Claude Vault

> AI-powered knowledge base: Obsidian + Claude Code integration with templates, skills, and automation.

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## What is this?

A ready-to-use Obsidian Vault pre-configured for seamless work with Claude Code (Anthropic's AI coding agent). Includes folder structure, note templates, Claude Code skills, system prompt (CLAUDE.md), and Git setup.

### Features

- **Structured Vault** with 7 organized folders (Resources, Tasks, Ideas, Projects, Daily, Templates, Archive)
- **4 Note Templates** (Research, Task, Project, Daily) with YAML frontmatter
- **CLAUDE.md** system prompt implementing Plan-Do-Verify methodology
- **3 Claude Code Skills**: quick-note, research-to-obsidian, code-scaffold, daily-review
- **Communication Style Skill** for personalized AI interaction
- **Git-ready** with proper .gitignore for Obsidian
- **Templater-compatible** templates

## Installation

### Prerequisites

- [Obsidian](https://obsidian.md/download) (v1.0+)
- [Git](https://git-scm.com/downloads)
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) (optional, for AI features)

---

### Windows

**Option 1: Git Clone (Recommended)**
```powershell
$repo = 'F:\ObsidianVault'
$utf8bom = New-Object System.Text.UTF8Encoding $true
Set-Location $repo

# === README.md ===
$readme = @'
# Obsidian Claude Vault

> AI-powered knowledge base: Obsidian + Claude Code integration with templates, skills, and automation.

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## What is this?

A ready-to-use Obsidian Vault pre-configured for seamless work with Claude Code (Anthropic's AI coding agent). Includes folder structure, note templates, Claude Code skills, system prompt (CLAUDE.md), and Git setup.

### Features

- **Structured Vault** with 7 organized folders (Resources, Tasks, Ideas, Projects, Daily, Templates, Archive)
- **4 Note Templates** (Research, Task, Project, Daily) with YAML frontmatter
- **CLAUDE.md** system prompt implementing Plan-Do-Verify methodology
- **3 Claude Code Skills**: quick-note, research-to-obsidian, code-scaffold, daily-review
- **Communication Style Skill** for personalized AI interaction
- **Git-ready** with proper .gitignore for Obsidian
- **Templater-compatible** templates

## Installation

### Prerequisites

- [Obsidian](https://obsidian.md/download) (v1.0+)
- [Git](https://git-scm.com/downloads)
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) (optional, for AI features)

---

### Windows

**Option 1: Git Clone (Recommended)**
```powershell
cd F:\
git clone https://github.com/Makaric/obsidian-claude-vault.git MyVault
```

**Option 2: Download ZIP/RAR**
1. Download archive from [Releases](https://github.com/Makaric/obsidian-claude-vault/releases)
2. Extract with WinRAR / 7-Zip / Windows Explorer to desired location (e.g. `F:\MyVault`)

**Open in Obsidian:**
1. Open Obsidian
2. Click vault icon (bottom-left) -> **Open folder as vault**
3. Select the extracted/cloned folder
4. Go to **Settings -> Core plugins -> Templates** -> enable -> set folder to `Templates`
5. (Optional) Install **Templater** plugin: Settings -> Community plugins -> Browse -> search "Templater" -> Install -> Enable

---

### Linux
```bash
cd ~/Documents
git clone https://github.com/Makaric/obsidian-claude-vault.git MyVault

# Install Obsidian (AppImage)
wget https://github.com/obsidianmd/obsidian-releases/releases/latest/download/Obsidian-latest.AppImage
chmod +x Obsidian-latest.AppImage
./Obsidian-latest.AppImage
```
Then open the cloned folder as vault in Obsidian (same steps as Windows).

**Snap:**
```bash
sudo snap install obsidian --classic
```

**Flatpak:**
```bash
flatpak install flathub md.obsidian.Obsidian
```

---

### macOS
```bash
cd ~/Documents
git clone https://github.com/Makaric/obsidian-claude-vault.git MyVault
```

Install Obsidian:
```bash
# Homebrew
brew install --cask obsidian
```
Or download .dmg from [obsidian.md](https://obsidian.md/download).

Then open cloned folder as vault in Obsidian.

---

## Folder Structure
```
ObsidianVault/
├── .claude/
│   └── skills/           # Claude Code skills
│       ├── maxim-communication.md
│       ├── research-to-obsidian.md
│       ├── quick-note.md
│       ├── code-scaffold.md
│       └── daily-review.md
├── Resources/            # Research, articles, references
├── Tasks/                # Tasks and checklists
├── Ideas/                # Ideas, hypotheses, drafts
├── Projects/             # Active projects
├── Daily/                # Daily notes / journal
├── Templates/            # Note templates
│   ├── Research Note.md
│   ├── Task.md
│   ├── Project.md
│   └── Daily.md
├── Archive/              # Completed / inactive notes
├── CLAUDE.md             # System prompt for Claude Code
├── .gitignore            # Git ignore rules
└── README.md             # This file
```

## Claude Code Skills

| Skill | Description |
|-------|-------------|
| `maxim-communication` | Personalized communication style (customize for yourself!) |
| `research-to-obsidian` | Research any topic and save structured notes to Vault |
| `quick-note` | Quickly save thoughts/ideas with proper encoding |
| `code-scaffold` | Scaffold new coding projects with proper structure |
| `daily-review` | End-of-day summary with learnings and plans |

## Using with Claude Code

1. Navigate to your vault folder in terminal
2. Run `claude` — it auto-detects `CLAUDE.md`
3. Claude Code will follow Plan-Do-Verify methodology
4. Skills are available in `.claude/skills/`

## Customization

- Edit `CLAUDE.md` to change AI behavior and methodology
- Modify skills in `.claude/skills/` to fit your workflow
- Add new templates to `Templates/` folder
- Adjust `.gitignore` for your needs

## Archive Extraction

- **WinRAR**: Right-click -> Extract Here / Extract to folder
- **7-Zip**: Right-click -> 7-Zip -> Extract Here
- **Windows**: Right-click -> Extract All
- **Linux**: `unzip obsidian-claude-vault-v1.0.0.zip -d MyVault`
- **macOS**: Double-click .zip file or `unzip` in terminal

## Contributing

PRs welcome! If you have useful skills or templates, feel free to contribute.

## License

[MIT](LICENSE) — do whatever you want with it.

---

**Made with Claude Code + human creativity**