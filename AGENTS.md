# AGENTS.md — llms-generator

Machine-readable entry for AI agents.

## Purpose
One command to become AI-discoverable: llms.txt + ecosystem links.

## Invocation
```bash
python scripts/llms_gen.py --name MyProject --url https://github.com/org/repo --desc "..." [--link ...] [--full README.md]
```

## Output contract
- Writes `llms.txt` (LLMs.txt v2 spec) with ecosystem links.
- `--full` inlines markdown content.

## Rules
- Never publishes to remote; writes local file only.
- No placeholders in outputs.

## Skill Marketplace
- lgd-skill-marketplace: https://github.com/zhaoxinghua09-cell/lgd-skill-marketplace — full skill catalog (enter from any skill).
