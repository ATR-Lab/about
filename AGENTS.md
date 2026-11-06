# AGENTS.md: about

This repository is the public profile of the Advanced Telerobotics Research Laboratory (Department of Computer Science, Kent State University, GitHub org `ATR-Lab`): what the lab is, its research, its dated achievements, its publications, a press kit for media and its member list, including the GitHub issue form members use to submit their own profile. People (students, visitors, reporters, Kent State editors) and coding agents both read it. It is **not** the lab website ([www.atr.cs.kent.edu](https://www.atr.cs.kent.edu/)), not an onboarding or safety guide (that is `getting-started-atr-lab`) and not a place for unverified claims: every lab fact here must trace to the lab's verified fact base or a linked source.

## Repo map

| Path | What it is |
|---|---|
| `README.md` | Landing page: formal one-liner, card grid, at a glance, highlights, projects, programs, contact, repo map |
| `research.md` | Positioning (telepresence to Physical AI), four message pillars, current projects, platforms, past projects, programs, public code |
| `achievements.md` | Dated timeline with the allowed wording and a source per row; never-upgrade table; never-claim list; how to add a result |
| `publications.md` | VendoBot (HRI 2026), awarded papers, a selected IEEE-style list from the lab website, website-vs-publisher differences |
| `press-kit/README.md` | Media kit index: top line for media contact, checklist, what is still to be supplied, rules for users |
| `press-kit/boilerplates.md` | One-liners, 25-, 50- and 100-word versions, social bio, mission statement, each with approval status |
| `press-kit/fact-sheet.md` | Verified facts only, for reporters |
| `press-kit/director-bio.md` | 50-word director bio template (brackets stay until the director's approved CV fills them) |
| `press-kit/coverage-log.md` | Table template for media coverage |
| `press-kit/logos/README.md` | Logo usage note (clear space, minimum sizes, backgrounds, Kent State co-branding, never list) |
| `press-kit/logos/png/` | Six 3000 px PNG masters: horizontal navy and white, horizontal-short navy, stacked navy, mark navy and white |
| `press-kit/logos/svg/` | The same six logos as SVG |
| `press-kit/photos/README.md` | Photo and b-roll requirements, consent rules, photo log (no photos yet) |
| `members/README.md` | Director entry, current member and alumni tables, submit link, message to send, maintainer procedure, profile file format |
| `members/profiles/` | One approved profile per member, `<slug>.md` plus an optional `<slug>.jpg`; empty for now (`.gitkeep`) |
| `.github/ISSUE_TEMPLATE/member-profile.yml` | Issue form members use to submit a profile (label `member-profile`) |
| `.github/ISSUE_TEMPLATE/docs-fix.yml` | Issue form to report a wrong fact or broken link (label `bug`) |
| `.github/ISSUE_TEMPLATE/config.yml` | Template chooser: blank issues allowed, contact link to the lab website |
| `.github/workflows/docs.yml` | CI: markdownlint on every push and pull request; lychee checks local links on pull requests and every link after merge and weekly |
| `.github/assets/header.png`, `.github/assets/social-preview.png` | README banner and GitHub social preview (don't regenerate) |
| `.github/assets/icons/` | The six navy badge icons used by the README card grid |
| `.lycheeignore` | URL patterns the link checker skips (sites such as ACM that refuse automated requests; check those by hand) |
| `.markdownlint.jsonc` | markdownlint rules shared by the lab's docs repos |
| `.gitignore` | OS, editor and local-tool files |
| `AGENTS.md` | This file |
| `CLAUDE.md` | One line, `@AGENTS.md`, so Claude Code loads this file |
| `LICENSE` | MIT, 2017-2026; the lab's and Kent State's names and logos are excluded |

## Sources of truth

- **Lab facts** (names, director, projects, platforms, programs, results, contacts): only the ATR Lab design skill's `references/brand-foundation.md` (the "fact base"; verified Sept. 28, 2026), mainly §1 (the lab in one screen), §9 (proof bank: allowed wording) and §11 (verified contact block). The skill is public at [ATR-Lab/atr-lab-design-skill](https://github.com/ATR-Lab/atr-lab-design-skill).
- **Results:** copy the proof bank's allowed wording exactly. Keep every `[confirm]` bracket until the director confirms it.
- **Boilerplates:** `brand-foundation.md` §10 is canonical. Copy verbatim, keep the draft labels.
- **Publications:** the lab website's publications page for what is listed, and the DOI record (Crossref) for venue, pages and DOI. Only entries whose authors and title match the DOI record go in the selected list.
- **Repositories:** link only public `ATR-Lab` repositories, and only after reading their README. Check with `gh repo view ATR-Lab/<name> --json visibility`.
- **Kent State rules:** kent.edu pages linked where used (brand, photography, media relations).
- **Never invent** names, rooms, phone numbers, results, dates, versions, counts or quotes. Anything only the lab can supply stays a `[bracketed placeholder]` and is listed under [Open items](#open-items).
- **Never print:** the nonexistent X handle from the old template footer, the director's office room or phone as the lab's, the college's former name, "KSU" in running copy, "ATR" alone, any RoboCup placement, media-outlet counts for TeleBot, headcounts or the director's career totals as lab statistics.

## Writing rules

- Voice: precise, curious, hands-on, welcoming, grounded. Write for a smart first-year student; define jargon on first use (Physical AI = "AI that senses and acts in the real world through a robot").
- Kent State style: sentence-case headings, no Oxford comma in a simple series, "and" not "&" in prose, one through nine spelled out, dates like "Sept. 30, 2026", phone "330-672-9980", no exclamation marks, no emoji.
- Names: "Advanced Telerobotics Research Laboratory" on first reference, then "the lab"; "ATR Lab" only in display and tight space on a piece that names Kent State. "Jong-Hoon Kim, associate professor of computer science", then "Kim"; no "Dr.". The round emblem is the "roundel", never a seal.
- Words: ROS 2 (never "ROS2" in prose), teleoperation, telepresence, tele-embodiment, human-robot interaction, open-source (adjective), real-world (adjective), advisor, leader-follower; robots are "it".
- Cut hype: cutting-edge, state-of-the-art, revolutionary, groundbreaking, world-class, innovative, novel, leverage, utilize, seamless, robust, holistic, transformative, pivotal, delve, furthermore, moreover. Quoted text and paper titles keep their original words.
- Never upgrade a result. A finalist is not a winner; a selection is not a placement; a special-session award is not a conference best paper.
- People: name students only with their written permission. Never name anyone under 18. Citations keep the published author list.
- Page structure (all pages except `README.md`, `AGENTS.md`, `CLAUDE.md`): `# Title`, a "Read this when" blockquote, a two-to-four-sentence intro, a Contents list when there are five or more sections, the sections, `## Related`, then the "Last reviewed" footer line. Relative links inside this repo; full `https://github.com/ATR-Lab/<repo>/blob/<branch>/<path>` links across repos.
- File names: lowercase kebab-case. Keep paths stable; other repos link here.

## Task: add a member profile from an issue

Issues from `.github/ISSUE_TEMPLATE/member-profile.yml` carry the `member-profile` label. The form renders each field as `### <label>` followed by the answer; empty optional fields read `_No response_`; ticked boxes read `- [X]`.

1. **Read the issue** (`gh issue view <n> --repo ATR-Lab/about`).
2. **Check consent.** Under "Consent (required)", both boxes must be ticked: the publishing consent and "I am 18 or older." If either is unticked, stop: comment asking the member to confirm, and add nothing.
3. **Never add** anyone who did not consent, anyone who is or may be under 18, or any high school intern. If in doubt, stop and ask the lab lead.
4. **Screen for private data** (phone numbers, ID numbers, home addresses, dates of birth). If present, don't copy it; ask a maintainer to edit the issue.
5. **Create `members/profiles/<slug>.md`**: slug from the printed name, lowercase ASCII, words joined by hyphens. Use the front matter and body format in `members/README.md` ("Profile file format"); keys match the form's field ids. Set `consent: true`, `adult: true`, `source_issue: <n>`, `approved_on: <YYYY-MM-DD>`.
6. **Headshot only with photo consent** ("Photo consent (optional)" ticked): save the attachment as `members/profiles/<slug>.jpg` after stripping GPS data, and set `photo`. Otherwise leave `photo` empty and don't download the image.
7. **Update `members/README.md`**: add a row to "Current members" (role order, then last name) or "Alumni" (with years), linking the name to `profiles/<slug>.md`. Remove the `[to be supplied through the form]` row once the first real row exists.
8. **Style-check the bio** (third person, 50 to 80 words, Kent State style) and run the checks below.
9. **Open a pull request** titled `Add member profile: <name>` with `Closes #<n>` in the body. Don't merge it yourself unless the lab lead asked you to. After merge, comment on the issue with a link to the profile (the `Closes` keyword closes it).
10. **Removal requests:** delete the profile, headshot and table row in one pull request that closes the request.

## How to check your work

Run from the repository root (macOS or Linux, with Node.js for `npx`):

```bash
# 1. Brand, facts and Kent State style (exit 0 = no errors). README files are named explicitly.
PYTHONDONTWRITEBYTECODE=1 ~/.claude/skills/atr-lab-design/.venv/bin/python ~/.claude/skills/atr-lab-design/scripts/brand_check.py $(git ls-files --others --cached --exclude-standard '*.md')
# 2. Markdown structure
npx --yes markdownlint-cli2 "**/*.md"
# 3. Hype words and "ROS2" in prose (review each hit; slugs, URLs, code and paper titles are fine)
grep -rnE -i "cutting-edge|state-of-the-art|revolutionary|groundbreaking|world-class|innovative|novel|leverag|utiliz|seamless|robust|holistic|transformative|pivotal|delve|furthermore|moreover|ROS2" --include='*.md' .
# 4. Issue forms parse as YAML (needs PyYAML)
python3 -c "import yaml, glob; [yaml.safe_load(open(f)) for f in glob.glob('.github/ISSUE_TEMPLATE/*.yml')]; print('ok')"
```

Brand-check warnings for intentional `[placeholders]` are expected. CI (`.github/workflows/docs.yml`) runs markdownlint and the lychee link checker, which also checks relative links.

## Open items

Placeholders in this repository, by file. Only the people named can fill them; agents must not fill them by guessing or by copying from older pages.

| File | Placeholder | Who can fill it |
|---|---|---|
| `README.md`, `press-kit/README.md`, `press-kit/fact-sheet.md` | `[UCM contact]` (media relations contact to print) | Director, with UCM |
| `README.md` | `[program kent.edu address]` | Director |
| `README.md` | `[Giving URL: confirm designation]` | Director, with Kent State's Division of Philanthropy and Alumni Engagement |
| `research.md`, `achievements.md` | `[confirm current role before use]` (NSF PRIDe) | Director |
| `publications.md` | `[paper title, to be confirmed by the director]`, `[DOI]` (same award) | Director |
| `research.md` | `[years]` for the Gesture-Enabled Telepresence Robot (Gesture2Game); `[years]` and `[one-line description from the director]` for MOVR | Director; Irvin Steve Cardenas (MOVR) |
| `research.md` | `[to be announced]` (2026 Summer Workshop details) | Director or program lead |
| `press-kit/README.md` | `[to be supplied]`: director headshot, photos, b-roll, coverage entries | Director; lab members; whoever handles communications |
| `press-kit/director-bio.md` | `[areas from the approved CV]`, `[One verified recognition.]` | Director (approved CV) |
| `press-kit/director-bio.md` | `[to be supplied]` (headshot), `[photographer or source]` | Director |
| `press-kit/photos/README.md` | `[to be supplied]` (photos, photo log rows), `[b-roll storage location]` | Lab members; lab manager |
| `members/README.md` | `[to be supplied through the form]` (current members and alumni rows) | Each member, through the form |
| `members/README.md` | `[lab lead name]`, `[lab lead kent.edu address]`, `[date]` (in the message to members) | Lab lead |

Drafts awaiting the director's approval (keep the "draft" labels until then): the one-liner, the 25-, 50- and 100-word boilerplates and the social bio in `press-kit/boilerplates.md`; the director bio in `press-kit/director-bio.md`.

Other decisions for the lab:

- Create the `member-profile` label in this repository; GitHub does not create labels from issue forms.
- UCM review of the ATR mark next to Kent State identity before the logo pack is used publicly.
- Website fixes listed in `publications.md` (entries that differ from the publisher's record) and the stale "Current Project" block on the lab homepage.
- Recount the public repositories (55 on Sept. 30, 2026) before printing the number.

## Related repos

| Repo | The question it answers |
|---|---|
| [about](https://github.com/ATR-Lab/about) | What is the lab, what has it done and who is in it? (this repo) |
| [getting-started-atr-lab](https://github.com/ATR-Lab/getting-started-atr-lab) | I just joined: what do I do first, and what are the lab rules and safety rules? |
| [dev-guidelines](https://github.com/ATR-Lab/dev-guidelines) | How do we write code, use Git and review changes in the lab? |
| [all-things-ros2](https://github.com/ATR-Lab/all-things-ros2) | How do I install, use and debug ROS 2 on the lab's robots? |
| [.github](https://github.com/ATR-Lab/.github) | What does the ATR-Lab organization profile show, and what are the org-wide issue and PR defaults? |
