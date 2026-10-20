# security-skills

A collection of Claude Code skills for code security review.

## How to install a skill

Copy the skill directory into your Claude skills folder:

```bash
# macOS / Linux
cp -r <skill-name> ~/.claude/skills/

# Example
cp -r cwe-security-check ~/.claude/skills/
```

After copying, the skill is immediately available in any Claude Code session — no restart needed.

## Available skills

### `cwe-security-check`

基于 CWE-699（软件开发视图，CWE 4.19.1）的代码安全审查技能。

Covers:
- 40 CWE-699 weakness categories as a review checklist (full catalog in `references/cwe-699-catalog.md`)
- Review scope: files / diff / PR / whole repository
- Prioritized scanning: injection, input validation, authN/authZ, crypto, memory, concurrency, deserialization, secrets
- Exploitability verification via data-flow tracing (source → sink)
- Findings mapped to specific CWE-IDs with file/line, severity-ordered report and fix suggestions

**Trigger keywords:** CWE, CWE-699, 安全检查, 安全审查, 安全审计, security review, security audit, 漏洞, injection, XSS, SQL 注入, 认证, 授权, 加密, race condition, 反序列化, 敏感信息, 硬编码密钥

**Usage:** mention any trigger keyword or type `/cwe-security-check` in the prompt.

---

## Contributing

1. Create a directory named after your skill
2. Add a `SKILL.md` with the required frontmatter:

```markdown
---
name: your-skill-name
description: one-line description used for trigger matching
---

# Skill content here
```

3. Submit a PR.
