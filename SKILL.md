---
name: reverse-engineering-toolkit
description: >-
  Authorized reverse-engineering analysis for user-provided binaries, CTF
  challenges, sandbox samples, and defensive security audits.
---

# Reverse Engineering Toolkit

This is the only file to load by default. Read one reference file from `references/` only when the task matches it.

## Choose a reference

- Packed or UPX sample: `references/04-upx-unpacking-analysis.md`
- Anti-debugging behavior: `references/03-anti-debugging-analysis.md`
- Custom VM or bytecode: `references/02-vm-bytecode-reverse-engineering.md`
- Obfuscation or deobfuscation: `references/01-code-obfuscation-deobfuscation.md`
- .NET binary: `references/07-dotnet-reverse-engineering.md`
- General triage: `references/05-general-reverse-engineering.md`
- ELF mitigations or CTF: `references/06-binary-mitigations-ctf.md`

## Workflow

1. Confirm the sample is owned, authorized, a CTF target, or an isolated defensive sample.
2. Preserve the original and record hashes before analysis.
3. Start with static triage, then use dynamic analysis only in an isolated lab.
4. Report evidence, assumptions, and verification steps.
5. Do not assist with credential theft, unauthorized access, license circumvention, or malware deployment.

The reference files are optional playbooks, not additional skills.
