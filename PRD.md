# Garage Gym PRD

28 October 2026

## Overview

Garage Gym helps a family of three plan each week's workouts around their sports, their goals and the kit in their home gym. It builds sessions from short follow-along video clips, shows what each new piece of kit would unlock, and spots when two people can train together. The hack day prototype is live at [katebordwell.github.io/garage-gym](https://katebordwell.github.io/garage-gym/).

## Problem

There are too many workout options, scattered across too many places, so the week rarely gets planned well.

- Saved conditioning videos sit in Instagram with no way to find one by muscle group, length or kit.
- Runs live in Strava and turbo rides in Zwift, separate from strength and mobility work.
- The family is planning a garage gym for the new house, but there's no view of which kit would be used most.
- Three people train separately, and can't easily see when their sessions line up.

## Users

Each person plans their own week, with their own preferences and their own look and feel.

| User | Main sports | Tools today | Theme |
| --- | --- | --- | --- |
| Mum | Trail and hill running, conditioning | Strava, Instagram saves | Hello-world cats: retro 90s desktop |
| Dad | Cycling, indoor and outdoor | Zwift on the turbo trainer | 2010-era club cycling: black, white, a pink stripe |
| Kid, 14 | Competitive gymnastics | Club training set by her coach | Grown-up preppy: florals, gingham, lilac, teal, yellow and green |

Mum and Kid sometimes enjoy training together, so shared sessions matter.

## Goals and what good looks like

Good looks like a Sunday-night plan that takes minutes, sessions that fit the time and kit available, and a garage that fills up with kit that actually gets used.

| Goal | Signal it's working |
| --- | --- |
| Planning is quick | Each person plans their week in under 10 minutes on a Sunday |
| Sessions fit real life | A session can be rebuilt for a new length or swapped on the day in a few taps |
| Saved content gets used | Clips from saved Instagram videos appear in planned sessions every week |
| Kit buying is guided | Each purchase unlocks videos people then do; nothing bought sits unused |
| The family trains together | Overlapping garage slots turn into shared sessions |
| It feels personal | Each person picks their own theme and wants to open the app |

## Scope

The hack day prototype shows the whole journey, with the kit and content features fully working.

**Working in the prototype**

- Weekly planner per person with real start times, editable entries, and "Start next week" with Repeat last week
- Session builder from tagged clips, with swap, shuffle, length changes and an honest time total (add a clip, repeat one, or finish early)
- Follow-along player; YouTube and Instagram clips open in their own apps
- Kit tracker with quantities and a weekly booking list per item
- Clash detection: kit in use by someone else, or not enough for everyone in a shared session
- Shopping list in three tiers (garage setup, big kit, small kit), ranked by family votes and benefit, with top-pick pictures, optional prices and a budget
- Train together when garage sessions overlap: one person leads, anyone can leave
- Points and rewards: equal points per session, together bonus, personal weekly goals, an opt-in race, Saturday dinner pick and a family kit jar
- Video library with quick capture to an inbox, tagging later, and More like this / Not again ratings
- Three personal themes and a 4-digit PIN per person

**Shown as intent, not built**

- Strava, Zwift and Instagram connections
- Shared family data across devices and real sign-in; today everything saves in one browser
- Big-screen garage TV mode

**Non-goals**

- Replacing Strava, Zwift or Kid's club; Garage Gym is the family's planning and decision layer around them
- Coaching, training load or injury advice; Kid's gymnastics training stays with her coach
- Hosting or downloading other people's videos; the app links to them
- Buying kit inside the app

## Requirements

### Weekly planning

- Each user plans Monday to Sunday, usually on a Sunday night.
- Entries have a day, a start time and a length.
- Entry types: garage session, run, turbo ride, outdoor ride, class or club, other.
- Garage sessions take a focus: core, legs and glutes, upper body, back, full body, mobility, power and cardio.
- Plans change on the day, so any entry can be edited, rebuilt or removed at the last minute.

### Session builder

1. Warm-up clip for sessions of 10 minutes or more.
2. Main clips matching the focus, filling the chosen time.
3. Cool-down clip for sessions of 15 minutes or more.

- Only uses clips whose kit is all owned.
- Garden kit (the trampoline) is only used when the user opts in.
- Users can swap one clip, shuffle the lot, remove a clip or change the length by 5 minutes.
- Session length has no fixed limit; the user sets it.

### Follow-along player

- Plays clips in order with progress, back and next.
- YouTube and Instagram clips open in their own apps; playing them inside Garage Gym comes later.

### Kit tracker

- Lists all kit by group, with where it lives (garage or garden).
- Ticking or unticking kit updates which videos are ready immediately.
- Owned kit takes specifics, such as weights in kg or band strengths, so clips can be matched more precisely later.

### Shopping list

- Ranks unowned kit by how many videos it would newly unlock, then by total videos it appears in.
- Shows example videos each item unlocks and their total minutes.
- Marking an item bought moves it to the kit list and reports what unlocked.
- Some items unlock features rather than videos, such as a garage TV.

### Train together

- When two or more people plan garage sessions on the same day at overlapping times, the app offers a shared session.
- One person leads and picks the focus; the others join the same clips.
- Shared sessions prefer clips tagged as good to do together.
- Only the leader can change a shared session.

### Family view

- A week grid showing everyone's plans side by side, with shared sessions marked.

### Video library

- Browse by focus, and by ready, locked, from Instagram or together.
- Add a video by pasting a YouTube or Instagram link and tagging it.
- Quick add needs only a link, a title and a rough length. New clips land in an inbox and aren't used in sessions until tagged with at least one focus.
- Each person can rate a clip More like this (picked more often, along with clips from the same creator or of the same type) or Not again (never picked for them, or for a shared session they're in).

### Kit bookings and clashes

- Each owned item has a quantity, starting at 1. Each person needs their own piece unless the item is shareable, such as the TV.
- Every planned session books the kit its clips use; a Zwift ride books the bike.
- The week flags clashes, such as "Bike in use by Dad 06:30–07:30". Sessions leave out kit that is booked, or that there isn't enough of for everyone, and say what was left out.

### Prioritising purchases

- Each person votes Must have (+3), Want (+1) or Later (−2) on each item, from their own view only.
- Ranking adds benefit to votes: videos unlocked, clashes fixed, shared sessions opened up, and setup essentials such as flooring and lighting.
- Three tiers: garage setup, big equipment, small equipment. Extra sets, such as a second set of dumbbells, appear when they would fix a clash.
- Top priorities show as pictures; prices are optional estimates, with an optional budget.

### Points and rewards

- 10 points per finished session, whatever its length; +5 for training together; +10 for hitting a personal weekly goal (a number of sessions each person sets).
- The race is opt-in each week. The top scorer picks Saturday dinner; only they can enter it.
- Everyone's points fill a family kit jar (100 points by default) towards the top-priority purchase. The jar keeps its points between weeks.

### Weeks and changes

- Any entry can be edited: day, time, length, type and focus. Moving a shared session takes that person out of it.
- Start next week resets ticks and points, then offers each person Repeat last week or a fresh start.

### Access

- Each person can only edit their own plan and votes, and only the leader can change a shared session.
- A 4-digit PIN per person stops others switching into their view on the same device. It is a convenience, not security.

## Content model

The building block is a short follow-along clip, ideally 30 seconds to 5 minutes, like the Instagram videos Mum already saves. Short clips are what make sessions flexible.

| Field | Example | Used for |
| --- | --- | --- |
| Source and link | Instagram, @ktlyn_lifts | Playing or opening the clip |
| Title | Gymnastics core circuit | Display |
| Length (min) | 2, marked approximate if unchecked | Filling the session's time |
| Focus | Core | Matching the session's focus |
| Type | Warm-up, strength, core, cardio, mobility, recovery, skill | Ordering warm-up, main and cool-down |
| Kit needed | Mat | Ready or locked, shopping list ranking |
| Together | Yes | Shared sessions |
| Location | Garden | Leaving out garden kit unless chosen |

The prototype starts with 33 clips: 5 of Mum's Instagram saves, tagged from screenshots, and 28 YouTube follow-alongs. Sources are mixed on purpose, since tagged content Mum doesn't know about yet is part of the value.

## Platforms and design

Phone first, then laptop and iPad, and eventually a TV in the garage.

- **Phone:** Sunday planning and following clips with the phone propped up.
- **Laptop and iPad:** a bigger screen for follow-alongs in the garage now.
- **Garage TV:** later, a big-screen mode that plays the session hands-free. The TV is on the shopping list.

Each user picks a theme, and switching user switches the whole app.

| Theme | Look | Notes |
| --- | --- | --- |
| Mum: hello-world cats | 90s desktop windows, teal dotted background, pixel fonts, pink and yellow accents | Matches the hack day cat site |
| Dad: club cycling | Black, white, one pink stripe, condensed caps, serif italic | Inspired by 2010-era cycling style; no third-party logos or branding |
| Kid: grown-up preppy | Ditsy florals, teal gingham, lilac with yellow and green, serif italic headings | Kid is 14, so florals over smileys and nothing babyish |

## Integrations and data

The biggest build after the hack day is shared data, so all three phones see the same family week.

| Integration | What it would do | Constraint |
| --- | --- | --- |
| Strava | Pull Mum's runs and Dad's outdoor rides into the week | Needs each person to sign in and a server to hold access |
| Zwift | Pull Dad's turbo sessions into the week | Same sign-in and server need as Strava |
| Instagram saved posts | Bring in saved videos automatically | Instagram doesn't let other apps read saved posts, so clips are added by pasting links or screenshots |
| YouTube | Search short follow-alongs, and later play them inside the app | Some creators block embedding, so the app opens YouTube instead |
| Shared family data | Same plans, kit and shared sessions on every device | The prototype saves to each browser only; needs a small backend and family sign-in |

Plans include a 14-year-old's schedule, so family data stays private to the family and isn't shared publicly.

## Risks and open questions

**Risks**

- Getting Instagram saves in by hand may feel like a chore, so the app's value depends on how easy adding a clip is.
- Clip lengths found online are often unchecked, so sessions may run long or short.
- Video links break or block embedding over time.
- Kit is matched by type, not weight or resistance, so a clip may need heavier kit than the family owns.

**Open questions**

- [ ] How should Kid's gymnastics training, set by her coach, shape what the app suggests for her?
- [ ] Should the app track completed sessions, or is planning enough?
- [ ] Do we have a barbell, or were the barbells the hand weights?
- [ ] Which details matter per kit item: dumbbell weights, band strengths, trampoline size?
- [ ] Should the shopping list include prices and a budget?
- [ ] Who can see whose plans: everyone, or only shared slots?
- [ ] How should family sign-in work when one of us is 14?
- [ ] Does competition suit us, or would a family-only jar and personal goals feel better?
- [ ] Should one item be shareable by taking turns, rather than needing one each?

## Backlog

The next build should make planning lighter and clip capture effortless before adding anything new. Items marked Now are next in line; Later items need sign-in, shared data or integrations first.

| Priority | Item | Why |
| --- | --- | --- |
| Now | Favourite sessions, e.g. "Mum's 15-minute core" or "Dad's post-ride mobility" | Reuse a session in one tap instead of rebuilding it |
| Now | Starting points: build around a saved clip, repeat a favourite, or surprise me | Fewer decisions on a Sunday night |
| Now | Take turns with kit, e.g. "one kettlebell, take turns" | Shared sessions are thin when we only own one of everything |
| Now | "Save for when we have this kit" | Shopping list reflects clips we actually want, not just clip counts |
| Now | Real links and checked lengths for the starter clips | Instagram entries point to profiles; some lengths are estimates |
| Next | "I only have 10 minutes" quick session | Fits a changed day without replanning |
| Next | Invitations based on when people are free, e.g. "Fancy 15 minutes together on Thursday?" | Makes training together an invitation, not just a clash |
| Next | Train alongside: same time, different focus | Mum and Kid can share the garage without the same workout |
| Next | Different home screen per person | Each person opens the app for a different reason; test first |
| Later | Family sign-in and private shared storage across devices | Needed for real use; must work for a 14-year-old |
| Later | Strava and Zwift sync | Runs and rides appear without retyping |
| Later | Share to Garage Gym from the Instagram app | Capture a clip at the moment it's saved |
| Later | Big-screen garage TV mode | Hands-free follow-alongs once the TV is bought |

## Research priorities

The most valuable next step is watching Dad and Kid plan a real week, before building more on their behalf.

| Priority | Question | Method | With |
| --- | --- | --- | --- |
| Now | Where do people hesitate when planning a real week? | Each plans next week in the app while thinking aloud | Dad, Kid, Mum |
| Now | What would each of us open the app for? | Short separate conversations | Dad, Kid |
| Now | How should the app sit alongside coach-led gymnastics without feeling like another coach? | Conversation, led by what Kid enjoys | Kid |
| Next | Does adding and tagging clips stick? | Two weeks of real use, counting clips added and tagged | Mum |
| Next | Does competition help or add pressure? | Two weeks with the race, two with jar and goals only, then a debrief | Family |
| Next | Do we trust the shopping list's ranking? | Rank the top 10 ourselves, then compare with the app | Family |
| Later | When and why do we train together? | Diary of shared sessions over a month | Mum, Kid |

## Hack day demo script

Two minutes, starting on Mum's Week tab. The story: one family, three sports, a garage gym to fill, built in a morning with Claude.

1. **Hook (15 sec):** we're moving and planning a garage gym. Three people, three sports, workouts scattered across Instagram, Strava and Zwift, and no idea what to buy first.
2. **Plan the week (25 sec):** show runs, a Zwift ride and garage sessions with real times. Point out the clash: Mum wants the bike at 07:00 but Dad has it until 07:30. Open a garage session and tap Shuffle all.
3. **Train together (20 sec):** tap the Kid banner and choose Kid to lead. We only own one of everything, so it leaves out kit we'd have to share, which tells us what to buy.
4. **Shop (30 sec):** show the Top priorities pictures, the votes and the reasons behind each ranking. Tap We bought it! on the kettlebell: 3 new videos unlocked.
5. **Rewards (20 sec):** mark a session done for +10 points, then open Rewards to see the race chart. The winner picks Saturday dinner and every point fills the kit jar.
6. **Ending (10 sec):** switch to Dad, then Kid, so the whole app changes style. Same app, three personalities.

**Before going on**

- [ ] Tap Reset demo so everything starts fresh
- [ ] Don't set PINs; if switching asks for one, tap Skip for now
- [ ] Don't play videos live, as they open YouTube in a new tab; use Mark done for points
- [ ] Optional: set the exercise mat to 2 in Kit so the shared session isn't thin
