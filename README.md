# Typst Homework Setup
This provides a simple way to interface your AI assistants with neat math homework, with guardrails so the assistant helps you learn instead of doing the homework for you.

This repository includes:
- `template.typ` - a template to nicely format homework. 
  - Feel free to switch to a different typst template: [typst.app/universe/search/?kind=templates](https://typst.app/universe/search/?kind=templates)
- `examplehw/` - an example assignment (`example.typ` + compiled `example.pdf`) showing how to use the template
- `AGENTS.md` - file that prompts AI assistants with the course's AI-use policy
- `.gitignore` - allowlists only the files above, so per-assignment work never accidentally gets committed here

# File organization
Each assignment gets its own folder, created locally (not part of this public scaffold):

```
hw1/
  pset.pdf        - the assignment as given by the course
  hw1.typ         - your Typst source, importing ../template.typ
  submission.pdf  - compiled output you turn in
```

General, not-assignment-specific scratch work (e.g. `tmp.typ`) can live at the repo root.

# Using this for your own class
This repo is a **GitHub Template Repository**, so to use it for your own coursework: click "Use this template" (not "Fork") at the top of the repo. That creates a new, unconnected copy under your own account with no visible link back here — set it to **private** when you create it, since your psets, submissions, and source will live there.

Once you have your own private copy:
- Edit `AGENTS.md` to match your own course's actual AI-use policy. The one here is just a starting point.
- Create an `hwN/` folder per assignment and drop in `pset.pdf`, `hwN.typ`, and `submission.pdf` as you go. 
- Update `.gitignore` to only track the files you want.
