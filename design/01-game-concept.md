# Steal a Car — Game Concept

*Working title. Alternative: "Heist City". This document describes the whole game, its systems, the game theory behind it and its social design. It does not cover how to build it. For the research behind these decisions, see `research/01-market-research-oct-2026.md` and `research/02-viral-dna-deep-dive.md`.*

---

## 1. What it is

**Steal a Car** is a free, multiplayer, open-world crime game on Roblox. It gives players the GTA fantasy (stealing cars, robbing, shootouts, heists, cops, crews) in a form Roblox's young audience can play, can share, and will return to every day.

Underneath the open world is a simple, addictive collection loop: **steal a car, get it home, and it earns money forever.** Everything else in the game (guns, police, crews, heists, races, the city itself) exists to make that loop more exciting, more social, and riskier.

**One-line pitch:** *"Steal cars, build the sickest garage in the city, and protect it from everyone else trying to do the same."*

**Why now:** GTA VI launches Nov 19, 2026. It is $80, rated M, and ships **without** an online mode. Millions of kids will see the hype and can't play it. We are the free version they can play with their friends that same week.

**Audience and rating:** ages 9+ (Roblox "Moderate" content rating). Violence is non-graphic: there is no realistic blood, players ragdoll and respawn, and police "bust" players rather than kill them. The game is mobile-first and also plays well on PC.

---

## 2. The core idea: the garage is a bank, the street is a casino

Every system in the game feeds one tension.

- **Parked in your garage**, a car earns money every second, including while you're offline. It is mostly safe.
- **Out on the street**, the same car earns several times more through missions, heists, races and robberies, and its speed and armor actually matter. But it can be carjacked, wrecked or impounded.
- **Upgrades improve both sides.** A better car earns more in the garage and performs better on the street. **Your best cars are the ones you most want to show off, and the ones everyone else most wants to take.**

This tension is why the game doesn't get stale. Players are always choosing between playing it safe and going big, between protecting what they have and chasing more.

---

## 3. The player experience

### The first minute
You spawn inside your own small garage, with your name on the sign. An arrow points out the door to a beat-up car parked on the curb. You hold a button to hotwire it; a short timing bar gives a faster start if you nail it. The engine roars, one wanted star lights up, and a police siren starts behind you. You floor it back to your garage, the door slams shut behind you, the car rolls onto its parking spot, and a counter starts ticking: **+$5/s**. That's the whole game in 30 seconds.

### The first ten minutes
The game opens up one piece at a time:

| Minute | What unlocks |
|---|---|
| 1–2 | Your first upgrade, so your income visibly jumps |
| 2–4 | The chop-shop order board gives you a target ("Bring me any blue car in 3 minutes") |
| 4–6 | A free pistol, and the server-wide announcement that an armored truck is rolling through downtown |
| 6–10 | Your first raid alert, when someone is breaking into a garage nearby. A prompt invites a friend to form a crew. A rare car spawn is announced to the whole server. |

### A typical 20-minute session
1. Log in to an offline-earnings payout.
2. Check the order board. Hunt a specific car across two districts.
3. Defend your garage when the door lock drops.
4. Join the server-wide rush for the armored truck.
5. Level up your favorite car.
6. Run a bank heist with your crew.
7. Lose your wanted stars at a paint shop.
8. Log off just as the next restock timer says "Rare spawn in 4:00", which gives you a reason to come back.

### What a long-term player is chasing
- A complete car collection.
- One-of-a-kind limited cars with serial numbers.
- A garage empire across several districts.
- A top crew that controls city turf.
- A legendary Rep rank.
- A spot on the "Most Wanted" leaderboard.

---

## 4. The city

**Setting:** a stylized, colorful, sun-soaked city. It is an original setting (no real-world or Rockstar names), with a coastal downtown, palm trees, neon nights and a cartoonish, chunky art style. It is cheerful and exaggerated, not gritty.

**Districts act as soft progression gates.** Anyone can go anywhere. Richer districts spawn better cars but have heavier police, so escaping them takes a stronger car.

| District | Spawns | Police | Feel |
|---|---|---|---|
| Junkyard / Docks | Beaters, Sedans | Light | Starter zone, rusty and chaotic |
| Suburbs | Sedans, Sports | Light–Medium | Driveways, cul-de-sacs, easy targets |
| Downtown | Sports, Muscle | Medium | Traffic, banks, stores, the action hub |
| Beachfront | Muscle, Super | Medium–High | Showrooms, flex spot, race strip |
| The Hills | Super, Hyper | High | Mansions with private garages |
| Airport / Port | Hyper, Secret | Very high, helicopters | Endgame: cargo planes, shipping containers, rarest spawns |

**A living world:**
- NPC traffic and pedestrians.
- **Day/night cycle.** Night brings rarer spawns but more aggressive cops.
- **Weather events** (rain, fog, heatwave, thunderstorm) change driving and spawn odds. A thunderstorm can "charge" cars with an Electric finish, the same way Grow a Garden's weather mutated crops.
- **City events.** A *blackout* shuts down police radios for 3 minutes. A *parade* closes Downtown streets. A *supercar expo* spawns showroom cars that can be stolen.

---

## 5. Cars: the collectible

Cars are the heart of the game. A car is a trophy, a tool, an income source and a target all at once.

**Rarity tiers:**

| Tier | Example (original designs) |
|---|---|
| Beater | rust bucket, mail van |
| Sedan | family car, taxi |
| Sports | hatchback, roadster |
| Muscle | classic V8 |
| Super | low exotic |
| Hyper | concept hypercar |
| Secret | prototype, armored limo, jet-car |

**Value layers.** These stack multiplicatively, which produces the "1-in-X" bragging moments:
- **Paint finish (mutation):** Matte → Metallic → Chrome → Gold → Neon → Rainbow → Glitch / Void / Galaxy. Each multiplies value.
- **Traits:** special properties that can roll on a car, such as *Turbo*, *Bulletproof*, *Classic*, *Prototype* or *Stolen from a cop*.
- **Level:** cars gain XP from driving, missions and races. Higher levels mean more income and better stats.
- **Upgrades:** engine, armor, nitro, tires, handling. Each one is a money sink that also makes the car more desirable.
- **Limited editions:** event and seasonal cars that never return, some with **serial numbers** ("#7 of 500").

**Rare spawns are announced to the whole server:**
- *"A 1-in-5,000 Gold Hypercar just spawned at the Airport!"*
- The whole server stampedes to it.
- This is the game's signature clip moment.

**Car Collection Book (Index):**
- Shows silhouettes of every car and finish not yet owned.
- **Set bonuses** for completing a group, e.g. "all Muscle cars" or "every Gold finish".
- Limited cars that are gone leave permanent gaps, which creates collector FOMO.

**Customization (pure self-expression, a big part of the flex):**
- Wraps, rims, spoilers, underglow neon, tinted windows, custom horns.
- **Custom license plates.** Plates players write themselves are clip and meme fuel.

---

## 6. The garage: your base, bank and trophy room

- **Starts small** (a couple of parking spots) and expands into multi-floor garages, then **safehouses in other districts**.
- **Parked cars earn money per second**, including offline earnings up to a cap.
- **Showroom:** other players can walk past or visit, see your collection with income labels, and like your garage. Garages are a status display.
- **Door lock:**
  - The garage is safe while the lock is active.
  - When it expires, the garage can be raided until you re-lock it. Lock duration grows with upgrades and Rep.
  - The owner gets an alert ("Someone is breaking into your garage!") and can rush home.
- **Defenses:** reinforced doors, alarms, traps such as spike strips, oil slicks and a guard dog. Crewmates can defend too.
- **Favorite spot:** one car slot (expandable) that can never be stolen. This protects the car a player cares most about.

---

## 7. The ways to make money (and the risk of each)

| Activity | Payout | Risk | Notes |
|---|---|---|---|
| Garage income | Steady, passive | Low (raids) | The idle backbone |
| Chop shop | Sell stolen cars for instant cash | Low | Order board pays a bonus for specific cars on a timer |
| Robbing stores | Quick cash | +1 star | Gas stations, jewelry stores, ATMs. Skill-timed mini-actions |
| Robbing players (mugging) | Their carried (unbanked) cash | Medium | The reason cash on hand vs. banked matters |
| Carjacking players | Their car, upgrades included | High | Triggers a chase and a bounty |
| Raiding garages | Their parked cars | High | Only while the lock is down. The owner is alerted |
| Armored truck (every 5 min) | Big cash bag | High, server-wide | The shared clock. Everyone converges |
| Bank heist (timed event) | Huge | Very high, crew | Multi-stage, needs roles and good cars |
| Street races | Prize money, or **pink slips** | Variable | Bet your car against theirs |
| Bounty hunting | Bounty value | Medium | Take down the most-wanted players |
| Police work (cop role) | Arrest rewards | Medium | See §9 |
| Businesses (later) | Passive | Low | Car wash, nightclub, tuning shop |

**Cash on hand vs. banked.** Cash you carry can be stolen, and some of it drops when you're busted or taken down. Cash you deposit (at your garage or an ATM) is safe. Every player constantly decides whether to bank now or push for more.

---

## 8. Combat, guns and trolling

- **Weapon ladder:** pistol → SMG → shotgun → rifle → special/heavy weapons, unlocked by Rep and bought with cash.
- **Ammo is a consumable** and a steady money sink.
- **Uses:**
  - Carjacking (shoot out tires, pull the driver out).
  - Defending your garage.
  - Fighting cops.
  - Robberies.
  - Heist shootouts.
- **Melee and non-lethal tools:** bat, taser, smoke grenades, spike strips, EMP to stall engines.
- **Takedowns are non-graphic:** the player ragdolls and respawns at a hospital for a small fee, and drops part of their carried cash.
- **Trolling is built in on purpose:**
  - Ragdoll physics, flinging, ramming.
  - Ramming knocks cash loose from players.
  - Trolls earn wanted stars, which eventually makes them the hunted.

---

## 9. Police, heat and the law

**Wanted stars (1–5) are the risk dial.**
- Every crime adds heat.
- More stars bring heavier police: patrol cars → roadblocks → SWAT → helicopters → special units at 5 stars.
- Payouts rise with stars, up to roughly 3× at 5 stars. Pushing your luck is literally profitable.
- **At 5 stars, a server-wide bounty** goes on you. Your location is periodically pinged to everyone.
- **"Longest at 5 stars"** is a leaderboard and a natural video series.
- Lose stars by escaping line of sight, hiding in your garage, or repainting at a paint shop.

**Busted vs. taken down:**
- **Busted** by police: you go to jail and your car is impounded. You can pay a fee to retrieve it, or break it out.
- **Taken down** by players: you ragdoll, respawn at the hospital and drop carried cash.

**Jail is a mini-game, not a timeout.** Serve a short sentence, or attempt a **jailbreak**: dig, sneak, or have your crew break you out. Getting busted becomes another adventure.

**Player cops (optional faction, strongly recommended):**
- Players can choose to play as police, earning money by busting high-star criminals and recovering stolen cars.
- This gives the game a second playstyle and natural counterplay.
- It makes chases player vs. player, which are far more dramatic than chases against AI police.

---

## 10. Crews: playing with friends

- **Crews of 2–4** (later, larger crews with ranks).
- **Friend bonus:** extra cash for each crewmate in the server.
- **Shared crew garage** and crew colors, decals and plates.
- **Crew heists need roles:**
  - *Driver* for the getaway.
  - *Gunner* to hold off cops.
  - *Hacker* to crack vaults and disable alarms.
  - *Lookout* to call out incoming threats.
- **Crew Rep, crew levels, crew leaderboards.**
- **Crew turf (later):** crews compete to control districts and earn passive cut and bragging rights. It is a server-level meta-game.
- **Crew betrayal (optional, high-drama):**
  - After a heist, the loot bag is physical, and anyone holding it can run.
  - Splitting fairly is the default.
  - Betrayal is possible but publicly tagged ("Backstabber") and costs Rep.
  - This is the prisoner's dilemma, and it produces viral drama.

---

## 11. Heists and missions

**Heist structure (bank, jewelry store, casino, cargo plane, armored convoy):**
1. **Prep:** steal the right getaway car, buy gear, scout the target.
2. **The job:** choose loud or stealth. Crack the vault (mini-game) and hold off police waves.
3. **The getaway:** a multi-star chase to a drop-off point.
4. **The split:** carry the bag home.

**Timed server events:**

| Event | Timing |
|---|---|
| Armored truck | Every 5 minutes |
| Bank heist window | Every 30 minutes |
| Rare-car spawn | Every 10–15 minutes |
| Supercar expo | Hourly |

**Small jobs** (1–3 minutes, mostly solo):
- Chop-shop orders.
- Deliveries under a timer.
- Taxi rides with chaotic NPC passengers.
- Stunt jumps.
- "Lose the cops" challenges.
- Repo jobs.

---

## 12. Street racing

- **Races:** sprint, circuit, drag, drift, and time trials across the city.
- **Pink-slip races:** both players stake a car and the winner keeps both. This is the purest high-stakes moment in the game and pure clip material.
- **Race skill matters:** nitro timing, drifting and racing lines. A well-driven lower-tier car can beat a badly driven hypercar.
- Racing gives cars XP and gives upgrades a purpose beyond income.

---

## 13. Losing things (and why players don't quit)

A game about stealing has to make losing hurt **without** making people quit.

- **Insurance:** when a car is stolen, the owner gets back part of its value. A higher insurance tier is an upgrade.
- **Repo:** your stolen car is marked in the thief's garage, so you have a revenge target to steal back.
- **Favorite slot:** your most precious car can never be taken.
- **Protections:**
  - New-player protection for the first few minutes.
  - Spawn and garage safe zones.
  - Lock timers.
  - Bounties on serial griefers.
- **Catch-up mechanics:**
  - The richest player in the server is always worth more to rob and carries a bounty.
  - Bounties scale with how much someone has stolen.
  - The game naturally pulls the leader back toward the pack.

---

## 14. Long-term progression

- **Rep rank:** permanent and always climbing. It unlocks districts, weapons, garage space and cosmetics, and is shown above your head.
- **Car mastery:** each car model has its own mastery levels with small perks.
- **Collection completion:** sets, finishes and limited serials.
- **Prestige ("Go Legit" / "Retire"):** cash out your empire for a permanent income multiplier and an exclusive badge, car or plate, then rebuild faster.
- **Empire layer (later):** properties and businesses (car wash, nightclub, tuning shop, dealership) that generate passive income and can be raided or defended.
- **Seasonal leaderboards:** Richest, Most Wanted, Best Garage, Top Crew, Fastest Racer, Top Cop.

---

## 15. The economy

**Sources** (money in):
- Garage income.
- Chop shop.
- Robberies.
- Heists.
- Races.
- Bounties.
- Police work.
- Businesses.

**Sinks** (money out):
- Upgrades.
- Ammo.
- Repairs.
- Impound fees.
- Hospital fees.
- Insurance.
- Garage expansion.
- Cosmetics.
- Bail.
- Heist prep gear.
- Fees for lowering wanted stars.

**Transfers** (money moving between players):
- Mugging.
- Carjacking.
- Raids.
- Pink slips.
- Bounties placed by players.
- Trading.

**Player trading:**
- Cars and cosmetics can be traded through a safe two-sided trade window.
- Rare finishes and limited serials become a status economy, the way pets work in Adopt Me or knives in Murder Mystery 2.

**Player-placed bounties:**
- Anyone can put a cash bounty on another player.
- Revenge becomes an economy, and grudges become content.

---

## 16. Game theory behind the design

| Concept | Where it lives in the game |
|---|---|
| **Risk vs. reward** | Garage vs. street; banked vs. carried cash; wanted-star multipliers; pink slips |
| **Loss aversion** | Your cars are physically visible and stealable, so you protect them, stay online and come back for revenge |
| **Endowment effect** | Your named garage, your customized car with a custom plate |
| **Variable rewards** | Rare spawns, finish rolls, trait rolls, crate contents, heist loot |
| **Prisoner's dilemma** | Crew loot splits and the option to betray |
| **Tragedy of the commons / scramble competition** | Everyone rushing the same armored truck or rare spawn |
| **Deterrence** | Visible garage defenses, crew presence, insurance and repo making raids costly |
| **Signaling and status** | Rare cars, finishes, plates and Rep shown publicly; garage showrooms; serial numbers |
| **Catch-up / anti-snowball** | Bounties on leaders, a richest-player target, insurance, newbie protection |
| **Goal gradient** | Districts, car levels and collection sets that are always "almost there" |
| **Asymmetric roles** | Criminal vs. cop, driver vs. gunner vs. hacker |
| **Reciprocity and alliances** | Crews, defending friends, shared bonuses, gifting |
| **Appointments** | Offline earnings, timed events, daily contracts, weekly updates |
| **Hot potato** | Whoever carries the heist bag or the armored-truck loot is visible, slowed and hunted |

---

## 17. Social interaction

- **Every player is both a threat and an opportunity.** That creates rivalries, revenge arcs, alliances and betrayals.
- **Server-wide moments pull everyone together:**
  - Rare spawns.
  - Armored trucks.
  - Bounty chases.
  - Five-star rampages.
  - Admin Abuse events.
- **Spectacle:** chases and getaways are watched by the whole server and shown on the minimap. Everyone sees the drama.
- **Communication without relying on chat.** Many young players have chat restricted, so the game provides:
  - Quick-chat callouts ("Need backup!", "Cops!", "Nice car!").
  - Emotes.
  - Car horns.
  - Pings on the map.
  - Gifting.
- **Garage visits and likes**, "best garage" leaderboards, and showroom tours.
- **Photo mode and highlight moments** for sharing clips.
- **Friend invites with rewards** for both sides, and a bonus for playing together.

---

## 18. Live-ops: the game changes every week

- **Weekly Saturday update:**
  - 3–5 new cars.
  - A new paint finish or trait.
  - A new heist, district, event or weapon.
- **"Admin Abuse" live event about an hour before each update.** The developers show up in-game and run:
  - **Hypercar Rain:** rare cars falling from the sky.
  - **Police Strike:** no cops for 15 minutes.
  - **10× Gold-paint luck.**
  - **Golden armored truck.**
  - **Everyone gets 5 stars.**
- **Seasons** (6–8 weeks), each with a theme, a car pass, and a seasonal city reskin. Examples: winter city with snow drifting, summer beach, Halloween night city.
- **Limited-time cars** that never return.
- **Crossovers and collabs** with other games or creators.

---

## 19. Monetization (fair, never pay-to-win at the core)

- **Passes:**
  - 2× Cash.
  - VIP: bigger garage, longer lock, a VIP tag.
  - Extra garage slots.
  - Better insurance.
  - Auto-collect.
  - Bigger favorite-car protection.
- **Cosmetics:**
  - Wraps, neon, horns, outfits, heist masks, plates.
  - Premium "hero" cars that are cosmetic-forward, not overpowered.
- **Impulse buys at the moment of need:**
  - Instant repair.
  - Bail out of jail.
  - Lose your wanted stars.
  - Extend your garage lock while it's being raided.
  - Revive in a heist.
  - Double the payout on the results screen.
- **Season car pass.**
- **Crates** (if used) always show their odds and follow Roblox's paid random-item rules.
- **Rules:** prices match Robux pack sizes, offers are honest, and there are no fake timers.

---

## 20. Viral moments the game is designed to produce

- *"Someone stole my max-level Rainbow hypercar"* → a server-wide revenge chase.
- *"1-in-10,000 Glitch finish"* → the reveal.
- *"I bet my best car in a pink-slip race"*.
- *"My crew betrayed me after the bank heist"*.
- *"How long can I survive at 5 stars?"*
- *"Day 1 vs Day 30 garage"* → glow-up videos.
- *"I raided the richest player in the server"*.
- Ragdoll and fling fails, ramming chaos, and custom license plate jokes.
- Admin Abuse Hypercar Rain → mass server chaos.

---

## 21. Safety and fairness

- **Content:** non-graphic violence only (ragdoll, no realistic blood), which keeps the "Moderate" content rating (ages 9+). No real gangs, drugs or other mature themes. Crime is cartoon-heist energy.
- **Original IP:** no GTA or Rockstar names, logos, places or characters.
- **Anti-grief:**
  - Safe zones and newbie protection.
  - Lock timers.
  - Bounties on griefers.
  - Cops vs. high-heat players.
- **Anti-cheat:** everything that matters (money, damage, ownership, steals) is decided by the server.
- **Fair monetization:** odds disclosure, honest pricing, and no reward-for-watching gimmicks.

---

## 22. Launch vs. later (what ships first)

The game is deep, but a new player meets it **one layer at a time**, and the launch version should be the strongest slice, not everything at once.

| Version | What it includes |
|---|---|
| **Launch core** | Steal → drive home → park → earn; car rarities, finishes, upgrades and levels; garages with lock and raids; carjacking; wanted stars and AI police; chop-shop order board; armored truck every 5 min; basic guns; crews with a friend bonus; rare-spawn announcements; insurance and repo; daily rewards; offline earnings |
| **Fast follow (weeks 1–4)** | Street races and pink slips, bank heist, jail and jailbreak, player bounties, trading, car customization, more districts |
| **Later** | Player-cop faction, crew turf, businesses and empire, prestige, seasons, crossovers |

---

## 23. Why it should work

- It follows the patterns behind every recent Roblox mega-hit:
  - A title that is the rule ("Steal a Car").
  - A 30-second core loop.
  - A rarity collectible with stacked multipliers.
  - Stealing as social friction.
  - A number that always climbs.
  - A shared server clock.
  - Clip-ready moments.
- It wraps those patterns in the most recognizable game fantasy in the world, the week the real thing launches to an audience that mostly can't play it.
- It goes deeper than the typical steal game (police, crews, heists, races, an economy, player cops), so players have reasons to stay for the 28-day window the Roblox algorithm now rewards.
