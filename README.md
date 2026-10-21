# linkedin-skills

Claude skills for writing LinkedIn posts.

## Install

```bash
git clone https://github.com/calebvergene/linkedin-skills.git
mkdir -p ~/.claude/skills
cp -R linkedin-skills/linkedin-post ~/.claude/skills/
```

For claude.ai, zip the `linkedin-post` folder and upload it under Settings → Capabilities → Skills.

## Usage

Run `/linkedin-post` in Claude Code, or just ask for a LinkedIn post:

```
/linkedin-post case study on how we grew a dev-tools founder from 0 to 18 inbound demos/month in 90 days
```

```
Write a lead magnet LinkedIn post for my cold email swipe file. Audience: agency owners.
```

### Formats

| Format | Structure |
|---|---|
| Lead magnet | Bold hook, problem, bullet preview of the resource, social proof, `Comment 'WORD'` CTA, repost bonus |
| Case study | "X days ago / Today" contrast, `→` results, how it was done, the takeaway, soft CTA |
| Educational | Clear promise, 5–7 numbered points (insight + how to apply), CTA |
| Viral lead magnet | Big breakdown teaser, what's inside, recognizable names, triple CTA, bonus |

Inputs: topic (required), plus optional result/metric, timeframe, target audience, and context. Numbers you don't provide come back as `[placeholders]`, never invented.

Output is plain text ready to paste into LinkedIn. Example posts for each format are in [linkedin-post/references/examples.md](linkedin-post/references/examples.md).
