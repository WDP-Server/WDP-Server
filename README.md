<p>
  <a href="https://github.com/WDP-Server" target="_blank" rel="noopener noreferrer">
    <img src="assets/logo-scoreboard-cropped.png" alt="WDP Server" width="255" style="max-width:100%;height:auto;display:block;margin:0 auto;image-rendering:pixelated;">
    <h1 style="text-align: center;">Main Repository</h1>
  </a>
</p>

[![Discord](https://img.shields.io/badge/Discord-Join-blue.svg)](https://discord.gg/A2vfymZwBE)  [![Open Issues](https://img.shields.io/github/issues/WDP-Server/WDP-Server)](https://github.com/WDP-Server/WDP-Server/issues)  


Welcome! This repository is the central home for the WDP Server project and links to the main modules. Use the Discord link above for real-time help, community discussion, and announcements.

---

## How to play 🖥️
- **Server IP:** `play.wdpserver.com`
- **Compatibility:** All client versions are supported — join with any release.
- **Voice chat:** Built-in voice chat is available in-game.

## How YOU Can Report Bugs or Suggest Features 🎮

If you encounter a bug while playing or have a cool idea for a new feature, we'd love to hear from you! Reporting helps us make the server better for everyone.

Please follow these simple steps:

1. Check the [Issues tab](https://github.com/WDP-Server/WDP-Server/issues) — someone might have already reported your issue or idea.
2. Click **New issue** and use the template below to describe what you found.
3. Be as detailed as possible, and attach screenshots or videos if you can!

Use this template for your report:

```markdown
**Title:** [Bug] or [Feature] Short and clear title

**What happened?**
Describe the bug you experienced or the feature you'd like to suggest. What were you doing when it happened?

**Steps to reproduce (for bugs only)**
1. Step one: What you did first
2. Step two: What happened next
3. And so on...

**What did you expect to happen?**
Explain what you thought should happen instead.

**Screenshots or videos**
Attach any images or clips that show the issue (drag and drop them here).

**Your Minecraft version**
What version of Minecraft are you using? (e.g., 1.20.1)

**Anything else?**
Any other details that might help, like when it happens or who else was affected.
```

> Tip: Screenshots are super helpful! Press F2 in Minecraft to take one, and it saves to your screenshots folder.

---

## Main Repositories (short descriptions & links) 📚

| Repository | Purpose | Link |
|---|---|---|
| **WDP-BaseDet** | Base detection & automatic protection systems. Handles clustering, trust, and smart teleport fallbacks. | <a href="https://github.com/WDP-Server/WDP-BaseDet" target="_blank" rel="noopener noreferrer">WDP-BaseDet</a> |
| **WDP-Help** | AI-powered help system serving contextual, server-aware assistance. | <a href="https://github.com/WDP-Server/WDP-Help" target="_blank" rel="noopener noreferrer">WDP-Help</a> |
| **WDP-Progress** | Player progression, skills, and the Score system. Tracks equipment, stats, and multi-dimensional progress. | <a href="https://github.com/WDP-Server/WDP-Progress" target="_blank" rel="noopener noreferrer">WDP-Progress</a> |
| **WDP-Quest** | Progressive community quests and tiered reward system. Unlocks content as the server progresses. | <a href="https://github.com/WDP-Server/WDP-Quest" target="_blank" rel="noopener noreferrer">WDP-Quest</a> |
| **WDP-Start** | New-player onboarding and tutorial flow that gives starters rewards and guidance. | <a href="https://github.com/WDP-Server/WDP-Start" target="_blank" rel="noopener noreferrer">WDP-Start</a> |

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
