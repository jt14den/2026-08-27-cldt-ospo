# CONTEXT.md — UC OSPO Collaborative Lesson Development Training (CLDT)

> For workflow rules and non-negotiables, load: `projctx bundle ospo_education`

## Event Facts

| Field | Value |
|---|---|
| Workshop title | UC OSPO Collaborative Lesson Development Training |
| Carpentry type | cp (Carpentries — custom/instructor-style training) |
| Curriculum / flavor | n/a |
| Start date | **Licensing LOCKED:** Thu 8/27 (afternoon). **Stewards:** TBD |
| End date | **Licensing LOCKED:** Fri 8/28 (full day) — afternoon+full day = 12 hours exactly, no additional days |
| Mode | online |
| Format | Licensing: Thu PM + Fri full day = 12 hours, confirmed with all four (Reid can't do Thu AM, which is why it moved to PM). Stewards: same content, deferred to September by default — poll built (not sent), option to join Licensing's session instead if it still works for them |
| Host institution | UCLA / UC OSPO Network |
| Daily times + timezone | Thu: afternoon PT, exact time TBD. Fri: full day PT, exact times TBD |
| Contact email | tdennis@library.ucla.edu |
| Trainer | Tim Dennis (UCLA / UC OSPO Network) — organizing and teaching directly, not Toby |
| Registration | Closed cohort — not public |
| GitHub repo | jt14den/2026-08-27-cldt-ospo |
| GitHub Pages URL | https://www.tim-dennis.com/2026-08-27-cldt-ospo/ (custom domain, same as the other workshop repos) |

## Cohorts

| Cohort | Topic | Lead | Roster | Schedule |
|---|---|---|---|---|
| 1. Librarians as Open Source Stewards | [Scoped, issue #121](https://github.com/UC-OSPO-Network/education/issues/121) | Anna Sackmann | Anna Sackmann, Sam Teplitzky, Jake Gibson, Rachel Torres (all UC Berkeley) | Deferred to September by default (poll built, not sent: https://lettucemeet.com/l/o2KYR); alternative is joining Licensing's Thu PM + Fri session |
| 2. Software Licensing | [Scoped, issue #83](https://github.com/UC-OSPO-Network/education/issues/83) | Karla Padilla (UCSD) | Karla Padilla (UCSD), Reid Otsuji (UCSD), Laura Langdon (UC OSPO), Jose Niño Muriel (UCSB) | **Locked:** Thu 8/27 PM + Fri 8/28 full day |

Jose Niño Muriel (UCSB) declined to anchor a third cohort (2026-07-09/10) and joined Licensing as its 4th member.

## Status

- [x] Repo scaffolded from carpentries/workshop-template
- [x] `_config.yml` configured (carpentry: cp, title, contact)
- [x] `index.md` front matter drafted — **dates are placeholders, not confirmed**
- [x] Custom "Who Can Attend" + "Participants" sections added (closed cohort, not public template content)
- [x] 2-day schedule drafted for Licensing: Thu PM (backward design, personas, objectives) + Fri full day (episodes, Workbench, drafting, pilot planning)
- [x] Custom Setup section (Carpentries Workbench + GitHub, not a domain-specific curriculum)
- [x] Licensing locked 2026-08-19: Thu 8/27 afternoon + Fri 8/28 full day = 12 hours, confirmed with all four (Jose, Karla, Reid, Laura — Laura may duck out ~2pm Thursday, covered by recording)
- [x] Jose's cohort choice confirmed: Licensing (roster updated 2026-08-17)
- [x] Sent format/recording/post-workshop-support email 2026-08-17; sent locked-schedule email to Licensing + separate note to Anna (Stewards) 2026-08-19
- [x] Decision made 2026-08-18: split by cohort rather than mixed subgroups. Licensing runs this week (real deadline); Stewards deferred to September by default (no funding urgency on their side)
- [ ] Stewards September poll built (https://lettucemeet.com/l/o2KYR, Aug 31-Sep 30 weekdays, excludes Labor Day + Tim's Sep UC Carpentries teaching days) but not yet sent to Anna
- [ ] Jose's funded time ends Aug 31 hard — this is why Licensing locked into this week rather than waiting on Stewards to coordinate too
- [x] Created GitHub repo `jt14den/2026-08-27-cldt-ospo` (public) and pushed `gh-pages` branch, 2026-08-17
- [x] GitHub Pages enabled (auto-enabled on push; already building as of 2026-08-17)
- [ ] Fill in `collaborative_notes` (Carpentries Etherpad, if provided)
- [ ] Confirm whether Eventbrite/registration is needed at all (currently: no, closed cohort)
- [x] GitHub team structure created 2026-08-20: parent `ospo-lesson-authors` (durable, generic — future lessons get their own child team here) → child `licensing-and-copyright` (scoped to the not-yet-created licensing repo)
- [x] `licensing-and-copyright` team populated: Tim (maintainer), Karla `Kpadil16` (member), Laura `LauraLangdon` (maintainer — auto, she's an existing UC-OSPO-Network org admin), Reid `U2NG` (member, org invite pending), Jose `josenino95` (member, org invite pending)
- [ ] Reid and Jose need to accept their UC-OSPO-Network org invitations
- [ ] Licensing lesson repo itself not yet created — per Tim's call, repo creation happens live in the Workbench episode (Fri), not pre-staged, so the team gets to do the actual exercise as taught; team access is pre-staged so whoever creates it can add the repo to `licensing-and-copyright` immediately
- [ ] Candidate repo slug `licensing-and-copyright` proposed, not finalized; Markdown template (`workbench-template-md`), not RMarkdown — no code/data in this lesson
- [ ] Stewards will get their own child team under `ospo-lesson-authors` once their repo slug is picked (no rush, schedule still TBD)

## Open Issues / Notes

- This site is **not a public open-enrollment workshop** like `2026-05-11-uc-lc` — it's a closed, custom CLDT cohort training. The "Who Can Attend" section reflects that explicitly.
- Directory and repo renamed from the `2026-tbd-cldt-ospo` placeholder to `2026-08-27-cldt-ospo` on 2026-08-17, using the target start date (Thu 8/27) even though it's not fully confirmed yet (waiting on Reid). If the training slips to September, rename again.
- Source docs for this training: `~/obsidian/active/CLDT-cohort-coordination-plan.md`, `CLDT-one-pager.md`, `CLDT-committee-brief.md`, `~/obsidian/reference/wiki/ospo/carpentries-cldt.md`.
- Draft schedule was synthesized from the CLDT wiki article's description of the backward-design curriculum, not a pre-existing agenda — review before publishing.
