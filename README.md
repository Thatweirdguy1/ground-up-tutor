# Ground Up Tutor

Learn a subject from the ground up with clear explanations, worked examples, visual models and practice that adapts to your answers.

Ground Up Tutor is a skills-based plugin for ChatGPT and compatible local Codex clients. It provides a teaching workflow; it does not run a separate model, server or learning management system.

## How it teaches

- Starts with prerequisites and builds toward practical applications.
- Explains unfamiliar terms in everyday language before introducing formal notation.
- Teaches one concept at a time, then checks understanding.
- Changes the explanation when you get stuck and revisits earlier ideas.
- Uses your syllabus and notes when supplied, with source references.
- Creates useful visuals, flashcards and study files through available companion tools.

## Start learning

Select **Ground Up Tutor** in a supported ChatGPT or Codex client, then try:

> Teach me cloud security from zero, one concept at a time.

> Use my Google Drive syllabus to build a course. Start with the first topic and check my understanding.

> Explain gradient descent using a worked example and an interactive visual.

> Help me revise this chapter, then create flashcards and a PDF practice sheet.

You can ask for a faster pace, more detail, lecture mode, exam practice or a different analogy at any time.

## ChatGPT and phone access

The private account copy is available at [Ground Up Tutor](https://chatgpt.com/plugins/plugins_6b01a3512890819182b8c4e02c163371). Open it while signed into the same ChatGPT account and add or select it if prompted. On your phone, use the same account and a client that supports plugins. Available tools and plugin UI can differ by client; a desktop-only capability does not become a phone capability merely by installing this plugin.

## Local installation

Clone this repository into a permanent folder:

```sh
git clone https://github.com/Thatweirdguy1/ground-up-tutor.git
```

Use your local client's supported plugin or marketplace installer to load this folder. The portable manifest is `plugin.json`; `.codex-plugin/plugin.json` provides Codex compatibility. `.agents/plugins/marketplace.json` provides a repository marketplace entry. Installer commands vary by client version; check the installed client's help rather than assuming a CLI command exists.

This plugin has no runtime dependencies, API keys or MCP server of its own. It needs a compatible AI host to interpret its instructions. Installing it does not install companion plugins.

## Companion capabilities

| Capability | Used for |
| --- | --- |
| Browser / web search | Authoritative sources and information verification |
| Google Drive | Syllabi, lecture notes, textbooks and past papers |
| Data | Calculations, datasets and quantitative models |
| Visualize | Interactive explanations and simulations |
| AhaMotion | Animated explanations and teaching videos |
| Quizlet | Flashcard sets |
| PDF | Revision sheets and practice papers |
| Presentations | Visual lesson decks |
| Spreadsheets | Calculation models and study trackers |
| Documents | Editable notes and study guides |

Enable and connect companion capabilities in the host when needed. The tutor discovers available tools, follows their instructions and provides a clearly labeled fallback if unavailable. Account permissions, provider limits and any costs still apply. It never claims to have created an artifact until the provider confirms success.

## Progress and privacy

The tutor tracks progress in the conversation and can provide a compact checkpoint for resuming later. It does not provide automatic cross-chat memory, background monitoring or scheduled reminders. Persistent saving requires a supported destination and authorization. It reads relevant study materials rather than unrelated account files and does not publish private notes by default.

## Repository layout

- `plugin.json`: portable plugin metadata.
- `.codex-plugin/plugin.json`: local Codex compatibility metadata.
- `.agents/plugins/marketplace.json`: repository marketplace entry.
- `skills/teach-from-zero/SKILL.md`: core teaching instructions.
- `skills/teach-from-zero/references/tools-and-sources.md`: source handling, tool selection and study artifact guidance.
- `CHANGELOG.md`: release history.

## Development

Edit teaching behavior in the skill and integrations in its reference file. Keep names, versions and presentation synchronized across manifests. Validate JSON, skill frontmatter, referenced files and the final package inventory before release. Package only plugin files, excluding `.git`, secrets and temporary outputs. Updating GitHub does not automatically update an already installed local or cloud copy; reinstall or update through its respective supported flow.

## Limitations

Generated lessons can contain errors. The tutor is instructed to verify uncertain claims, show assumptions and distinguish simplified models from the full subject. Companion integrations are instructions for using available host capabilities, not bundled external services. No phone-specific interface or independent mobile app is included.
