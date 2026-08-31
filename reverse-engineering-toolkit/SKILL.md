---
name: reverse-engineering-toolkit
description: >-
  Authorized reverse-engineering toolkit for analyzing user-provided binaries,
  malware samples, CTF challenges, software protection, obfuscation, packing,
  anti-debugging, custom bytecode, and .NET applications. Use for static and
  dynamic analysis, debugging, deobfuscation, unpacking, and defensive audits.
---

# Reverse Engineering Toolkit

Use this skill only for software the user owns or is authorized to analyze, CTF challenges, sandbox samples, and defensive security research.

## Routing

- Start with `04-upx-unpacking-analysis.md` for packed samples and UPX.
- Use `03-anti-debugging-analysis.md` for debugger detection and analysis blockers.
- Use `02-vm-bytecode-reverse-engineering.md` for custom VMs and bytecode.
- Use `01-code-obfuscation-deobfuscation.md` for control-flow and string obfuscation.
- Use `07-dotnet-reverse-engineering.md` for managed .NET binaries.
- Use `05-general-reverse-engineering.md` for general triage and tool selection.
- Use `06-binary-mitigations-ctf.md` for CTF and defensive ELF mitigation analysis.

## Operating rules

1. Establish authorization and scope before analyzing a real target.
2. Prefer the user's supplied files and an isolated lab environment.
3. Preserve originals, hash inputs and outputs, and keep changes reproducible.
4. Report evidence, assumptions, and verification steps separately.
5. Do not provide credential theft, unauthorized access, license circumvention, or malware deployment instructions.

The numbered Markdown files are reference playbooks. This file is the loadable skill entry point.
