# What Makes a Roblox Game Go Viral — Deep Dive (Oct 2026)

*Compiled 2026-10-26. This follows `01-market-research-oct-2026.md`. That report covered **what** is popular; this one covers **why**. It combines five research tracks: two genre teardowns, viral-hit history and themes, marketing and distribution, and UI/UX and player psychology. It ends with a scoring rubric and a cheap-to-build kit we can use in brainstorming.*

> **Confidence.** Mechanics and prices come from guide sites and trackers, which often disagree. Where a number is a range, sources conflicted. Items marked *(u)* are unverified or inferred. **Correction to report 01:** 99 Nights in the Forest peaked at about **14.2M CCU** (Oct 2025), not 2.2M. The 2.2M figure came from a tracker that started recording later.

---

## 0. The short version: the viral equation

Every 1M+ CCU breakout of 2025–26 is a combination of the same seven layers. A game missing any one of them tends to peak at tens of thousands of players, not millions.

```
VIRAL HIT =
  1. A title that IS the rule           ("Steal an Egg", "DONT SPLASH", "99 Nights in the Forest")
× 2. One verb, loop playable in 30s     (grab-and-run-home, plant-sell, jump-don't-splash)
× 3. A hot collectible noun + rarity    (brainrot → lucky block → egg/pet → animals/mounts)
× 4. A social friction moment           (stealing, betrayal, pushing a friend into the water)
× 5. A number that climbs forever       (Speed, $/s, Night 47, Shift 11, +1 per second)
× 6. A shared clock                     (5-min restocks, Saturday update + Admin Abuse, seasons)
× 7. A 3-second clip moment             (rare reveal, theft, jumpscare, splash, mass swarm)
```

The 2026 platform adds two conditions on top of the equation:
- **Retention gate.** The algorithm now counts 28-day retention, first-minute bounce, days spent playing with friends and days with a purchase. A game that gets a spike but can't keep players gets cut off within about a week.
- **Audience gate.** A new game is shown only to age-checked players aged 16+ until it reaches **500 highly engaged players** (plus a refundable 1,000 Robux fee). Only then does it reach the 9–15 audience. The first wave has to come from older players, ads, or players we send from outside Roblox.

---

## 1. The two families of viral hits

Nearly every breakout belongs to one of two families. They spread differently, so they need different designs.

| | **Family A: Collect / Steal / Idle Tycoon** | **Family B: One-Rule Horror / Co-op / Chaos** |
|---|---|---|
| Examples | Steal An Egg (14.3M), Steal a Brainrot (25.9M), Grow a Garden (22.4M), Break and Steal an Egg (1.3M), Kick a Lucky Block (~1.7M), Ride A Pet (~1.6M), +1 Speed Keyboard Escape (3–6M) | 99 Nights in the Forest (14.2M), Dead Rails (1.48M), Forsaken (1.22M), Animal Hospital (~1.2M), Dandy's World (867K), DONT SPLASH (116K in a week), Huss Valley (175K), Backseat Rally |
| Core feeling | Greed, envy, ownership, "numbers go up" | Fear, laughter, teamwork, betrayal |
| Why it spreads | "Look what I got" rare reveals; "he stole my ___" outrage; whole-server events | "Spot the anomaly" puzzles; jumpscare reactions; friend-betrayal fails |
| Session shape | Endless, idle-friendly, with appointments to come back | Rounds, runs or shifts of 5–20 minutes, with a visible "how far did you get" counter |
| Peak ceiling | **Highest** (10–26M) | High (1–14M) |
| Decay | Fast: down 95–99% within 6–9 months, leaving a 200–300K tail | Slower: 99 Nights still about 250K a year later |
| Money | Volume: luck, speed and multiplier passes | Revive, class and cosmetic purchases at the moment of loss |
| Build complexity | Low–medium (data, economy, a few mechanics) | Low (one-rule obby) to high (AI monsters, co-op) |

**The strongest recent hybrids combine both families.** *Sell Fries! [Anomaly]* is a tycoon by day and horror by night. *99 Nights* combines gathering and crafting with horror. *Kick a Lucky Block* puts a tsunami chase on top of a collection game.

---

## 2. Teardown cards: what each hit actually does

### Family A

**Steal An Egg and Collect Rare Pets** (Jul 25 2026; 14.27M peak on Sep 19; 7-player servers; ~15-minute average session)
- **Loop:** run into a biome → press E to grab an egg → sprint home while the biome Guardian chases you, with a "RUN!!" warning; if it catches you, you're ragdolled and drop the egg → place the egg in your Pen → hatch it on a timer (rare eggs take hours) → the pet earns $/s.
- **One gating stat, Speed.** It is trained on a treadmill. Each biome has a soft speed requirement: Forest 0 → Lake 900 → Desert 10K → … → Cosmic 700M → Angels vs Demons 20B. You *can* go in early; the Guardian will just catch you.
- **Rarity:** 10 tiers, Common through Divine. Income runs from **$1/s to $8M/s**. On top of rarity, a mutation can multiply value: Silver 1.2×, Golden 2×, Rainbow 3×, Luminous 10×. Size also matters, and bigger eggs are more likely to carry a mutation.
- **Shared clocks:** egg spawns reset for everyone every 5 minutes, followed by a 13-second map closure, so the whole server stampedes at once. Boss rifts and drone invasions every 30 minutes. A biome rotates nightly.
- **PvP:** steal eggs from other players' bases. A bat knocks a carrier over so they drop the egg; a bear trap holds them for 5 seconds.
- **First 60 seconds:** like, favorite and join the group for **+10,000 Speed**. That skips two biomes and also feeds the algorithm (likes, favorites and group joins). Then the first hatch shows a pet and its $/s.
- **Live-ops:** an update every Saturday, each adding a biome, an egg tier or a mutation, plus Admin Abuse. Story beats such as "Sammy Is Coming", a teased crossover with Steal a Brainrot's developer, set the record.
- **Monetization is lean:** 2× Money (399 Robux), 2× Hatch Speed (467), Instant Hatch (~9 Robux per egg), Speed packs, and a rotating premium egg. No codes.
- **The cautionary tale:** the treadmill originally had a TikTok-style "Reels" feed that paid Speed for watching. Roblox pulled the game for 3–4 hours, then banned that mechanic for under-16s across the platform.

**Steal a Brainrot** (May 2025; 25.9M record; 8-base servers)
- **Loop:** a red conveyor parades Brainrots with price tags → buy one → it walks to a pedestal in your base and earns $/s → collect by stepping on the pedestal → raid other bases when their lock runs out.
- **Stealing rules:** while carrying a stolen unit you are slowed and can't use items, and **the owner gets an alert**. One bat hit sends the unit back to its owner.
- **Base lock:** 30 seconds of protection when you join. After that, a lock button gives 60 seconds of shield, plus 10 seconds per rebirth and per VIP.
- **Pity timers:** a Legendary appears on the belt about every 5 minutes and a Mythic every 15. Higher tiers ("Brainrot God") appear when the game hits like milestones, which gives players a reason to press like.
- **Mutations:** Gold 1.25× up to Rainbow 10×, plus event-only traits (Nyan 6×). They stack: Rainbow + Nyan = 60×.
- **Rituals:** three players in a triangle with a particular unit summon a meteor for the whole server, which forces cooperation.
- **Rebirth:** wipes cash and units in exchange for a permanent multiplier and extra floors. Later rebirths require specific Secret-tier units, which pushes high-end players to steal.
- **Live-ops:** weekly Saturday Admin Abuse plus "Taco Tuesday". The developer floods servers with exclusive units, luck boosts and chaos.
- **Scale events:** the "Admin War" against Grow a Garden produced a **47.4M platform record**. A Bruno Mars concert in the game reached 12.8M.
- **Theme:** Italian Brainrot memes at the peak of their search interest, so kids already knew the characters from TikTok audio.
- **Viral clip:** "kid cries after getting robbed" videos drew tens of millions of views.

**Grow a Garden** (Mar 2025; 22.4M; built in about 3 days by a 16-year-old)
- **Loop:** buy a seed → plant → harvest → sell for Sheckles → buy rarer seeds.
- **Plants grow while you're offline**, so there is always a reason to come back.
- **Shop restocks every 5 minutes for the whole server** (or skip the wait for 79 Robux).
- **Weather is a server-wide mutation event:** Rain 2×, Frozen 10×, Shocked 100×, Celestial 120×. Everyone looks at the same sky at the same moment.
- **Social:** stealing a crop costs 37 Robux, and the steal is **announced to the whole server**.
- **Growth curve:** about 1K CCU when a studio partner bought in, then weekly named Saturday updates with Admin Abuse took it 5M → 11.7M → 16M → 21.3M → 22.4M. Each record landed on an update day.
- **Warning:** Grow a Garden 2 (2026) added guilds, combat and night raids, and fell from about 976K to 21K. Adding complexity to a sequel did not work.

**Break and Steal an Egg** (Sep 5 2026; 1.31M; **97.4% like rate**, higher than the original)
- Same game as Steal An Egg plus **one verb and one stat**: eggs have HP, and you swing a pickaxe to break them open.
- That adds a 20-tier pickaxe ladder. Each tier is about 4× the power and 7–10× the cost.
- Adds server-wide countdown events: a "Titanic Egg" everyone swarms to break, and a Demon King Rift boss phase.
- **Lesson:** a fast follower that changes one thing, ships weekly and keeps players happy reaches about 10% of the original's peak.

**Kick a Lucky Block** (Apr 2026; ~1.7M)
- Fill a power meter (a "perfect" kick gives bonus luck) → kick the block; distance decides which rarity zone it lands in → open it for a Brainrot → **a tsunami spawns and chases you home** → place the unit on a pedestal.
- Weights add Kick Power. Rebirth at 1,000 Kick Power. Mutations range from Gold 1.5× to Rainbow 30×.
- Random server-wide luck events (2×, 4× or 8× for 5 minutes) are announced in chat.
- **Lesson:** it combines three proven loops: the brainrot pedestal economy, the tsunami chase, and a skill-timed power bar.

**Ride A Pet** (published Apr 2026, dormant; grew from 3.5K to 129K CCU in a day on Sep 19 when a weather-mutation update shipped, then ~1.6M)
- Ride your pet → a radar shows nearby eggs → **picking one up starts a break timer** → deliver it to your nest → hatch.
- **The pet you hatch becomes your faster mount**, so a better reward also gets you to rarer eggs.
- Odds are shown as "1 in X". There is a physical "Ride Pet With Friend" station for co-op.
- **Lesson:** a dead game can be revived by an update. It then fell to about 3% of its peak within weeks; the ride-and-collect loop alone doesn't keep players long.

**+1 Speed Keyboard Escape** (2026; 3–6M; won the Roblox Innovation Award for Best Party & Casual)
- **Every keyboard key you step on gives +1 Speed**, with an ASMR clack.
- 13 stages; falling resets you to the start of the stretch. Wins buy trails (1.5× up to 20×), idle treadmills (the paid Admin treadmill is 100×) and rebirths.
- Seasonal reskins work: the Halloween reskin produced an **8.5× spike**.
- Single-use "social codes" are generated in Discord, which forces players to join it.

### Family B

**DONT SPLASH** (Oct 17 2026; 48M visits and 116K peak in 9 days; 10-player servers, parties of 1–4)
- **The rule is the title:** "It can't see you. It hears the water."
- Set in the Poolrooms, a known liminal-space meme. You jump across platforms over water; a splash brings the monster.
- **9 stages, each a new twist:** platforms that sink, a rotating bridge, a memory bridge, crushing walls.
- **The climax forces you to break the rule:** two noisy valves start a 14–18-second countdown while the water rises.
- **Clip mechanic:** **player collision is on and there's a Push / Super Push tool**, so friends shove each other into the water. Downed players press H to call for help; teammates rescue them with E or a rope.
- **Monetization at the moment of loss:** a paid self-revive, "double this run's coins" for 24 Robux on the results screen, a Halloween Pack (150), 2× Cash (200), extra tool slots (99/149), and coin packs from 24 Robux.
- **Shipped "[NEW STAGES]" within 7 days** of launch.
- **Lineage:** DOORS' blind "Figure" monster + A Quiet Place + the Poolrooms.

**99 Nights in the Forest** (Mar 2025; 14.2M; film deal with 20th Century Studios)
- The goal is in the title. You keep a campfire alive and rescue 4 kids.
- **The monster has one counter:** tap your flashlight to stun the Deer.
- Day is for gathering; night brings threats. A huge "Night 47" counter makes it easy to brag and to make "Day 1 vs Day 99" videos.
- 25–33 classes bought with diamonds (Camper 10 up to Assassin 500).
- Named events roughly every two weeks; CCU waves line up exactly with event dates.

**Animal Hospital (Anomaly)** (May 2026; ~1.2M; won 4 Roblox Innovation Awards in 2026)
- **Premise:** night-shift vet at a cute Animal Crossing–style clinic. Some patients are not animals.
- **Three checks per patient:** visual (an unnatural grin, wandering eyes), paperwork, and photo vs. CCTV. **Binary verb:** shutter the window, or admit them.
- A Sanity meter works as a soft health bar; coffee restores it. Numbered shifts. Co-op roles split desk and camera duty.
- **Growth was organic and happened before any updates:** average CCU went from **884 to 430K in three weeks**.
- **The characters went viral, not the gameplay.** Fan animations of the Head Nurse cat hit 9.4M and 8M views, and peak CCU (July 12) came in the same window. The two Robux-only classes (Head Nurse 190, Secret Agent 890) are the characters fans draw most.

**Sell Fries! [Anomaly]** (Sep 2026; 112K)
- **Tycoon by day:** peel, fry and serve, then buy automation (a conveyor for $60 up to a Fries Shooter for $12K).
- **Anomalies at night.**
- **Each morning, pick 1 of 4 perks.**
- To win, find the key hidden in one potato.
- Classes are a 7-rarity gacha (the 0.2% Potato King).

**Huss Valley** (Aug 2026; 175K; 30-player servers)
- Red Rover / British Bulldog rules: runners cross the field 3 times, and one knife hit converts you into a chaser.
- **"Hero or Chicken":** each round, one random runner chooses to make a solo crossing for a bonus. It creates a guaranteed spotlight moment every round.

**Dead Rails** (2025; 1.48M)
- Drive a train 80 km through a zombie Wild West.
- **Remixes** Build A Boat and *a dusty trip*.
- **Ignition was Roblox's own TikTok account** (499K likes), followed by Flamingo, KreekCraft and Thinknoodles, followed by Top Trending and Up-and-Coming.

**Backseat Rally** (Oct 2026)
- **The driver can't see the road; the co-driver calls the turns.** The information gap turns voice chat into comedy.
- Solo play gives you an AI co-driver that uses a friend's avatar.

**Murder Mystery 2** (2014, still up to 1.35M): fixed social-deduction roles and a cosmetics and trading economy have kept it alive for 12 years.

---

## 3. The master list of shared patterns

These patterns appeared across both families and all five research tracks.

### Hook and premise
1. **The title is the rule or the loop.** It follows "Verb a Noun", "+1 X", "Don't X" or "Survive N Nights". Roughly 9 of 12 recent 1M+ hits used this. Kids who can't read much understand it, so do non-English players, so does someone glancing at a thumbnail.
2. **Remix proven loops: change one thing.** Steal An Egg = Steal a Brainrot's steal loop + Pet Sim egg hatching + a "+1" treadmill. Animal Hospital = *That's Not My Neighbor* + Animal Crossing. DONT SPLASH = DOORS' Figure + the Poolrooms. Dead Rails = Build A Boat + *a dusty trip*.
3. **The breakout is rarely the first game in a wave.** It's the one that combines the proven loop with the current hottest noun.
4. **Familiar setting, fresh noun.** Kids want something new inside a format they already know how to play.
5. **The cute–creepy or mundane–absurd contrast is the hook.** A vet clinic hiding monsters, a fry shop with anomalies, a kid alone at home.

### Core loop
6. **"Grab it and run home before X."** X is a guardian, a defender's bat, a tsunami, or a break timer. That gives 10–30 seconds of tension, then the relief of reaching safety.
7. **One verb you can play in 30 seconds.** No tutorial. A glowing beam or arrow points at the one thing to do.
8. **One sensory constraint on the monster.** It's blind but hears water, hates light, or punishes you for looking at it. One rule means one counter, which a viewer can follow in a clip.
9. **The climax forces you to break the rule.** Noisy valves, skill checks that alert monsters, a power outage.
10. **Soft gates.** You can go into the hard zone at any time; you'll just lose. Players see what they're aiming for from minute one.

### Collection and randomness
11. **A physical trophy shelf.** Rewards are objects carried and placed on pedestals or in pens with floating $/s labels. Your base is a public display.
12. **Rarity ladders run 8–20 tiers past Legendary,** e.g. Mythic, Cosmic, Secret, Divine, Celestial, Void. Value spans up to a millionfold from bottom to top.
13. **Mutations stack on top of rarity** (1.25× to 120×; stacked traits reach 60× or more). One lucky roll is worth hours of grinding, and that roll is the clip.
14. **Odds shown as "1 in X" plus a size or weight.** Players can see how rare something is and brag about it.
15. **Weather or events apply mutations server-wide.** Everyone experiences the lightning strike at once.
16. **Pity timers** (a guaranteed Legendary every 5 minutes, a Mythic every 15) give even unlucky players regular hits.
17. **An Index** with silhouettes, completion rewards, and permanent gaps from limited items that create FOMO.
18. **Fuse or merge machines** turn duplicates into a second lottery.

### Progression
19. **One number climbs forever,** shown with K/M/B/T/Qa suffixes and a visible "+X/s" rate. Each tier costs about 4–10× the last.
20. **Offline or passive income.** You come back to a pile of cash or a finished hatch.
21. **Rebirth** resets you for a permanent multiplier. Late rebirths require specific rare items, which pushes collection and stealing at the top end.
22. **Shift, night or door counters** ("Night 47", "Shift 11", "Floor 30") turn a game into a series of videos and "how far did you get" comments.
23. **Classes or loadouts are the main sink.** One or two Robux-only hero classes end up as the most charismatic characters.
24. **A roguelite draft between rounds** (pick 1 of 4 perks; vote on 1 of 3 cards).

### Social
25. **Small servers** (6–10 players) for tycoons, so every base is visible and rivalries are personal. **Big servers** (30) for tag and crowd games, where mass conversion makes a good clip.
26. **Theft or betrayal is the social glue.** The owner gets an alert, the server gets an announcement, and the drama produces clips.
27. **Every attack has a counter.** A lock timer, a bat that returns the stolen item, upper floors, private servers, a rescue rope. Losses hurt but can be recovered.
28. **Co-op where you can hurt your teammates.** Pushing, friendly fire, letting the fire go out. Betrayal makes the funniest clips.
29. **Forced cooperation rituals,** like Steal a Brainrot's three-player meteor summon, or Animal Hospital's desk-and-camera split.
30. **A spotlight mechanic,** like Huss Valley's "Hero or Chicken", which manufactures a clip moment every round.
31. **Information gaps create comedy:** a blind driver, a blind monster, hidden roles.
32. **Communication that works without text chat.** Age checks now restrict chat for many players, so emotes, pings, gifting and physical interaction carry the social layer.

### Live-ops
33. **A shared clock.** 5-minute restocks or spawn resets, 30-minute rifts, nightly rotations, weekly Saturday updates. When the timer is visible, the whole server moves together.
34. **Saturday update plus Admin Abuse about an hour before it.** Every 1M+ record was set on an event day.
35. **Each update extends the top of the ladder** with a new biome, egg tier or mutation, so the most engaged players always have a next target.
36. **The title is a live-ops billboard:** `[🎃EVENT]`, `[UPD]`, `[NEW STAGES]`, `[x2]`.
37. **Ship new content within 7 days of launch** (DONT SPLASH added new stages on day 7).
38. **Crossovers and feuds between developers** (the Admin War, "Sammy Is Coming") and celebrity tie-ins.
39. **Seasonal reskins:** the Halloween reskin produced an 8.5× spike, and platform CCU rises 38% in Halloween week.

### Distribution
40. **Mascots that fans adopt.** Animal Hospital's Head Nurse, Dandy's Toons, Forsaken's lore characters. Fan edits are free advertising.
41. **Like, favorite and group-join rewards** that also skip early progress. Roblox itself counts those signals.
42. **Discord social codes, not public codes.** Players have to join the Discord, which then becomes the channel for event notifications.
43. **Built to be recorded.** Huge floating numbers, rainbow auras, rare hatch reveals, mass swarms, theft fails, splash deaths.

---

## 4. The psychology: why these patterns work

### The reward stack (what fires at each time scale)

| Time scale | What happens | Examples | UX that delivers it |
|---|---|---|---|
| **~1 second** | Action → feedback | "+$" floaters, coin tick, step +1 Speed, the splash | Floating numbers, pitch-varied sounds, button squash, haptics |
| **~10 seconds** | Variable reward or tension spike | Egg hatch, conveyor arrival, grab-and-run, jump over water, anomaly check | Slot-machine reveal, rarity colors, "1 in X" |
| **~1 minute** | Upgrade or goal tick | Buy the next tier, progress bar fills, steal or defend, clear a stage | Progress bars that start part-filled, red "!" badges, a purchase prompt at the right moment |
| **~5–10 minutes** | Pulse event | Restock, weather, rift, playtime gift, base lock expires | Toast notification with countdown, server announcement, gift ladder past the 10-minute mark |
| **Session (15–25 min)** | Big unlock | Rebirth, new biome, Index tier complete, jackpot, finishing a run | Rebirth screen, natural stopping point, then "ready in X min" |
| **Day** | Appointment | Offline earnings popup, daily login, free spin, crops ready | "While you were away you earned…" |
| **Week** | Live event | Saturday update and Admin Abuse, weekly leaderboard reset | Event countdown, update log, title tag, codes |
| **Season (4–8 weeks)** | Meta | Battle pass, Halloween or winter reskin, crossover | Pass track with honest end dates |

### The psychological levers, and how hits pull them

| Lever | Mechanism | How the hits use it |
|---|---|---|
| **Variable-ratio reward** | Unpredictable payoffs drive repeat behavior | Eggs, rolls, mutations, lucky blocks |
| **Legible rarity** | A "1 in 1,000,000" is something to brag about | Sol's RNG made the odds themselves the product |
| **Loss aversion** | Losing hurts more than winning feels good | Your stuff sits visibly in your base and can be carried away, so you stay online to guard it |
| **Endowment** | We overvalue what's "ours" | You spawn on your own named plot, and your pets follow you |
| **Social proof and envy** | Others' wins prove wins are possible | Server-wide announcements of rare drops; walking past other players' glowing bases |
| **Goal gradient** | We speed up as a goal gets close | Bars that start 40% full; "3/5 eggs until bonus"; first level-up in under 2 minutes |
| **FOMO** | Fear of missing something limited | 5-minute restocks, limited eggs leaving permanent Index gaps, live-only Admin Abuse drops |
| **Appointment** | A reason to come back at a set time | Offline growth, hatch timers (use them to bring players **back**, never to **stop** them playing) |
| **Anticipation then payoff** | Dopamine fires on the build-up | Egg wobble, a color flash before the reveal, the monster turning toward the splash |
| **Sunk cost** | Investment makes quitting feel costly | Rebirth multipliers, Index progress, class levels |
| **Self-expression and status** | Visible flex | Auras, titles above heads, trails, rare mounts |
| **Reciprocity and community** | Gifts create obligation | Gifting, server-wide luck passes that help everyone, rescue ropes |

**Where the ethical and policy line sits.** A 2026 University of Sydney study flagged false reference pricing, near-miss visuals on paid rolls, pressure after losses, false urgency and pay-to-progress in 14 of the 15 top games. Roblox's own guidelines ban fake scarcity, timers that restart, permanent sales and pushy copy. **Use these levers on gameplay and free rewards. Keep paid offers honest.**

---

## 5. UI/UX blueprint (what top games converge on)

### First 60 seconds (this is the algorithm's "first-play bounce" window)

| Time | What happens |
|---|---|
| 0–5 s | Spawn **on your own named plot** or in a party lobby. No menus, no text walls. |
| 5–15 s | An animated **beam plus a bouncing arrow** point at the one thing to do. |
| 15–30 s | First action is guaranteed to succeed, using starter currency. **First reward reveal with full visual effects.** |
| 30–60 s | Income ticking, first sell or upgrade, a progress bar already about 40% full. A like/group prompt offers a big boost (e.g. +10K Speed). |
| 1–3 min | Second goal; the Index appears ("1/30 discovered"); first free gift. |
| 3–10 min | Social hook: you see someone's rare item, or a server-wide announcement fires. Playtime gifts carry the player past the 10-minute mark. |

### Juice that every hit has
- Floating "+$" numbers in rarity colors that drift upward. Merge them ("+$4.2K ×12") so mobile screens don't flood.
- The currency counter **rolls up and pops** (scale 1.0 → 1.15 → 1.0 with a bouncy ease).
- Panels open with a bouncy scale (0.8 → 1.05 → 1.0) over a dimmed backdrop. Buttons squash on press.
- **Slot-machine hatch sequence:** egg centered on screen → 2–3 wobbles of rising pitch → a **color flash that hints the rarity** → the pet pops in with "1 in X" → Legendary and above get slow-motion, screen shake, confetti, a unique sound sting and a server-wide announcement.
- A sound sting per rarity tier, so players can hear a Legendary from across the map.
- Screen shake and a field-of-view punch on big moments, with a toggle in settings.
- Big numbers abbreviated (K, M, B, T, Qa).

### Rarity colors (players already know this mapping)

| Tier | Color |
|---|---|
| Common | Gray |
| Uncommon | Green |
| Rare | Blue |
| Epic | Purple |
| Legendary | Gold |
| Mythic | Red or pink |
| Secret / Divine | Rainbow cycle, or black with a glow |

Use the same color on the frame, the label above the item, chat messages, particles and sound pitch.

### HUD layout

| Position | What goes there |
|---|---|
| **Left edge, vertical stack** | Shop, Inventory, Index, Rebirth, Trade, Settings. Easy for a thumb to reach, and clear of the mobile jump button. |
| **Top** | Currency pills with a **"+" that opens the Robux shop** |
| **Right side** | Free gift timer, active boosts with countdowns, quest tracker |
| **Top-center toast lane** | "Restock in 1:12", "Event starting", rare-drop announcements |
| **Buttons with rewards waiting** | A red **"!" badge**, the strongest driver of UI exploration |

- **Visual style:** thick dark outlines, saturated gradients, rounded corners, chunky cartoon fonts, icons first, almost no text.
- **Touch targets:** about 8–10% of screen height.

### Retention widgets
- A playtime gift ladder at 5, 10, 15, 25, 40 and 60 minutes.
- A 7-day login calendar that pauses a streak rather than resetting it.
- A daily free spin.
- An offline earnings popup with an optional 2× (from a rewarded ad the player starts themselves, or from a pass).
- A codes button.
- Friend boost: +X% per friend in the server.

---

## 6. Monetization patterns

**Price passes to fit Robux pack sizes.** Packs are 80, 400, 800, 1,700 and 4,500 Robux. Kids think in packs, so price at 99, 199, 399, 799 or 1,299.

| Tier | Price (Robux) | What sells at this price |
|---|---|---|
| Impulse | 9–99 | Instant hatch, revive, "double this run", restock skip, tool slots |
| Core passes | 139–499 | 2× Money, 2× Luck, Auto-collect, extra egg slots, faster hatch |
| Status / anchor | 499–1,299 | VIP, hero classes (Head Nurse 190, Secret Agent 890), premium egg |
| Whale | 1,999–4,999 | Admin-command passes (Steal a Brainrot), Admin treadmill |

**What converts:**
- **Prompt when the player wants something**, never when they join:
  - after a near-jackpot
  - when inventory is full
  - while your pet is being stolen ("Lock base 10 min")
  - on the death or results screen (revive, double this run)
- **Convenience that removes friction the player already feels:** auto-collect, skip animation.
- **Luck boosts and server-wide luck passes.** Buying one benefits everyone in the server, so it feels generous.
- **Gifting.**
- **Robux-only hero characters fans love.**

**Algorithm link:** "spend days" is a ranking signal. One cheap purchase early in a player's life is worth more than one big purchase later.

**Compliance (required):**
- Anything bought with Robux (directly, or through a currency bought with Robux) that gives a random result must **show odds as percentages that add up to 100%** before purchase.
- Luck boosts must state their effect, and the displayed odds must update while the boost is active.
- The game must check `PolicyService.ArePaidRandomItemsRestricted` and `IsPaidItemTradingAllowed`.
- Free random drops need no odds disclosure, but showing "1 in X" is good UX anyway.

---

## 7. Marketing and distribution: how a game actually gets out

### The 2026 algorithm (Recommended For You, which drives about 90% of game traffic)

| Weight | Signals |
|---|---|
| **Most important** | Play-through rate (impression → play); **first-play bounce under 60s and at 61–180s (negative)**; play days (day 1, days 2–7, days 8–28); playtime (capped at 60 min per day) |
| **Important** | **Days spent playing intentionally with friends** (joining a friend, invites, private servers); qualified sessions; **days with a purchase**; Robux per user |

How it works in practice:
- **Getting into the candidate pool needs very few plays from any source.** Ads, search, friends and social links all help.
- **Ranking only counts players who arrived organically from Recommended For You.**
- **Similarity detection:** games whose metadata *and place files* resemble existing games are deprioritized. Clones need original art and a real change to the loop.

### The two gates for a brand-new game
1. **Under-16s can't see it at first.** Only age-checked players aged 16+ can see a new game until it reaches **500 highly engaged players** within 60 days.
   - It also needs a refundable 1,000 Robux fee (or two months of Roblox Plus), plus an age-checked, ID-verified creator account with 2-step verification.
   - **Ads Manager's "Engagement" objective** buys exactly this audience.
2. **Momentum.** Developers report that about **50–100 steady CCU for about a week**, with decent retention, gets a game picked up by the algorithm.

### Packaging
- **Thumbnails:** upload 3–5 and use Roblox's built-in A/B test (thumbnail personalization), which Roblox reports gives +8.5% average play-through and up to +50%.
  - Style: one big character or collectible, a shocked face, saturated colors, a rarity glow, big numbers.
  - Keep text away from the bottom edge, where the player-count overlay sits.
  - **The thumbnail must match the first 60 seconds**, or the bounce penalty cancels the click.
  - Add a gameplay video thumbnail (3 uploads a month, real gameplay only).
- **Title:** "Verb a Noun" in fresh wording, with a status tag (`[🎃]`, `[UPD]`). Never mention Robux rewards.
- **Description:** natural language with genre words. Search understands meaning now ("food games").

### Short-form video (TikTok, Shorts, Reels)
- **It drives "what's this game called?" searches.**
- Searches for the game's name, and visits through our share links, also earn **Creator Rewards: 35% of a new player's first $100 of spending**.
- **Formats that work** (views from a creator's self-reported 30-day test):

  | Format | Avg views |
  |---|---|
  | Glitch or exploit discoveries | 890K |
  | Horror jumpscare reactions | 720K |
  | "POV: you find…" | 540K |
  | Secret locations | 480K |
  | Before and after an update | 310K |
  | **Plain gameplay** | **42K** |

  Also: rare reveals, "I stole the rarest…", trade scams, Admin Abuse chaos, "Night 1 vs Night 99", friend betrayal.
- **The first 1.5 seconds decide whether people keep watching.** Post 3–5 times a day. Use trending sounds early.
- **Clipping campaigns** pay about $1–1.50 per 1,000 verified views. Studios seed their own clips this way.
- **Roblox's own social accounts and curation team** can start a breakout. Roblox's TikTok post about Dead Rails led to 600K+ CCU.

### Creators
- YouTubers amplify a game that is already trending; they rarely start the trend.
- Start with **small and mid-size creators** (10K–500K subscribers): give them free passes or admin perks, and put no restrictions on recording.
- Go to Roblox's Video Stars program and the big creators once the game retains players.
- **The developer as streamer:** the Admin Abuse sessions run by Jandel and Sammy were themselves the content.

### Loops built into the game
- **Referral rewards** for both inviter and invitee (tracked with `ReferredByPlayerId`). Games that prompt invites in-game get **6× more players sending invites**.
- **Share links** (`PromptLinkSharing`) that deep-link straight into the action.
- Free or cheap private servers, which count as intentional co-play.
- Rewards for likes and group joins, codes released at like milestones.
- **Roblox's Experience Events feature,** with a countdown and a "Notify Me" button.
- **Update notifications.**
- **Note:** social links on a game page (Discord etc.) are hidden from under-16s since June 2026, so the in-game channels carry most of the weight.

### Timing
- **Saturday is the weekly peak,** around 19:00 UTC and about 16M CCU. Tuesday morning is the low point.
- Release updates on Friday or Saturday, with Admin Abuse about an hour before.
- **Holiday windows are worth 3–4× normal traffic.** The next one is the **US Thanksgiving to New Year break**.

---

## 8. Trend cycles: where the next breakout is likely to come from

**Waves are getting shorter and faster.** In 2025, a mega-hit took about 5 months to reach its peak. In 2026, Steal An Egg took 8 weeks and Break and Steal an Egg took 19 days. Waves last about 2–3 months, and **20–50 clones appear within 2–4 weeks** (26 clones of the Steam hit MECCHA CHAMELEON appeared in 3 weeks).

**The collectible noun rotates every 3–6 months; the verbs last longer.**
```
brainrot (2025) → lucky block (spring 2026) → egg/pet (summer–fall 2026) → animals/mounts: cats, dinos (forming now)
Verbs that persist: steal · grow · +1 · escape · survive N nights · ride
```

**Hook types compared:**

| Hook | Peak potential | Longevity |
|---|---|---|
| Steal from others (raid + base defense) | **10–26M** | Fast decay, but a large tail |
| Idle / offline growth | 3–22M | Medium |
| Survive N nights / co-op survival | 1.5–14M | **Long** |
| Numbers go up (+1, escape obby) | 1.5–6M | Medium (kept alive by reskins) |
| Luck / rarity (lucky block, hatch) | 0.7–1.7M | Short–medium |
| Ride or drive an X | 0.1–1.6M | Short |
| Anomaly job sim | 0.1–1.2M | Short |
| PvP skill, social judging (Dress To Impress), fishing | ≤1.7M | **Longest** (years) |
| Steam ports, brands, regional | 50–300K | Short |

### Gaps open right now (late Oct 2026)

| Opportunity | Evidence |
|---|---|
| **Cats** as the next animal noun | Cat Battles grew nearly 500% in a week |
| **Dinos and mounts** | Ride a Dino +404% in a week; no dominant game yet |
| **Ragdoll / physics chaos** | Ragdoll Reality +2,525%; no 1M+ ragdoll game since Fling Things |
| **Tesla Roadster "kickflip" meme** | ~98M views; no Roblox game yet |
| **GTA VI launches Nov 19** | Most kids can't play it. A kid-safe "steal a car / heist city" game, with no Rockstar IP |
| **Steam Next Fest hits not yet on Roblox** | Worst Class Ever (classroom hide-and-seek), Probably Stolen (fencing stolen goods), Dumpster Gang (raccoon heist), Bombanana (co-op where players are deaf, mute or blind) |
| **Anomaly jobs that aren't food or vet** | Airport security X-ray, pharmacy, cashier |
| **Winter / Christmas reskin window** | A hazard-escape game ("Escape the Blizzard") or a seasonal version of a proven loop |
| **Occult ghost-hunt co-op** | Demonology +561%; SCP and liminal spaces rising |
| **Absurd consumption** | "Eat Everything In A Grocery Store" +414% |
| **Regional** | Arabic games at 100–122K; Karinderya at 294K. Indonesia, Brazil and the Middle East / North Africa are underserved. |

---

## 9. Viral Fit Score: a rubric for judging ideas in brainstorming

Score each concept from 0 to 3 on each criterion, then multiply by the weight. The maximum is 105.

| # | Criterion | Weight | What a 3 looks like |
|---|---|---|---|
| 1 | **Title = rule** | 3 | A child understands the whole game from the title and icon in under 5 seconds |
| 2 | **30-second core moment** | 3 | The first fun action happens in under 30s, with no tutorial |
| 3 | **Clip moment** | 3 | A 3-second vertical clip makes sense with no context (reveal, theft, splash, scare, swarm) |
| 4 | **Fresh noun on a proven verb** | 3 | Uses a verb with a 1M+ history, plus a noun that is rising and not yet owned |
| 5 | **Social friction or co-op** | 2 | Stealing, betrayal or forced teamwork produces emotion and pulls in friends |
| 6 | **Collectible depth** | 2 | Rarity tiers, mutations, "1 in X" odds, an Index, items others can see |
| 7 | **Climbing number / counter** | 2 | Speed, $/s, nights or shifts climb forever, and players can brag about it |
| 8 | **Return hooks** | 2 | Offline progress, timers, daily rewards (covering the algorithm's day 2–7 and day 8–28 windows) |
| 9 | **Shared clock / events** | 2 | Server-wide restocks, weather, and a hook for Admin Abuse |
| 10 | **Monetization at the moment of desire** | 2 | Natural spots for revives, luck, 2×, auto-collect and hero cosmetics, all compliant |
| 11 | **Mascot potential** | 1 | Characters fans would draw or animate |
| 12 | **Seasonal and update extensibility** | 1 | Easy to add biomes, stages, eggs or reskins every week |
| 13 | **Cheap to build** | 3 | An MVP in 2–3 days with simple systems |
| 14 | **Policy-safe** | 2 | No IP, no reward feeds, odds can be disclosed, and the game can be shown to kids |

---

## 10. Building in 2–3 days: what is cheap and what is expensive

The research shows viral MVPs are usually **simple**. Grow a Garden's first version took about 3 days. DONT SPLASH is an obby with one monster. +1 games are a treadmill and a stage. The polish and depth came later through weekly updates.

| Cheap (hours) | Medium (about a day) | Expensive (avoid for the MVP) |
|---|---|---|
| A climbing stat plus leaderstats | Plot or base system with pedestals and $/s income | Smart AI monsters with pathfinding and perception |
| Conveyor or spawn-reset timer | Steal-and-carry with an owner alert and base lock | Full trading UI with anti-scam protection |
| Rarity tables, mutations, "1 in X" | Hatch/reveal sequence with all the visual effects | Many hand-built biomes |
| Floating numbers, counter pop, sounds | DataStore saving with session locking | Custom vehicle physics |
| Obby stages with one hazard rule | A single simple chaser (Guardian or water monster) | Complex co-op roles and voice-dependent mechanics |
| Like/group reward, codes, playtime gifts | Rebirth loop; server-wide events (weather, luck) | Story, lore, cutscenes |
| Gamepasses and dev products | Seasonal reskin | Large-scale combat balancing |

**The 2–3-day viral kit (ship with all of these):** a "Verb a Noun" title and 3–5 thumbnails · spawn on your own plot or in a party · a beam guiding you to the one verb · first reward in under 30 seconds with a full reveal · a rarity ladder with 1–2 mutation layers · a climbing number with abbreviations · an owner alert or server announcement on big moments · a 5-minute shared clock · a like and group reward that skips early progress · playtime gifts up to 10+ minutes · 2× pass, luck pass, an impulse product · offline earnings popup · saving · rarity color system and sounds · a hook for Admin Abuse (luck multiplier and spawn controls) · referral rewards and share links · an Experience Event for the first Saturday.

---

## 11. Concept seeds for brainstorming, scored

These are starting points, not decisions. Scores use the rubric in §9.

| Concept | Formula | Why it fits | Rough score |
|---|---|---|---|
| **Steal a Cat** | Steal + hatch loop, with cats as the noun | Cats are trending (+500%). Proven top-tier verb. Cute mascots. The egg lane is crowded, so it needs a twist (e.g. cats that grow "chonkier", with size as a mutation) | ~88 |
| **Ride a Dino, Steal Its Eggs** | Ride-collect + egg-steal | Combines the two hottest October verbs. The mount you hatch is your speed | ~84 |
| **Escape the Blizzard for Pets** | Hazard-escape collection (the Escape Tsunami format, 4–5M) + winter theme | Ready for the December holiday spike. Simple to build | ~84 |
| **Don't Wake the ___** (one-rule horror obby) | DONT SPLASH format with a new sense rule (e.g. "it sees movement", "it hears footsteps on snow") | Cheapest to build. Very easy to clip. A Push tool for betrayal. Lower ceiling and fast decay unless it gets collectibles | ~80 |
| **Steal a Car: Heist City** | Steal-tycoon with a garage base, rarity cars and mutations (paint finishes) | GTA VI hype on Nov 19 for kids who can't play it. Cars clip well. Must stay IP-free | ~82 |
| **Airport Security (Anomaly)** | Anomaly job sim with X-ray spot-the-difference | Comment-bait "can you spot it?" clips. A known gap. Shorter lifespan | ~74 |
| **Raccoon Heist: Steal Trash** | Steal-tycoon with raccoons and gross-out collectibles | Dumpster Gang was a Next Fest hit. Animal + steal + humor | ~78 |
| **Ragdoll ___ (physics chaos + collection)** | Fling or ragdoll toy plus "+1" or collect progression | Physics chaos is rising with no 1M+ owner. Clips well. Harder to hold retention | ~72 |

---

## 12. Policy landmines (lessons from things that already got punished)

- **No "watch content for rewards" feeds.** Steal An Egg was pulled over this and Roblox changed its rules.
- **No other people's IP or meme characters you don't own.** Tung Tung Tung Sahur was removed during a licensing dispute, and Spyder Games has filed at least 4 lawsuits.
- **No copied code or assets.** Steal An Egg was accused of reusing decompiled Pet Sim 99 code. Similarity detection also hides clones.
- **No "Free Robux" or reward promises in metadata or invites.** Roblox says they reduce distribution.
- **No fake timers, permanent sales, or near-miss visuals on paid rolls.** Researchers are watching, and enforcement is likely to tighten.
- **Disclose odds and check PolicyService** for any paid randomness.
- **Thumbnails must show the actual game.**

---

## Key sources (full lists are in the research notes)

**Platform and official**
- Discovery and algorithm: [Roblox Newsroom: Optimizing Discovery](https://about.roblox.com/newsroom/2026/06/optimizing-discovery-great-games-reach-millions-players-roblox), [DevForum: RFY algorithm update](https://devforum.roblox.com/t/recommended-for-you-algorithm-improvements-that-better-value-long-term-retention/4684575), [Discovery docs](https://create.roblox.com/docs/discovery.md)
- Kids & Select gate: [DevForum announcement](https://devforum.roblox.com/t/roblox-kids-and-select-global-launch-upcoming-updates-to-eligibility-ads-manager-and-expedited-review/4685717), [docs](https://create.roblox.com/docs/production/publishing/kids-and-select)
- Monetization and payouts: [Creator Rewards](https://create.roblox.com/docs/creator-rewards), [Paid Random Items](https://create.roblox.com/docs/production/monetization/paid-random-items), [Monetization guidelines](https://create.roblox.com/docs/en-us/production/monetization)
- Product docs: [Onboarding](https://create.roblox.com/docs/production/game-design/onboarding), [Thumbnails](https://create.roblox.com/docs/production/publishing/thumbnails), [Ads Manager](https://create.roblox.com/docs/production/promotion/ads-manager), [Referral system](https://create.roblox.com/docs/production/promotion/referral-system), [Share Link API](https://devforum.roblox.com/t/introducing-the-share-link-api-deep-link-players-directly-into-the-action/3972678), [Experience Events](https://create.roblox.com/docs/production/promotion/experience-events)

**Analytics and industry reports**
- GameAnalytics: [Roblox report](https://www.gameanalytics.com/reports/2026-roblox-report), [Dead Rails "Hit Makers"](https://www.gameanalytics.com/blog/dead-rails-and-the-hit-makers-formula)
- Trackers: [RoWatcher: brainrot CCU decline](https://rowatcher.com/news/is-the-brainrot-trend-dying-what-ccu-data-from-three-top-games-reveals), [RoWatcher: Oct 17 week](https://rowatcher.com/news/roblox-week-of-oct-17-ccu-surges-cats-battle-dinos-ride), [RoWatcher: busiest hours](https://rowatcher.com/news/when-is-roblox-busiest-we-mapped-every-hour-of-the-week), [RBLXSTAT records](https://rblxstat.com/lists/record-breaking-roblox-games)
- Research and press analysis: [University of Sydney monetization study](https://www.sydney.edu.au/news-opinion/news/2026/05/17/inside-the-pay-to-play-world-of-roblox-targeting-children-.html), [Beebom on Admin Abuse](https://beebom.com/admin-abuse-might-save-dying-roblox-games-but-hurts-them-in-the-long-run/amp/), [Tubefilter: Admin War record](https://www.tubefilter.com/2025/08/25/roblox-grow-garden-steal-brainrot-admin-war-record/amp/)

**Steal An Egg**
- Guides: [beginner guide](https://allthings.how/steal-an-egg-beginner-guide-biomes-speed-and-pets-explained/), [mutations](https://allthings.how/steal-an-egg-all-mutations-and-multipliers/), [eggs and income](https://games.gg/roblox/guides/steal-an-egg-all-eggs-pets-and-income-rates/), [Sammy update](https://allthings.how/steal-an-egg-sammy-is-coming-update-patch-notes-and-dr-scramble-event/)
- Reels-feed crackdown: [Kotaku](https://kotaku.com/roblox-cracks-down-on-doomscrolling-games-like-steal-an-egg-that-forces-players-to-watch-reels-while-running-on-a-treadmill-2000727952), [MassivelyOP](https://massivelyop.com/2026/08/29/roblox-clamps-down-on-gen-ai-brainrot-scrolling-games-after-steal-an-egg-goes-viral/)

**Other collect/steal hits**
- Wikipedia: [Steal a Brainrot](https://en.wikipedia.org/wiki/Steal_a_Brainrot), [Grow a Garden](https://en.wikipedia.org/wiki/Grow_a_Garden)
- [Beebom: Steal a Brainrot engagement](https://beebom.com/robloxs-steal-a-brainrot-delivered-a-2025-masterclass-in-player-engagement-and-gave-uefn-a-second-wind/)
- [Break and Steal an Egg pickaxes](https://roonby.com/2026/10/19/break-and-steal-an-egg-pickaxe-tier-list-all-pickaxes-costs-and-power/amp/)
- [Ride A Pet guide](https://allthings.how/ride-a-pet-on-roblox-how-to-play-full-guide/)
- [Kick a Lucky Block luck guide](https://techwiser.com/kick-a-lucky-block-increase-luck/)

**Horror, survival and chaos**
- DONT SPLASH: [how to play](https://dontsplash.wiki/guide/dont-splash-how-to-play), [Rolimons stats](https://www.rolimons.com/game/119958473240233)
- Animal Hospital: [how the night shift works](https://allthings.how/animal-hospital-anomaly-on-roblox-how-the-night-shift-and-anomalies-work/), [Know Your Meme](https://knowyourmeme.com/memes/subcultures/animal-hospital-roblox)
- [Sell Fries beginner guide](https://games.gg/roblox/guides/sell-fries-beginners-guide/)
- [Huss Valley beginner guide](https://games.gg/roblox/guides/huss-valley-beginners-guide/)
- [99 Nights in the Forest film deal](https://www.thewrap.com/creative-content/movies/20th-century-studios-roblox-game-99-nights-in-the-forest/)

**Trends**
- [Kotaku: MECCHA CHAMELEON clones](https://kotaku.com/more-people-are-playing-meccha-chameleon-knock-offs-than-the-original-hit-steam-game-as-the-roblox-clone-machine-goes-into-overdrive-2000715371)
- [Steam Next Fest Oct 2026](https://accountshark.net/blog/steam-next-fest-october-2026-most-played-demos-what-to-play-before-it-ends)
