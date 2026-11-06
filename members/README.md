# Members

> **Read this when** you want to know who is in the Advanced Telerobotics Research Laboratory, you are a member who wants to be listed, or you maintain the member list.

Members list themselves: each person submits a short GitHub form, the lab lead reviews it, and the approved profile becomes a file in [profiles/](profiles/) plus a row in the tables below. Nobody is listed without their own written permission, and nobody under 18 is ever listed by name.

## Contents

- [Director](#director)
- [Current members](#current-members)
- [Alumni](#alumni)
- [Submit your profile](#submit-your-profile)
- [Message to send to lab members](#message-to-send-to-lab-members)
- [Consent and minors](#consent-and-minors)
- [Maintainers: turn an approved issue into a profile](#maintainers-turn-an-approved-issue-into-a-profile)
- [Profile file format](#profile-file-format)
- [Related](#related)

## Director

| Name | Title | Education | Profile |
|---|---|---|---|
| Jong-Hoon Kim | Associate professor of computer science; director of the Advanced Telerobotics Research Laboratory | Ph.D., Louisiana State University | [Kent State profile](https://www.kent.edu/cs/jong-hoon-kim) |

## Current members

> [!NOTE]
> **To do:** this table fills as approved profiles arrive through the [member profile form](https://github.com/ATR-Lab/about/issues/new?template=member-profile.yml). Don't copy names from the lab website's Team page: it is out of date, and listing someone needs their own consent.

| Name | Role | Program | Since | Profile |
|---|---|---|---|---|
| [to be supplied through the form] | | | | |

Order: roles in the order of the form (postdoctoral researchers, Ph.D. students, M.S. students, undergraduate researchers, visiting researchers, staff, other), then by last name.

## Alumni

> [!NOTE]
> **To do:** alumni are listed the same way, only with their consent. Former members can use the same form and pick "Alumni".

| Name | Role in the lab | Years | Profile |
|---|---|---|---|
| [to be supplied through the form] | | | |

## Submit your profile

**[Open the member profile form](https://github.com/ATR-Lab/about/issues/new?template=member-profile.yml)**

- You need a GitHub account and must be 18 or older.
- Have ready: your name as it should be printed, your role, program and start term, a 50- to 80-word bio in the third person and, if you want, a square headshot (at least 800 × 800 px, plain background).
- The issue is **public the moment you submit it**. Don't include phone numbers, student or employee ID numbers, home addresses or anything else private.
- Ticking the two required consent boxes is your written permission to be listed. Photo consent is a separate, optional box.
- To update your profile later, submit the form again. To be removed, open an issue that says so or email the director.

No GitHub account, or you'd rather not post publicly? Email the same information to [lab lead name] at [lab lead kent.edu address], and state in the email that you consent to being listed and are 18 or older. The lab lead keeps that email as the record of consent.

## Message to send to lab members

The lab lead can paste this into Slack or an email. Fill the brackets first.

```text
Subject: Add your profile to the lab's member page

Hi everyone,

We are rebuilding the Advanced Telerobotics Research Laboratory's member page on GitHub, and we would like to list you, with your permission.

Please fill in this short form by [date]:
https://github.com/ATR-Lab/about/issues/new?template=member-profile.yml

You will need a GitHub account, a 50- to 80-word bio written in the third person and, if you want one on the page, a square headshot.

Before you start:
- The form creates a public GitHub issue. Anyone can read it, so don't include phone numbers, student IDs, home addresses or anything private.
- Use the form only if you are 18 or older. High school interns should not use it; we never list anyone under 18 by name.
- Being listed is optional. If you would rather not be listed, simply don't submit.
- You can ask us to update or remove your profile at any time.

Alumni are welcome too: choose "Alumni" as your role and add the term you left.

Questions? Reply here or ask [lab lead name].

Thanks,
[lab lead name]
```

## Consent and minors

> [!CAUTION]
> These rules protect members and minors. They come from Kent State style and the lab's rules on writing about minors.
>
> - **Students are named only with their written permission.** For this page, that permission is the member profile form with both required boxes ticked, or an email that says the same thing.
> - **High school interns and anyone under 18 must not use the form and are never listed by name.** Credit their work to the group ("a team of high school interns built..."), with no names, ages or schools. If you can't tell whether someone is 18, treat them as a minor.
> - **Photos:** publish a headshot only when the photo consent box is ticked. Never publish a photo of a minor on this page.
> - **Withdrawal:** when someone asks to be removed, remove their profile file, table row and headshot promptly.

## Maintainers: turn an approved issue into a profile

Issues from the form carry the `member-profile` label. GitHub turns each form field into a `### Label` heading followed by the answer; empty optional fields read `_No response_`, and ticked boxes read `- [X]`.

1. **Check the issue before anything else.**
   - Both required consent boxes are ticked: "I consent to the Advanced Telerobotics Research Laboratory publishing my name..." and "I am 18 or older." If either is missing, don't add the person; comment and ask.
   - The person is not a high school intern and is not under 18. If in doubt, don't add them; ask the director.
   - Nothing private is in the issue (phone number, ID number, home address). If there is, edit the issue to remove it and tell the member.
   - The bio is 50 to 80 words, third person, Kent State style (full name first, then last name; no "Dr."; no Oxford comma; titles lowercase after the name). Make small style edits yourself; ask the member before changing meaning.
   - Projects are lab projects, and any links point to public repositories only.
2. **Make the slug** from the printed name: lowercase, ASCII letters and digits only, words joined by hyphens (for example "Firstname Lastname" becomes `firstname-lastname`). If that file already exists for someone else, add a middle initial.
3. **Create `members/profiles/<slug>.md`** in the [profile file format](#profile-file-format), copying each field from the issue. Leave optional fields that read `_No response_` empty.
4. **Headshot, only if the photo consent box is ticked:** download the attached image, strip location data (`exiftool -gps:all= -overwrite_original <file>`), save it as `members/profiles/<slug>.jpg` (or `.png`) and set `photo` in the front matter. Without photo consent, don't download or link the image, and set `photo` empty.
5. **Update the tables** in this file: current members go in [Current members](#current-members) in role order, then by last name; alumni go in [Alumni](#alumni) with their years. Link the name to `profiles/<slug>.md`.
6. **Open a pull request** titled `Add member profile: <name>` with `Closes #<issue number>` in the description, so merging closes the issue.
7. **After merge,** comment on the issue with a link to the published profile.
8. **Updates and removals:** a newer form from the same person replaces the old profile (keep the original `start` term unless they correct it). A removal request deletes the profile file, its headshot and its table row; close the request with a short confirmation.

## Profile file format

One file per person in [profiles/](profiles/), named `<slug>.md`. YAML front matter mirrors the form's fields (the keys match the form's field ids); the Markdown body is the bio.

```markdown
---
name: "Firstname Lastname"        # "Name as it should be printed" (required)
preferred_name: ""                # optional
pronouns: ""                      # optional
role: "Ph.D. student"             # exactly one of the form's role options
program: "Computer science, Ph.D., class of 2028"
start: "Fall 2025"                # start term and year (required)
end: ""                           # end term and year, alumni only
interests:                        # from "Research interests"
  - "Human-robot interaction"
  - "Teleoperation"
projects:                         # from "Lab projects"
  - "PepperKit"
links:                            # leave any unused key empty
  github: ""
  website: ""
  scholar: ""
  orcid: ""
  linkedin: ""
photo: ""                         # "firstname-lastname.jpg" only with photo consent
consent: true                     # both required consent boxes were ticked
adult: true                       # "I am 18 or older" was ticked
photo_consent: false              # the optional photo box
source_issue: 0                   # number of the issue the profile came from
approved_on: "2026-10-01"         # date the lab lead approved it (YYYY-MM-DD)
---

Firstname Lastname is a Ph.D. student in computer science at Kent State University and a member of the Advanced Telerobotics Research Laboratory. Lastname works on ...
```

Rules for the file:

- `consent` and `adult` must both be `true`, or the file must not exist.
- `role` uses the form's wording exactly: Director, Postdoctoral researcher, Ph.D. student, M.S. student, Undergraduate researcher, Visiting researcher, Staff, Alumni or Other.
- Dates in `start` and `end` are a term and a year ("Fall 2025", "Spring 2026"); `approved_on` is ISO (`YYYY-MM-DD`) so scripts can sort it.
- Keep the bio as the member wrote it, apart from small style fixes.

## Related

- [Profiles folder](profiles/): one approved file per member
- [Member profile form](../.github/ISSUE_TEMPLATE/member-profile.yml): the fields members fill in
- [AGENTS.md](../AGENTS.md): the same procedure, written for coding agents
- [Press kit](../press-kit/README.md): the director bio template
- [getting-started-atr-lab](https://github.com/ATR-Lab/getting-started-atr-lab): onboarding for new members

<sub>Last reviewed: Nov. 4, 2026 · Sources checked Sept. 30, 2026 · [Suggest a change](https://github.com/ATR-Lab/about/edit/master/members/README.md)</sub>
