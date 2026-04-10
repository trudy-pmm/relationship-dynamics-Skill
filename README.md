# Claude Code Skills

A collection of custom skills for [Claude Code](https://claude.com/claude-code).

## Skills

### /relationship-dynamics

Analyze power structures, dependency patterns, and information asymmetry in any relationship (intimate, workplace, social).

Inspired by the TV drama《危险关系》(2026), this skill examines relationships from five dimensions:

1. **Power Geography** — who holds what power, and how it flows
2. **Exchange Structure** — what each person gives and gets, where the asymmetry lies
3. **Attachment Currents** — unspoken needs and fears, and the dance patterns they create
4. **Information Landscape** — what each person sees, what they're blind to
5. **The Arc** — trajectory, inflection points, and growth edges

### /create-website

Scaffold and build a personal website project with dark mode support. Guides you through choosing a tech stack, creating pages, and deploying.

## Installation

Copy the skill folders into your Claude Code skills directory:

```bash
# Personal (available in all projects)
cp -r relationship-dynamics ~/.claude/skills/
cp -r create-website ~/.claude/skills/
```

Then use in Claude Code:

```
/relationship-dynamics describe a relationship or paste a conversation
/create-website my-site
```

## License

MIT
