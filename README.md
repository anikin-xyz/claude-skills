# Claude Skills for Development Work

A collection Claude skills designed to improve collaboration, documentation, and workflow management.

## Skills Included

### 1. brainstorm-partner
Collaborative brainstorming sessions with structured dialogue and strategic questioning.

**Use when:** You need an equal thinking partner for ideation or an extension of mind so to speak  

Key features:
- Numbered responses for easy reference
- Strategic questions (open-ended, context-based, motivation-probing)
- 2-4 solution alternatives when proposing ideas
- Constructive disagreement with reasoning
- Session summary documents on completion

**Triggers:** "I want to brainstorm," "Let's brainstorm about [topic]"

---

### 2. dev-cleanup-tracker
Track and manage cleanup of failed technical attempts, unused packages, and configuration changes.

**Use when:** Changing approaches mid-troubleshooting, ending work sessions, or after failed setups  
Key features:
- Monitors packages, files, configs created during troubleshooting
- Asks permission before cleanup (never automatic)
- Provides exact removal commands
- Suggests verification steps

**Triggers:** "Should we clean up?", "What needs cleanup?", "Remove leftovers"

---

### 3. dev-collaborative-assistant
Collaborative technical decision-making with state verification and option presentation.

**Use when:** Making system changes, configuring services, troubleshooting, or choosing implementation approaches  
Key features:
- Verifies actual state before proceeding (never assumes)
- Presents multiple approaches with trade-offs
- Security awareness for credentials and permissions
- Contextual confirmation tracking

**Triggers:** "Configure," "Set up," "Which approach?", "Verify," "Check if working"

---

### 4. dev-doc-generator
Generate formatted session documentation for completed technical work.

**Use when:** You need documentation of configuration changes, troubleshooting, or system setup  
Key features:
- Date-prefixed filenames (yyyy.mm.dd-name.md)
- Proper metadata and version tracking
- Security compliance (no credentials in docs)
- Follows your documentation-standards.md if provided
- Asks where to save documentation

**Triggers:** "Document this session," "Create documentation," "Write up what we did"

## Installation

### For claude.ai or Claude Desktop:
1. Download the .skill file you want
2. Go to Settings → Capabilities → Skills
3. Click "Upload skill"
4. Select the downloaded .skill file

### For Claude Code (CLI):
1. Extract the skill folder from the .skill file (it's just a zip)
2. Copy to `~/.claude/skills/`
3. Or add to your project at `.claude/skills/`

### For Other LLMs (Gemini, etc.):
1. Upload the .skill file at the start of your conversation
2. If that doesn't work, unzip it and upload the SKILL.md file instead
3. The AI will follow the instructions defined in the skill

## Customization

### dev-doc-generator
If you want automatic save paths, create a `documentation-standards.md` file defining your conventions. The skill will follow it. Otherwise, it asks where to save each time.

### All Skills
All skills are designed to adapt to your environment. They'll ask clarifying questions when needed rather than making assumptions.

## Version
All skills: v1.01

## License
MIT - Use these however you want
