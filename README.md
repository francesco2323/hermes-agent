# Hermes Agent

Hermes Agent is a structured AI-agent workspace focused on cloud and platform architecture.
It combines one core identity (`SOUL.md`) with multiple specialist skill profiles under `skills/`.

## What this repository contains

- `SOUL.md` – core identity, principles, and decision framework.
- `AGENTS.md` – operating rules and response behavior.
- `config.yaml` – runtime configuration for personality, paths, behavior, and security defaults.
- `skills/` – role-specific skills (AWS, Terraform, DevSecOps, Kubernetes, Identity, Observability, Migration, Executive).
- `memories/` – long-term and user-context memory files.
- `hooks/` – pre-run, post-run, and error hook locations.
- `plugins/` – plugin folders for observability, security, and productivity extensions.
- `skins/` – output/theme presets.
- `sessions/` – session state data.
- `cron/` – scheduled job definitions and outputs.
- `logs/` – runtime logs.

## Default behavior

From `config.yaml`, Hermes is configured to:

- use `aws-architect` as the default personality,
- prefer concise, structured, actionable responses,
- keep conversation context bounded and summarize old sessions,
- remember user preferences,
- enforce security defaults such as secret redaction and explicit confirmation for dangerous actions.

## Purpose

This setup is designed for production-aware architecture guidance across AWS, Terraform, Kubernetes, identity/federation, DevSecOps, observability, and GitHub automation workflows.
