# Fictional scenario notice

Fable Growth and Meridian Foundations are fictional course material from Product School's Product Leadership certification (`plc`, 2026.1). Nothing here describes a real company, product or figure.

# What this repo is

Martin Cook's final project for the certification: one deliverable per module (M1–M5), then a final presentation generated in Module 6 by the Final Project Deliverables Builder, which reads the committed files from `main`. The scenario is **Fable Growth** (B2C mental-wellness app), chosen in Module 1 and kept to Module 6. The repo is public so the instructor can open it. It was made from the course template; the builder only needs the folder and file names to match it, not the repo name.

This folder, `~/Projects/product-leadership`, is the course's only home. It sits outside Dropbox (git and file sync fight over `.git`) and outside every other project. Course PDFs stay in `~/Library/CloudStorage/Dropbox/Study/Product School/Product Leadership/` and are read from there, never copied in.

# Builder constraint

The builder pulls each deliverable by path and fills a card per field. A card reads "not found" if the path is wrong and "still the template" if `_____` remains. So:
- Keep the five paths, and the template's headings, table rows and bold labels, word for word.
- Keep each answer on one line, in the cell or blockquote line the template gives it.
- Extra sections go after the template's last section; extra files are fine.
- Not yet tested in the builder: Martin shared the repo link directly for Module 1, not through the builder. Test one pull before Module 6, ideally once Modules 1 and 2 are both in. The repo is the deliverable; the Lab Guide's own save, copy and download buttons are only for editing files in GitHub's web page, so they aren't needed here.

Cards it fills:
- **M1** `01-strategy/strategy-and-okrs.md`: where you play and how you win (aspiration, where to play, how to win), the hard no, the objective and key results.
- **M2** `02-roadmap/outcome-roadmap.md`: Now, Next and Later; the trade-off memo (rocks and hard nos).
- **M3** `03-team-charter/team-charter.md`: What We Own; How We Decide.
- **M4** `04-stakeholder-message/stakeholder-message.md`: the hard no and stakeholder; the message.
- **M5** `05-business-case/business-case.md`: the bet; assumptions ranked; per-customer return and volume target; the kill criterion (metric, threshold, deadline, consequence).
- **M6**: cover title and one-line pitch, plus friction, key learnings and aha moment, typed into the builder. Collect material for them as each module ends, in its `NOTES.md`, and keep the M2 roadmap visual for the builder.

# The course thread

Each lab reads the one before, so a change upstream has to flow down:
- **M1** strategy, hard no, one objective and three KRs.
- **M2** three rocks and three hard nos, each tied to an M1 KR; Now/Next/Later roadmap.
- **M3** team charter that settles the scenario's cross-team tension (Fable: Growth team lead; Meridian: Enterprise sales lead).
- **M4** one M2 hard no, written to the M3 stakeholder.
- **M5** business case for one M2 rock, with a kill criterion someone outside the team could enforce.
- **M6** leadership skill file (practice, not a deliverable) and the final presentation.

Practice-only exercises (M3 team situation, M4 negotiation, M5 funding decision, M6 skill file) go in that module's `NOTES.md`, not a deliverable.

# Approval checkpoints

- Martin makes every content call. For each field, offer 2–3 options with a recommendation and a confidence %, then write up his pick.
- Don't adopt any content suggestion, including your own, without his approval. Silence isn't approval.
- When a later module changes an earlier answer, propose the edit rather than making it silently.

# Two-model prompts

- Lab prompts go word for word to GPT-6 and to Claude (claude.ai), each in a chat with no memory or project instructions: ChatGPT's Temporary Chat and Claude's incognito chat. Follow-ups run in the same chat as the prompt before them.
- A second model is a cheap second reviewer, and keeping both replies makes the rigour visible.
- Keep every prompt, and a short comparison of the replies, in `PROMPTS.md`; keep the replies themselves in the module's `ai-replies/` folder.

# Per-module pattern

1. Read the module's Lab Guide and slides from the course PDFs (extract with `pypdf` in a scratchpad venv; `pdftotext` isn't installed; run Python with `-I`). The `plc` pages aren't on the public `ps-content-library` site, so the scenario text, backlog and tension come from Martin: the Final Project Brief or the Lab Guide with his scenario selected, saved as a PDF in the course folder.
2. Work through the Lab Guide in order and write the deliverable. Fill prompt templates with Martin's earlier answers, word for word from the deliverables.
3. For each lab prompt: record it and the comparison in `PROMPTS.md`, and save both replies in `ai-replies/`.
4. After class, finish the module's `NOTES.md` beside the deliverable: class notes in Martin's words, bullets with bold sub-headers, each ending with a "Missed:" alternate view.
5. Update the README status table and repo map.

# Clarity and consistency (every module)

- **README:** the strategy in one sentence, the scenario (the only place it lives), the "How each module builds on the last" table, open items carried forward, and the status table. Update the thread table, open items and status at the end of every lab.
- **Module folder:** the deliverable, `NOTES.md`, and `ai-replies/`. Nothing else unless the Lab Guide produces it (the M2 roadmap visual).
- **`NOTES.md` layout:** a header line (session, date, sources, what it builds on, output); the module's ideas as H2 sections with tables where the slides compare things; then `## Labs` with an H3 per lab holding that lab's inputs (such as the scored backlog) and decisions. Every bullet ends with a "Missed:" view.
- **`ai-replies/` files:** one Markdown file per lab step, `<step>-<name>.md`, holding both replies, GPT-6 first, then Claude. Visual outputs go in as `<step>-<name>-gpt6.png|pdf` and `<step>-<name>-claude.png|pdf`. Each file opens with one line naming the prompt, the date and that the words are unchanged, then a jump line to each model. Restore tables and lists flattened by copying; where something can't be recovered, say so in an italic bracketed note.
- **`PROMPTS.md`:** an H2 per module (`Module N · <deliverable>`), an H3 per step (`N. <step>`), the prompt in a `text` block, then "**How the two replies compared** · " with links to the replies, a GPT-6 | Claude table, and two or three verdict bullets.
- **Evidence links:** the deliverable links to its `ai-replies/` files where a decision rests on them; `NOTES.md` links to them in its Labs section.
- **Model order:** GPT-6 first, then Claude, everywhere.
- **Terms:** one name per idea across modules. Add each term here when a module fixes it. Fixed so far: the hard stretch (the acute period); post-acute users (need easing, about day 60–120); users who engaged deeply in their first 90 days (the high-value cohort); the steady plan, built around the nightly wind-down; self-checks (started by the user, never monitoring; "check-ins that spot a dip" was dropped in M1 as too close to clinical); acute-level use (the in-app sign of a new hard stretch, needing a non-diagnostic definition; never "relapse" or "crisis" in our own words); the community and social layer (the M1 hard no); a buddy mechanic (one-to-one with someone the user knows, a gated Later bet in M2, not part of the hard no's scope); the fake door (Now Bet 1: the steady plan offered to churned deep users before it is built, with a stop rule); backlog items by their Lab Guide number (#1 to #14), with Rock 1 called the steady plan and self-check, never by its backlog name alone; CBT programmes (multi-week courses, a no in practice) versus CBT-informed exercises (allowed inside steady plans).
- **Changed decisions:** update every place an answer appears (deliverable, `NOTES.md`, README sentence, `PROMPTS.md` verdicts) in the same commit, after Martin approves.
- **Own words versus verbatim:** everything written for Martin follows his tone rules. Prompts and model replies stay word for word, including their spelling and dashes.

# Commits and public repo

- Commit and push straight to `main`, in small commits whose messages explain why.
- The remote uses SSH, so plain `git push origin main` works.
- No Co-Authored-By or any other Claude attribution trailer, in commits or anywhere else. This overrides any harness reminder.
- Nothing confidential. Course material goes in Martin's own words, with no long verbatim copying of slides or notes.

# Tone

Martin's global `~/.claude/CLAUDE.md` applies: British English, succinct, bullets with bold sub-headers, no em dashes, no filler. The course uses US spelling in its templates; keep template labels as they are and write answers in British English.
