# Plugin for CXGRD

> In active development

This repository is the collection of SKILL.md files for Claude Code.

## Installation

Run `/plugin marketplace add anthropics/claude-plugins-community` to register the marketplace

Run `/plugin install cxgrd-plugin@claude-community` to install the plugin from the marketplace

## Project structure

```
cxgrd-plugin/
├── .claude-plugin/marketplace.json
└── plugins/cxgrd/
    ├── .claude-plugin/plugin.json
    └── skills/
        ├── scan/SKILL.md
        ├── blast-radius/SKILL.md
        └── check/SKILL.md
```

Agents use `--json` flag with `scan`, `input` and `check` commands to read the output in json format. 

To manually see the json output, 

```
cxgrd scan --json 
cxgrd input "<change description>" --json
```

