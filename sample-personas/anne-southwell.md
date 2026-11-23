---
title: "Personna — Anne Southwell (fictional composite, games student)"
purpose: "Demo persona for sample portfolios in the Alexander theme — (1) theme revision, (2) faculty explainer, (3) model for ~5 early-adopter students. Contrasts with John Donne (2D background artist). Retire once real students replace it."
status: "Draft v0.9 for the November 2026 portfolio specimen. Site filled 23 Nov (Alexander 0.6.5; updated to 0.6.6 the same night); content revision of 23 Nov folded in."
created: 2026-11-21
revised: 2026-11-23
---

# 0. Provenance and caveats

- **Editorial provenance.** Earlier drafts used generic patterns from student and professional profiles. The student, work history, and project results in this dossier are fictional. See §10.
- **Fictional organizations** are marked † below. Company and studio names were made up for this file; check them before publishing so they don't collide with real firms.
- **Miami specifics to check** are marked [VERIFY]. That covers course numbers, the exact degree title, and club names.
- **The name is deliberate.** Lady Anne Southwell (1574–1636) was a Jacobean poet in John Donne's circle, so the two personas are a pair. Search turns up the poet, which is enough to mark the site as fictional; it carries no separate label.
- **Content revision, 23 Nov 2026.** Garrison's revised worksheet rewrote the close of the About text, added passages to Quill, Tidewatch and Heatcheck, a seventh project (*The Beat Between Buoys*), a Gallery of two pieces and the summer-camp job as a fifth Experience entry. This version folds those into §1, §3.5, §4, §8, §9 and §11. The live site carries them; the worksheet snapshot (`worksheets/AnneSouthwell-worksheet.md`) is the field-by-field record.

---

# 1. Identity / header

- **Name:** Anne Southwell (goes by "Anne"; friends say "Southwell")
- **Status:** Senior, graduating May 2027
- **Degree:** B.S. in Games + Simulation, Miami University (Oxford, OH); Minor in Computer Science (CSE). Degree title confirmed in the Miami Bulletin, 22 Nov 2026.
- **Hometown:** Mason, OH (Cincinnati suburb)
- **Seeking:** Full-time role, starting summer 2027, as Tools Programmer, Gameplay/Tools Engineer, or Technical Designer (tools-heavy). Since 23 Nov the About text says so: "I'm graduating in May and looking for a tools-programming role starting summer 2027."
  - **Plan B (she'd say so if asked):** a software role at an Ohio simulation, training or enterprise firm. Many Miami Games/CS alumni land in non-games software first; this is the honest fallback.
- **Contact for demo:** anne.southwell@example.org. Social profiles, downloads, and project embeds are optional fields pending supplied assets.
- **Headline candidates (pick one per narrative; see §7):**
  - "Tools programmer: I build the editors other developers live in."
  - "Games + CS senior making game teams faster, one editor window at a time."
- **LinkedIn headline (pipe style, as real profiles do it):** "Tools Programmer | Unreal C++ & Editor Extension | Games + Simulation, CS minor @ Miami University '27". The site can carry the personal headline; LinkedIn's search rewards keywords.

# 2. Education  [ACADEMIC]

| Item | Detail |
|---|---|
| Degree | B.S. in Games + Simulation, Miami University, Aug 2023 – May 2027 (expected) |
| Minor | Computer Science |
| GPA | 3.46 overall; 3.71 in major |
| Honors | Dean's List ×4 semesters |
| Games core [VERIFY numbers] | IMS211 Game Studies · IMS212 Game Design · IMS213 Game Development · IMS314 Game Usability · IMS285 Inside the GDC · IMS443 Research Methods in Games · IMS489 Game Production · IMS452 Senior Degree Project (Spring 2027) |
| CSE minor [VERIFY numbers] | CSE 174 Fundamentals of Programming (Java) · CSE 271 Object-Oriented Programming · CSE 274 Data Structures · CSE 278 Systems I (C, memory, Linux) · one upper-level elective: Software Engineering (team project, §4.7) |
| Relevant elective | IMS222 Interaction Design. It's where she first treated other developers as "users." |
| Certification | CompTIA A+ (Mar 2025). She earned it the spring before the IT internship; it got her the interview. List once on the résumé, not on the portfolio home page. |

# 3. Experience  [GAME-PRO]

## 3.1 Tools Engineering Intern, Lantern Hollow Interactive† (Columbus, OH), May–Aug 2026  ★
- A mid-size studio (~60 people) making a co-op action game in Unreal Engine 5.
- Built an **Editor Utility Widget plus a small C++ editor module** that batch-validates level assets (missing collision, naming violations, oversized textures) before check-in.
- Hooked the validator into the studio's **Perforce pre-submit** and Jenkins nightly build. Cut "broken-asset" build failures from ~6/week to ~1/week over the last 5 weeks of the internship (the figure her mentor quoted in her exit review).
- Wrote internal Confluence docs and ran one 20-minute lunch demo for level designers.
- **Lesson she'll tell in interviews:** her first version blocked submits outright. Designers hated it, so she changed it to warn by default and block only on hard errors. *A missing collision mesh and a misnamed texture called for different responses.*
- **The same job, LinkedIn-style** (bold lead-ins, one claim each, scale stated; the pattern strong student profiles use):
  - **Asset Validation:** Built a UE5 editor module (C++, Editor Utility Widgets) that checks level assets for collision, naming and texture-budget errors before submit.
  - **Build Stability:** Integrated the validator with Perforce pre-submit and Jenkins nightlies; broken-asset failures fell from ~6 to ~1 per week.
  - **Designer Adoption:** Ran a demo and wrote Confluence docs for 12 level designers; reworked hard blocks into warnings after their feedback.

## 3.2 Tools Programmer (part-time contract, remote), Lantern Hollow Interactive†, Sep 2026 – present (~10 hrs/week)
- Kept on after the internship to maintain the validator and add rules the level team requests.
- Common among strong students: a summer role that becomes a remote contract during senior year. It is also her best hiring signal: *they kept her.*
- Bounded honestly: 10 hours a week, and she says it caps her senior-project hours.

## 3.3 IT Support Intern, Tri-County Mutual Insurance† (Cincinnati, OH), May–Aug 2025
- Help-desk tickets, laptop imaging, and PowerShell scripts that automated new-hire account setup (~40 min saved per hire).
- Not a games job, but it's where she learned to like **removing tedium for other people**. Pass 2 keeps it for that reason.

## 3.4 Undergraduate Teaching Assistant, IMS213 Game Development, Miami, Fall 2025 & Fall 2026
- Held open lab hours (4 hrs/week) for sections of ~25, mostly on Git/GitHub Desktop and Unreal source-control problems, plus the usual Blueprint debugging.
- Wrote the **"Unreal + Git LFS Survival Guide"** for the course (a markdown guide with screenshots, now on the course site). It covers .gitattributes, LFS locking, and restoring a known-good .uasset revision after a binary conflict.
- Pattern to note: her tools instinct shows up in teaching too, because the guide is itself a tool.

## 3.5 Instructor (summer), Code Summit Camps† (Cincinnati area), Jun–Aug 2024
- Taught week-long day camps (ages 11–16) in Unity/C# and Roblox Studio, in 2-hour group blocks.
- A very common first "games" job on real student profiles. For Anne it does two things: it fills the summer after first year, and it's the first time she wrote a handout so she wouldn't have to repeat herself 30 times. (The Git LFS guide is that handout grown up.)
- **On the site since 23 Nov** as Experience entry 5 ("Summer coding instructor"; earlier it stayed off the site). Its text is one small usability lesson: "Taught small groups of 11- to 16-year-olds. My first Unity handout said to open the Inspector. A camper had closed it. I redrew the first panel to show how to get it back, then let the next group start from the sheet while I watched." The last clause is the same habit as Quill's first test: hand over the tool, then watch.

## 3.6 Student staff, Miami IT Services help desk, Jan 2024 – May 2025 (~10 hrs/week)
- Ordinary student job; keep as one line. It shows reliability and steady hours alongside school. Not on the site.

## 3.7 High-school jobs (cut from the résumé; About page only)
- Stock and register at Mason Hardware & Supply†, summers 2021–22. Real profiles often keep seasonal retail through senior year; by senior year Anne has enough game work to drop it.
- Kept as background for one reason: it's where she learned the names of the tools her grandfather uses (§8).

# 4. Projects  [GAME-PRO — the heart of the portfolio]

## 4.1 *Quill*: dialogue & quest data editor for Unreal Engine 5 (personal, open source), 2025–present  ★ flagship
- **Problem:** On student teams, writers draft dialogue in Google Docs and a programmer hand-copies it into Data Tables, which leads to typos, broken quest flags and lost revisions. Anne first saw this in her IMS213 lab hours in fall 2025 and started the importer that semester. When her IMS489 team began Tidewatch in fall 2026, the same problem arrived at full scale, and Tidewatch became Quill's largest user.
- **Tool:** An Unreal editor plugin (C++ with Slate UI) offering a node-graph dialogue editor, conditions/flags, CSV/JSON import from spreadsheets, and a "missing-line" report for localization.
- **Numbers:** two other Miami student teams used Quill. In the case study, show what a writer could do with it. Leave repository statistics off the homepage.
- **Process evidence to show:** early paper mockups, a writer-facing usability test (5 participants, from IMS314 methods), before/after screenshots, the issue tracker.
- **Honest limitation:** no runtime localization yet, and the Slate code "needs a refactor she's afraid of."
- **Reality check:** working tools engineers' profiles describe exactly this kind of job (owning a studio's narrative pipeline: a branching-script writing tool, then automation built on it). Quill is a plausible student-scale version of a real job, not a fantasy project.

**Case-study detail, in Anne's voice:** "The writer changed one line. I had to open Unreal to tell her whether it had made it into the game. That was the part I wanted to get rid of." In the demo, follow one line from the spreadsheet into a dialogue node, then show where the writer can see that its translation is missing. The missing-line report checks the data at edit time. Runtime localization is still open work.

**Added 23 Nov (on the site):**
- *Research:* one writer finished an import, saw "1 missing translation" and asked which line. The importer knew the answer; Anne had left it out of the interface. The finding the test was for.
- *Iteration:* the worked example. In the sample sheet, KEEP_014 changes from "Leave the lamp burning" to "Leave the west lamp burning." The writer can move the row without breaking the branch because Quill matches on its ID. Selecting the warning now focuses that node and shows the empty French field. Credit line: "The writer supplied the dialogue; I wrote the import and selection behavior."

## 4.2 *Tidewatch*: senior team game (IMS489 → IMS452), Aug 2026 – May 2027
- A 7-person team (2 programmers, 2 artists, 2 designers, 1 producer) working as **Lampblack Games†**, a student studio name. Students often list such a studio under Experience (title "Lead Programmer", "self-employed"); Anne lists it under Projects so the internship stays on top. Either works; it's a lever choice.
- Tidewatch is a narrative lighthouse-keeper sim in UE5, targeting an itch.io release and a booth at GDEX.
- **Anne's role:** gameplay programmer *and* the team's de facto pipeline person. She set up the repo, LFS, branching rules, and a GitHub Actions build that posts nightly packaged builds to the team Discord. She also integrated *Quill*.
- **Which build did you open?** (the project's one section, added 23 Nov): the producer filed a ticket about an old line of dialogue; she was playing yesterday's package, which had the same name as today's. Anne put the short commit ID and build date on the title screen and in the Discord post. On the next ticket the producer pasted the ID, and the writer and Anne could open exactly what she'd heard. Small, concrete and checkable: a pipeline fix told as a story about three teammates.
- Portfolio angle: tooling on a real team, with the toolmaker also as the tool's user.

## 4.3 *Heatcheck*: lightweight playtest telemetry for Unity, IMS314 Game Usability, Spring 2026
- A drop-in C# package that logs player position and custom events to JSON. A Python (pandas/matplotlib) script renders heatmaps and death maps.
- Used in her class's usability studies on three student games. Includes a one-page method note: what the heatmap does *not* tell you.
- **The worked example** (added 23 Nov to the second section): one gate looked like a bottleneck until the pause was lined up with the gate-open event; the gate was already open. The observer had written, "Went back to watch the platform." That became the worked example on her method sheet. It shows the limit of the instrument and why an observer still sits in the room.
- This is the bridge to design and research: tools in service of understanding players.

## 4.4 Game jams
- **Global Game Jam 2025**: *Second Helping*, a co-op cooking puzzle (Unity, 3-person team). Anne: programmer.
- **Global Game Jam 2026**: *Undertow*, a one-button rhythm game (Godot). Anne: programmer plus a level-editor script so the designer could place beats without code. (On the site as a Brief; the beat-placement tool reappears in §4.8.)
- **Ludum Dare 57 (Apr 2025)**: solo entry, finished but rough. Keep it as evidence of follow-through, not of quality.

## 4.5 Small utilities (a "toolbox" section, 1 line each)
- `sprite-sheet-slicer`: Python CLI for slicing and naming sprite sheets.
- Unreal Editor Utility Widget for editing item Data Assets in bulk (an IMS213 assignment, extended).
- VS Code snippets pack for Unreal C++ macros (UPROPERTY/UFUNCTION boilerplate).

## 4.6 *Ferryman's Lantern†*: Game Design Club team game, Sep 2024 – Apr 2025 (free on Steam)
- A 14-person club team made a short UE5 puzzle game in Blueprints over two semesters and released it free on Steam. Club-scale shipped games are a recurring pattern on Miami profiles.
- **Anne's role:** junior programmer, then (by spring) the person who could make a build. She wrote the packaging and SteamCMD upload scripts and the "how to ship a build" page, because the one person who knew how was graduating.
- **Numbers:** ~2,100 downloads in the first month (Steamworks dashboard, which she screenshots for the case study).
- Why it matters for the theme: it's her first time as the release bottleneck, and the first time she automated herself out of being one.

## 4.7 *OfficeQueue*: lab help-queue web app, CSE Software Engineering, Spring 2026
- A five-person team built a web app where students join a queue for help during open lab hours; TAs see the queue, mark tickets done and leave notes. TypeScript/React front end, Flask back end, PostgreSQL, everything in Docker containers.
- Anne pitched it from her IMS213 TA hours (the sticky-note queue kept falling off the whiteboard) and wrote the TA-side views.
- Piloted during open lab hours for the last four weeks of the spring software-engineering course; ~130 tickets handled.
- Not a game. Under Lever E (§7) it's a lead project; under Levers A–D it's a *Brief* (one line at the end of Projects).

## 4.8 *The Beat Between Buoys*: editor-scripting workshop, Game Design Club, Fall 2026 (added 23 Nov)
- **Card copy:** "A paper timing exercise for teaching editor scripting." Kind *Brief*, Order 7; role "Workshop author and facilitator"; tags Teaching, paper prototype, editor scripting.
- The "Intro to Editor Scripting" workshop she ran for the club (§6), written up. She brought a roll of adding-machine paper, a marker and a bag of red paper buoys. One person tapped a rhythm; a partner placed buoys on the strip and slid the whole thing under a pencil held still. Then they made the same edit with her Godot beat-placement tool from *Undertow* (§4.4). A participant moved a buoy one square and asked whether she'd moved the note or changed the tempo. Anne added a second pass to the handout: keep the buoys still and pull the paper faster. The two gestures gave them names for two different controls.
- **Why it belongs:** the clearest single statement of Lever B and C together. A paper prototype of an editor's controls, tested on people, revised into a handout: the camp handout (§3.5) and the Git LFS guide (§3.4) at workshop scale.

## 4.9 Gallery (added 23 Nov)
Two pieces in Alexander's Gallery section; before the revision Anne had none.
- ***One Beat Late*** (Order 1, on the home page): two paper timing strips from the workshop (§4.8) aligned at a pencil mark, one red buoy offset by a single square. Caption: "From my editor-scripting workshop. Try tapping both strips at the same speed. Only the third note should land differently."
- ***First Shaving*** (Order 2, not on the home page): two wood shavings beside a hand plane and a penciled arrow on a scrap of pine (§8). Caption: "My grandfather marks the direction of the grain before he hands me the plane. The first shaving broke halfway across. The second is from the same edge after we backed the iron off a little."
- For a tools programmer a Gallery is optional. These two earn their place because each shows a first attempt and an adjustment, the habit her About text claims; *First Shaving* stays off the home page so the hand planes remain a quiet detail.

# 5. Skills (as she'd list them; ordered by evidence)

- **Languages:** C++ (UE5), C#, Python, Java (coursework), C (systems coursework), TypeScript (OfficeQueue)
- **Engines/editor extension:** Unreal 5 (Editor Utility Widgets, Slate, Blueprints, plugin modules); Unity (EditorWindow, custom inspectors, packages); Godot (jam level; beat-placement tool)
- **Pipeline:** Git & Git LFS, GitHub Actions, Perforce (internship), Jenkins (internship, as a user), SteamCMD/Steamworks (club release), Docker (course project)
- **Web (secondary):** React, Flask, PostgreSQL
- **Methods:** usability testing, writing technical documentation and handouts, running workshops, code review, teaching
- **Weak spots she admits:** 3D art, shaders, and networking

# 6. Activities & community  [BOTH]

- **Game Design Club** [VERIFY; this is the name alumni profiles use]: member since 2023; programmer, then build person, on *Ferryman's Lantern* (§4.6); workshop lead 2025–26 (ran "Intro to Editor Scripting", written up as *The Beat Between Buoys*, §4.8)
- **GDC 2026** (via IMS285 Inside the GDC): attended the **Tools Summit** sessions; met her internship recruiter there
- **GDEX 2026** (Columbus): helped staff the Miami booth
- **Open source:** small merged PR to a popular Unreal plugin (a docs fix plus one bug fix)

# 7. Narrative levers (the same data, told five ways)

The persona is built so one data set supports different portfolio stories. Each lever changes what goes first and what gets cut.

| Lever | Story | Lead project | Demoted or cut |
|---|---|---|---|
| **A. Engineer-first** | "I write C++ editor tools." | Quill (code, architecture) | Heatcheck method note, TA work, camp, the workshop |
| **B. Developer-as-user (designer of tools)** | "Tools are UX for developers." | Quill usability test (the missing-translation finding), plus the warn-not-block pivot at Lantern Hollow | Jam games, IT jobs |
| **C. Team enabler / teacher** | "I make teams faster and make knowledge stick." | Tidewatch pipeline (the build ID), Git LFS guide, TA, camp, the club "how to ship" page, *The Beat Between Buoys* | Small utilities |
| **D. Research-minded** | "I build instruments for understanding players." | Heatcheck (the gate that was already open) plus the IMS443 methods work | Internship metrics |
| **E. Software generalist (Plan B)** | "I build software people use, games included." | OfficeQueue, IT internship, Quill as an open-source project | Jams, Tidewatch art |

Pedagogical note for faculty: the same facts support several honest stories, and choosing among them is the portfolio's argument. Lever B has the clearest humanist hook, the toolmaker as someone who serves another person's making (Heidegger's ready-to-hand: a good tool disappears into the work). Since the revision the About text makes the hook explicit: her grandfather hands her the plane and waits for the first shaving; she tries to give a writer the same uninterrupted first turn. Lever E exists because the alumni record says many graduates start outside games. Whether a games portfolio should be built for that is a faculty decision, not the persona's.

# 8. Human details (pass 3: make her cohere)

- **Origin story:** In 9th grade she modded *Skyrim* and wrote a batch script to rename 300 texture files. She liked the script more than the mod.
- **Off-hours:** restores old hand planes with her grandfather, a retired machinist. He marks the direction of the grain before he hands her the plane, then waits for the first shaving. Since 23 Nov this is both the close of her About text and a gallery piece (*First Shaving*, kept off the home page). Used with restraint, it's the persona's single image of toolmaking as a family trade.
- **Plays:** Factorio, Slay the Spire, Outer Wilds; currently replaying Tunic.
- **Reads:** *The Design of Everyday Things*; Robert Nystrom's *Game Programming Patterns* (free online; she cites it constantly).
- **Voice:** plain, a little dry; uses "honestly" too much in her drafts (a revision note for the specimen). On LinkedIn she over-uses "thrilled to announce", like everyone; the portfolio is where she sounds like herself.
- **One sentence a recruiter would remember:** "If a warning stops the whole team, it had better tell somebody what to fix."
- **Contrast with John:** she serves other developers; he serves players' eyes. The pair also avoids the default casting of the man as coder and the woman as artist.

# 9. Page map (for the Alexander sample site)

**Default specimen:** Lever B, for a tools lead hiring a junior programmer in summer 2027. Feature *Quill*. Follow with *Tidewatch* (in progress) and *Heatcheck*. Use the studio validator under Experience. The studio owned it; Quill was Anne's personal project.

| Template field | Suggested public copy |
|---|---|
| Headline | Tools programmer for game teams |
| Intro | I build Unreal editors for the people making the game. My favorite part is sitting beside a writer while she tries the first version. |
| Featured card | **Quill** · A dialogue editor that gives writers a way to check their own changes in Unreal. |
| Experience excerpt | My first asset checker stopped a designer from submitting work over a texture name. I kept the hard stop for missing collision and turned the naming check into a warning. |
| About excerpt (since 23 Nov) | My grandfather and I restore old hand planes. We test one on a scrap of wood before putting it back on the shelf. He hands me the plane and waits for the first shaving. I try to give a writer that same uninterrupted first turn with an editor I built. I'm graduating in May and looking for a tools-programming role starting summer 2027. |

**Pages CMS entry plan (Alexander 0.6.6; site made from 0.6.5 and updated 23 Nov).** From 0.6.6 the Projects form is labelled **Selected Work** and Experience's dropdown **Related work**; nothing stored changed. One row per form, in Pages CMS order. Leave every field not named here empty. This is what the live site holds after the 23 Nov revision.

> **No “fictional” label** (Garrison, 22 Nov 2026; restated 23 Nov): the generic details, the poet's name and the `example.org` email are enough.

| Form | Entries |
|---|---|
| **Profile** | **Your name:** Anne Southwell · **Area of expertise:** Tools programmer for game teams · **About:** the Intro sentence above, then the About excerpt · **Email:** anne.southwell@example.org · **LinkedIn, GitHub, Résumé, Custom Links:** empty (no fictional accounts; a GitHub link for Quill would point at a real user's namespace) |
| **Selected Work** (Projects before 0.6.6) | 1. **Quill**: Kind *Case study*; Year 2025–present; Role "Sole developer"; Caption = Featured card; Tags Unreal, C++, Slate, tools. Sections, the seven defaults in their default order: Problem (writer → programmer copying, §4.1) · My role · Research (usability test, 5 writers; the missing-translation finding) · Prototype (paper mockups) · Iteration (one line followed from spreadsheet to node; KEEP_014) · Outcome (two other teams; missing-line report) · Reflection (runtime localization open; the Slate refactor). 2. **Tidewatch**: *Project*; 2026–27; "Gameplay programmer; build pipeline (team of 7)"; caption says *in progress*; one section, "Which build did you open?"; no itch link until one exists. 3. **Heatcheck**: *Project*; 2026; "Sole developer"; two sections, "Heatmaps and death maps" (with picture) and "What a heatmap doesn't tell you" (the gate example). 4. **Ferryman's Lantern**: *Brief*; 2024–25; "Build and release scripts (club team of 14)". 5. **OfficeQueue**: *Brief*; 2026; "TA-side views (team of 5)". 6. **Undertow**: *Brief*; 2026; "Programmer; beat-placement editor (GGJ)". 7. **The Beat Between Buoys**: *Brief*; Fall 2026; "Workshop author and facilitator" (§4.8). |
| **Gallery** | 1. **One Beat Late** (shown on the home page). 2. **First Shaving** (not on the home page). Captions in §4.9. |
| **Experience** | 1. Tools Programmer (part-time contract), Lantern Hollow Interactive†, remote, Sep 2026 – present. 2. Tools Engineering Intern, Lantern Hollow Interactive†, Columbus, OH, May–Aug 2026; text = Experience excerpt. 3. Undergraduate Teaching Assistant, IMS213 Game Development, Miami University, Fall 2025 & Fall 2026 (the Git LFS guide). 4. IT Support Intern, Tri-County Mutual Insurance†, Cincinnati, OH, May–Aug 2025. 5. Summer coding instructor, Code Summit Camps†, Cincinnati area, OH, Jun–Aug 2024; text from §3.5. **Related work:** none on any entry; the validator belonged to the studio. The help desk stays off the site. |
| **Education** | B.S. in Games + Simulation, minor in Computer Science · Miami University · 2027 (expected) · detail: one line naming IMS314 and CSE 274 (on the site: "Coursework includes IMS314 Game Usability and Data Structures."). |
| **Tools** | Unreal Engine 5 (note: "C++, Slate, Editor Utility Widgets") · Unity (note: "Editor scripting") · Git and Git LFS · GitHub Actions · Perforce · Python |
| **Appearance** | Planned: Ink; Inter for text; Source Serif 4 for titles. **Live:** Dusk; Literata for text; Source Serif 4 for titles (Garrison set it before the fill and it was left as he chose). |
| **Analytics** | Defaults (no statistics; AI training refused). |

**Images needed** (none exist yet; project images 3:2, about 1800 × 1200): Quill editor mockup (card), paper mockup, before/after screenshots and the missing-line report (sections); Tidewatch pipeline diagram; Heatcheck heatmap and death map; Ferryman's Lantern, OfficeQueue and Undertow cards; the buoy strip (*The Beat Between Buoys*); the two gallery pieces (timing strips, wood shavings). Original mockups and photos only, never real software screenshots. Grid placeholders for all 14 are in Garrison's `ClaudeAI_Accessible/AnneSouthwell_assets/` (11 on 23 Nov morning, 3 that evening); palettes in the fill runbook.

# 10. Pass log

- **Pass 1 (generic pool):** major/minor and courses; two internships (one games, one not); TA; campus job; 3–4 projects; jams; club; GDC/GDEX; skills list; GPA; hometown.
- **Pass 1b (grounding, 22 Nov 2026; LinkedIn earlier dossier research).** Patterns borrowed, generically:
  - seasonal retail/food jobs kept on profiles from high school → §3.7 (cut from résumé)
  - summer tech-camp instructor teaching Unity/Unreal to teens → §3.5
  - internship that turns into a remote contract → §3.2
  - student studios listed as Experience ("Lead Programmer, self-employed") → Lampblack Games† note in §4.2
  - club team games released free on Steam → §4.6
  - CS team web app (React/TypeScript, Flask, Docker) → §4.7
  - CompTIA A+ alongside an IT path → §2
  - pipe-style headlines; bold-lead-in bullets with scale numbers → §1, §3.1
  - working tools engineers who own narrative/cinematic pipelines → reality check in §4.1
  - alumni in non-games software, HPC, simulation, grad school → Plan B in §1 and Lever E in §7
  - degree written as B.S. and the club called "Game Design Club" → §1, §6 (still [VERIFY])

  **Deliberately not borrowed:** any real employer, studio, game title, person's name or date; a AAA technical-design internship (too distinctive, and a prodigy marker the method rules out); a study-abroad health-game controller project (memorable enough to identify its maker); an amusement-park job (would collide with the Mason hometown and a real profile).
- **Pass 2 (theme: tools for developers):** *Cut* generic "passionate about games" filler, a freshman Unity platformer, a marketing-club membership, and Photoshop/Blender as "skills" (thin evidence). *Kept* the IT internship and help desk, reframed as removing tedium. *Added* Quill, Heatcheck, the Git LFS guide, the Tools Summit, the warn-not-block lesson, and the Tidewatch pipeline role. *Dossier v0.4 additions* are themed the same way: the camp handout, the club "how to ship" page and OfficeQueue all show her removing tedium for someone else.
- **Pass 3 (coherence):** origin story, grandfather/hand planes, reading list, voice tics, admitted weak spots and limitations, concrete metrics with stated sources, one memorable line. Dossier v0.4 ties the hardware-store job to the hand planes.

- **Dossier v0.6:** Added default template copy in §9 and a concrete design decision in §4.1. Earlier pass entries above are drafting history.
- **Dossier v0.7 (22 Nov 2026):** Quill's timeline fixed (the problem it solves now predates it); degree title confirmed; §9 rewritten as an entry plan for Alexander 0.6.4's Pages CMS forms.
- **Dossier v0.8 (22 Nov 2026):** IMS213 utility moved from Unity to Unreal (the course uses Unreal); no fictional label.
- **Dossier v0.9 (23 Nov 2026):** site filled from the worksheet (morning); then Garrison's content revision folded in (applied to the live site the same evening): About close rewritten (§8, §9); Quill Research and Iteration additions (§4.1); "Which build did you open?" (§4.2); the gate example (§4.3); new §4.8 *The Beat Between Buoys* and §4.9 Gallery; camp job on the site as Experience 5 (§3.5); §5, §6, §7, §9 and §11 brought in line; §9 records the live Appearance. The revision's line asking to label the demo fictional was not applied (Garrison).
- **23 Nov 2026 (late, no version change):** site updated to Alexander 0.6.6 (commit `13f61a4`); §9 uses the new form names.

# 11. Gaps / to-do

1. ~~Ground pass 1 in real profiles.~~ Done 22 Nov 2026 (§10, pass 1b).
2. Verify IMS/CSE course numbers and the club's name ("Game Design Club"?). Degree title confirmed: B.S. in Games + Simulation (Miami Bulletin, checked 22 Nov 2026).
3. Check the † names for real-world collisions: Lantern Hollow Interactive, Tri-County Mutual Insurance, Code Summit Camps (now named on the site, Experience 5), Mason Hardware & Supply, Lampblack Games, *Ferryman's Lantern*; and the titles added 23 Nov, *The Beat Between Buoys*, *One Beat Late*, *First Shaving*.
4. For a second sample, try Lever E alongside the default Lever B.
5. Produce assets: fake screenshots/mockups for Quill and Heatcheck (original, not borrowed); photos of the buoy strips and the shavings.
6. The Donne refrain belongs to John. Anne can call her collection of short technical notes *Commonplace* if the template has room for her Git LFS guide.
7. Résumé length check: the one-page résumé must still cut (the help desk goes first; the camp can stay as one line now that the site carries its story). The portfolio's About and its *Brief* projects can carry the rest.
8. **Size check** (23 Nov): seven projects (four of them Briefs), two gallery pieces and five roles is full for a senior's site. A further addition should replace a Brief; *Undertow* and *The Beat Between Buoys* could merge into one entry if space is needed.
