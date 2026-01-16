# WDP Server — Main Repository 🔧

[![Discord](https://img.shields.io/badge/Discord-Join-blue.svg)](https://discord.gg/A2vfymZwBE)  [![Open Issues](https://img.shields.io/github/issues/WDP-Server/WDP-Server)](https://github.com/WDP-Server/WDP-Server/issues)  

Welcome! This repository is the central home for the WDP Server project and links to the main modules. Use the Discord link above for real-time help, community discussion, and announcements.

---

## Quick: How to open a good Issue ✅

Please follow these steps to help us triage and fix things quickly:

1. Check existing issues using the Issues tab — your problem may already be reported or fixed.
2. Click **New issue** and choose a template (if available). If you don't see a template, use the format below.
3. Fill in the fields and attach logs, screenshots, or minimal reproduction steps.

Use this issue body template when reporting bugs or feature requests:

```markdown
**Title:** [bug] Short clear title here

**Summary**
A one-paragraph description of the problem or feature.

**Steps to reproduce**
1. Step one
2. Step two
3. Expected result vs actual result

**Environment**
- Server build: (e.g. paper-1.19.4 #123)
- WDP version: (git commit or release)
- Active plugins: (short list)

**Logs & Attachments**
- Paste relevant logs in triple backticks, or attach a file/gist

**Suggested labels:** bug, enhancement, question
```

> Tip: If your report includes logs, wrap them with triple backticks (```), and mark the approximate timestamps of the error.

---

## Main Repositories (short descriptions & links) 📚

| Repository | Purpose | Link |
|---|---|---|
| **WDP-BaseDet** | Base detection & automatic protection systems. Handles clustering, trust, and smart teleport fallbacks. | [./WDP-BaseDet](./WDP-BaseDet) |
| **WDP-Help** | AI-powered help system serving contextual, server-aware assistance. | [./WDP-Help](./WDP-Help) |
| **WDP-Progress** | Player progression, skills, and the Score system. Tracks equipment, stats, and multi-dimensional progress. | [./WDP-Progress](./WDP-Progress) |
| **WDP-Quest** | Progressive community quests and tiered reward system. Unlocks content as the server progresses. | [./WDP-Quest](./WDP-Quest) |
| **WDP-Start** | New-player onboarding and tutorial flow that gives starters rewards and guidance. | [./WDP-Start](./WDP-Start) |

> Each of the above modules contains a `FEATURES_SUMMARY.md` and `README.md` with more details. Visit them for implementation specifics, commands, and admin controls.

---

## Feature Summary — A Second README (📘)

This repository has a dedicated `FEATURES_SUMMARY.md` that acts as a full secondary README showcasing features, commands, mechanics, and design rationale.

- Quick link: [View the full Feature Summary](./FEATURES_SUMMARY.md)
- Highlights (excerpt):
  - Intelligent Base Detection & Protection
  - AuraSkills RPG progression and abilities
  - Progressive Quest system (250 quests)
  - Rogue Wanderer world events and exclusive rewards
  - Secure death recovery (graves) and teleport network

<details>
<summary><strong>Expand: Example Feature Highlights</strong></summary>

- Teleportation fallback order: `/sethome` → bed → base center → spiral search
- Skill categories: Mining, Combat, Farming, Foraging, Fishing, Enchanting
- Quest tiers: Beginner → Expert (50 quests per tier)
- AI Help relevance scoring and server-specific context

</details>

---

## Contributing & PRs ✨

- Fork the repo, create a topic branch, and send a PR with a clear description and link to any open issue.
- Use descriptive commit messages and keep PRs scoped.

Suggested PR checklist:
- [ ] Tests or manual verification added
- [ ] Changelog entry (if applicable)
- [ ] Linked to an Issue (bug/feature)

---

## Support & Contact

- Discord: [Join the community](https://discord.gg/REPLACE-WITH-YOUR-INVITE) — best for live help and announcements.
- Issues: Use the GitHub Issues tab for reproducible bugs and feature requests.

---

## License & Notes

See individual module `README.md` files for licensing and deployment notes. If you're setting up a local environment, check each subproject's `deploy.sh` or `pom.xml` where applicable.

---

> Made with ❤️ — keep docs tidy, issues reproducible, and the community helpful.
