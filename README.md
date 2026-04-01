# Dragon Dreaming Wisdom in Claude Code

An AI facilitator for the [Dragon Dreaming](https://dragondreaming.org) project methodology, built as a [Claude Code](https://claude.ai/code) skill.

Dragon Dreaming is an open-source project methodology rooted in wisdom from Aboriginal Australian culture — one of the oldest living cultures on Earth (~60,000 years). **John Croft and Vivienne Elanta** bridged this ancient wisdom into a modern framework, drawing from the Mandjilidjara Martu and Whadjuk Noongar peoples of Western Australia. Used in 56+ countries since the 1990s.

## Why This Skill?

There's a familiar pattern in projects: jumping from idea to execution, skipping the dream, never pausing to reflect on what was learned. Dragon Dreaming offers a different way — giving each phase of a project the same weight, guided by an AI facilitator.

```
        DREAMING
       /         \
CELEBRATING    PLANNING
       \         /
         DOING
```

The cycle is circular, not linear. You can move backward at any time — and that's healthy.

**What this skill does:**
- Detects which phase your project is in
- Behaves differently per phase (listens in Dreaming, structures in Planning, coaches in Doing, facilitates in Celebrating)
- Guides you through Dream Circles, Karabirrdt planning, and celebration processes
- Prevents the most common mistake: skipping phases

**What makes it different from a checklist:**
- It's a *facilitator*, not a task manager. In Dreaming, it will refuse to plan. In Planning, it will test your commitment. In Celebrating, it won't let you rush.
- It uses the original Dragon Dreaming tools and language (Pinakarri, Karabirrdt, Song Lines, Dream Circle) — and explains them as you go.

## Requirements

- [Claude Code](https://claude.ai/code) (any plan — free or paid)
- No additional dependencies, packages, or API keys needed

## Install

Copy the skill folder to your Claude Code skills directory:

```bash
# Clone this repo
git clone https://github.com/Jokerclues/dragon-dreaming-wisdom.git

# Copy the skill
cp -r dragon-dreaming-wisdom/dragon-dreaming-wisdom ~/.claude/skills/

# That's it. Start Claude Code and say "dragon dreaming" or "new project".
```

Or symlink if you want to stay synced with updates:

```bash
ln -s "$(pwd)/dragon-dreaming-wisdom/dragon-dreaming-wisdom" ~/.claude/skills/dragon-dreaming-wisdom
```

**Note on state:** The skill operates within your conversation context. It does not persist project state between sessions. For multi-session projects, it will ask you where you left off and which phase you're in. You can connect it to your own project tracking (Notion, Linear, markdown files — whatever you use).

## Usage

Once installed, Claude Code will automatically recognize Dragon Dreaming triggers:

| What you say | What happens |
|---|---|
| "I have a new project idea" | Enters **Dreaming** — asks generative questions, collects your dreams |
| "Let's plan this out" | Enters **Planning** — builds a Karabirrdt (spider web) with milestones and dependencies |
| "I'm working on X but stuck" | Enters **Doing** — coaches you, checks alignment with the dream |
| "We finished the milestone" | Enters **Celebrating** — gratitude, lessons learned, next dream |
| "What phase am I in?" | **Phase check** — identifies where you are and suggests next steps |

### Example: Starting a New Project

```
You: I want to build a CLI tool that helps people journal daily.

Claude: [Enters DREAMING mode]
"What would this project have to be like for you to say
it was the best use of your time?"

You: I want it to feel effortless. Like talking to a friend.
     And I want it to work offline.

Claude: [Records dreams, asks for more, doesn't evaluate]
"Those are two strong dreams. What else? Take your time."

You: That's it for now.

Claude: [Reads dreams back as completed story]
"You built a CLI journaling tool that felt effortless — like
talking to a friend. It worked fully offline. Ready to move
to Planning?"
```

### Key Dragon Dreaming Concepts

| Concept | What it means |
|---|---|
| **Pinakarri** | Deep listening. No planning your response while someone speaks. Claude will call "Pinakarri" if things get scattered. |
| **Dream Circle** | A structured process for sharing visions without judgment. One speaker at a time. All ideas welcome. |
| **Karabirrdt** | "Spider Web" — a visual planning tool. Goal in center, milestones as nodes, dependencies as Song Lines connecting them. |
| **Song Lines** | The paths along which information, resources, and decisions flow between tasks. Named after Aboriginal songlines. |
| **The Dragon** | Fears and obstacles are teachers, not enemies. Every block carries a lesson. |
| **Win-Win-Win** | Every project must serve: (1) your growth, (2) your community, (3) the Earth and greater good. |
| **100% Identification** | A task is only assigned if the owner fully identifies with it — not just commits, but sees it as theirs. |

## File Structure

```
dragon-dreaming-wisdom/                    # repo root (after git clone)
├── README.md                              # You are here
├── LICENSE                                # MIT
└── dragon-dreaming-wisdom/                # <- copy this folder to ~/.claude/skills/
    ├── SKILL.md                           # Main skill definition
    └── references/
        └── dd-methodology.md              # Deep methodology reference
```

## How It Compares

| | Dragon Dreaming | Agile/Scrum | Waterfall | Design Thinking |
|---|---|---|---|---|
| **Starts with** | Dream / vision | User stories | Requirements | Empathy |
| **Celebration** | 25% mandatory | Sprint retro | Post-project | Reflection |
| **Personal growth** | Core goal | Not addressed | Not addressed | Not addressed |
| **Flexibility** | Circular, go back anytime | Sprint-based | Linear | Iterative |
| **Obstacles** | Teachers (dragons) | Impediments | Risks | Constraints |
| **Success =** | Win-win-win | Velocity | On time/budget | User satisfaction |

## Customization

The skill works out of the box. If you want to adapt it:

- **Add your own project tracking**: The skill doesn't assume any specific tool (Notion, Linear, Jira). It suggests "update your project documentation" — connect it to whatever you use.
- **Team use**: The Dream Circle and Karabirrdt processes work for teams. Each person can run Claude Code and reference shared project state.
- **Language**: The skill adapts to whatever language you write in.

## Contributing

This is an open-source project and contributions are welcome. Dragon Dreaming has been improved by its community for 30+ years — this skill should grow the same way.

**Ways to contribute:**
- **Test it** — Use the skill on a real project and share what worked and what didn't
- **Improve facilitation** — If you're a DD practitioner and notice something that could be more faithful to the methodology, open a PR
- **Add translations** — The skill adapts to any language, but the reference documentation could be translated
- **Share your experience** — Open an issue with your story of using the skill

**Guidelines:**
- Respect the Dragon Dreaming methodology — changes should be faithful to John Croft and Vivienne Elanta's work
- Experience first, explain later — keep the facilitative, experiential approach
- Keep DD terms (Pinakarri, Karabirrdt, Song Lines) — they are the methodology's identity
- Test your changes on a real project before submitting

## Credits

- **Dragon Dreaming methodology**: [John Croft](https://dragondreaming.org) and Vivienne Elanta, Dragon Dreaming International
- **Skill development**: Eliyahu, [House of Clues](https://houseofclues.world)
- **Dragon Dreaming is open-source**: Free to use, share, and adapt under Creative Commons

## License

MIT License — see [LICENSE](LICENSE).

The Dragon Dreaming methodology itself is open-source under Creative Commons, maintained by Dragon Dreaming International.
