# How to install the prompt-architect skill

A skill is a small folder with one instruction file inside. Claude loads it when you say the right words. You install it once.

The skill is the folder `skill/prompt-architect/`. It has one file in it: `SKILL.md`.

Menus move around as Claude gets updates. If a button isn't where these steps say, look for the word "Skills" in Settings.

## Claude.ai (the website or the desktop app)

1. Zip the `prompt-architect` folder. On a Mac, right-click the folder and choose Compress. On Windows, right-click, then Send to, then Compressed folder.
2. In Claude, open Settings.
3. Find Skills. It's usually under Capabilities. If you don't see it, check that code execution and file creation are turned on, and that your plan includes skills.
4. Choose to upload a skill and pick `prompt-architect.zip`.
5. Make sure the skill is switched on.
6. Open a new chat and type: `architect a prompt`. If Claude asks what job you want done, it's working.

## Claude Cowork

1. Open the Claude desktop app and go to Settings, then Skills.
2. Upload `prompt-architect.zip` the same way as above, and switch it on.
3. Start a Cowork task and type: `architect a prompt`.

## Claude Code

1. Copy the `prompt-architect` folder into the skills folder in your home directory. Run this from inside the download folder. It doesn't overwrite anything that's already there:

```
mkdir -p ~/.claude/skills && cp -Rn skill/prompt-architect ~/.claude/skills/
```

2. To use it in only one project, copy it into that project's `.claude/skills/` folder the same way.
3. Start Claude Code and type: `architect a prompt`.

## ChatGPT, or a Claude plan without skills

1. Open `skill/prompt-architect/SKILL.md` in any text editor.
2. Copy everything below the second `---` line.
3. Paste it as your first message in a new chat, then add: "Follow these instructions. Start the interview."

You can also skip the skill and paste `templates/05-interview-me.md`. It's the short version.

## Check that it works

It's working when the AI asks you ONE question, waits, and then asks the next. If it asks 9 questions at once, say: "One question at a time, please."
