# CBT Emotion Log · an Agent Skill

A little companion that keeps a **CBT thought record** for you — just by talking. When something upsets you, tell your agent the way you would tell a friend. It answers you first, then quietly writes the event down: what actually happened, what you thought, how you felt, and what you are worried will happen next. Later it helps you look back.

The skill itself speaks Chinese (中文), the language it was written for.

- **In the moment, in your own words.** No form to fill in. It keeps your original words and never invents a score for you; it asks at most one question, and only when the next step depends on it.
- **Support first.** It responds to the person before the record. If you only want to vent, the record is kept in the background.
- **Facts apart from thoughts.** "He hasn't replied for two hours" and "he must be unhappy with me" are kept apart, so you can see which is which later.
- **Worries checked against what happened.** A worry becomes a prediction with a deadline; when the time comes it is settled honestly — happened, partly, didn't happen, or not enough information — so you can see how often your fears came true.
- **Other angles, and the good parts.** When you are going round in circles on the same worry with no new facts, it puts the facts you already confirmed in front of you, and helps you look for other explanations and the parts of an event that went well.
- **Good moments kept too.** Happy and precious moments are recorded in their own right, and can be brought back on a low day — without forcing positivity.
- **Stats when you ask.** "How many of my worries actually happened?", "what keeps making me angry?", weekly or monthly reviews — with sample sizes and no diagnoses.

## Install

Pick one:

```bash
npx skills add advnljs/cbt-emotion-log-skill   # skills.sh: choose the agents to install it for (Codex, Claude Code, OpenClaw, …)
```

```bash
clawhub install cbt-emotion-log                 # ClawHub (OpenClaw)
```

```bash
npx cbt-emotion-log              # copies it to ~/.claude/skills/cbt-emotion-log (Claude Code, all projects)
npx cbt-emotion-log --dir <path> # or into any agent's skills folder
```

Or download `cbt-emotion-log.zip` from the [latest release](https://github.com/advnljs/cbt-emotion-log-skill/releases/latest) and import it in any agent that lets you upload or add a skill (for example WorkBuddy's skills page).

Then start a new session and just talk, for example: 「刚把方案发给领导，两个小时了没回，焦虑死了。」

## Where your records live

Records are kept in a file you choose (by default `emotion_log.json`) or another storage you authorize, so the next conversation can read them. Nothing in the skill uploads your records anywhere; it reuses the place you agreed on and never shares personal logs when the skill itself is shared.

## Please note

This is a journaling companion based on the thought record of cognitive behavioural therapy (CBT). It does not diagnose and is not a substitute for professional help. If you are thinking about hurting yourself or someone else, please reach out to someone you trust, a professional, or your local crisis line now.

## License

[MIT-0](LICENSE)
