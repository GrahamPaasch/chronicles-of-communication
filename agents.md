# AI Agent Templates

This document outlines prompt patterns for using OpenAI Codex to automate VR development tasks in this repository.

## Generate VR environment code

Prompt:
```
Generate VR environment code using the provided 3D scan data and historical references.

Input folders:
- assets/models/*
- docs/reference-links.md
```

Output path: `scenes/` with a new scene file per exhibit.

## Create interaction scripts

Prompt:
```
Create interaction scripts that handle knob turns, patch-cord jacks and ringing logic.
Use provided scene file and user input events.
```

Output path: `scripts/` with one script per interactive element.

## Build asset pipeline scripts

Prompt:
```
Build automation scripts for retopology and texture baking of new 3D scans.
```

Output path: `scripts/pipeline/`.

## Example Codex invocations

```bash
# Generate environment code
openai api completions.create -m codex -p "Generate VR environment code" -f assets/models/panel-switch.obj

# Create interaction script
openai api completions.create -m codex -p "Create interaction scripts" -f scenes/panel-switch.scene

# Build asset pipeline
openai api completions.create -m codex -p "Build asset pipeline scripts" -f assets/models/panel-switch.obj
```
