# linkedin-skills

Claude skills for writing LinkedIn posts, one per post format.

## Install

```bash
git clone https://github.com/calebvergene/linkedin-skills.git
mkdir -p ~/.claude/skills
cp -R linkedin-skills/linkedin-* ~/.claude/skills/
```

For claude.ai, zip each skill folder and upload it under Settings → Capabilities → Skills.

## Skills

| Skill | Structure |
|---|---|
| `linkedin-lead-magnet` | Bold hook, problem, bullet preview of the resource, social proof, `Comment 'WORD'` CTA, repost bonus |
| `linkedin-case-study` | "X days ago / Today" contrast, `→` results, how it was done, the takeaway, soft CTA |
| `linkedin-educational` | Clear promise, 5–7 numbered points (insight + how to apply), CTA |
| `linkedin-viral-lead-magnet` | Big breakdown teaser, what's inside, recognizable names, triple CTA, bonus |
| `linkedin-resource` | Credibility hook with big names, the whole roadmap in 2–3 bold-header sections, objection, recap line, "drop your email" for the full guide |

Inputs: topic (required), plus optional target audience and context. Case study, viral lead magnet and resource also take a result and timeframe. Resource also needs the guide you'll send. Numbers you don't provide come back as `[placeholders]`, never invented.

Output is plain text ready to paste into LinkedIn. Each skill ends with an example post.

## Usage

```
/linkedin-case-study how we grew a dev-tools founder from 0 to 18 inbound demos/month in 90 days
```

```
/linkedin-lead-magnet my cold email swipe file, audience: agency owners
```

Or just describe the post you want and the matching skill will trigger.
