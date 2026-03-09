# Game Design Document

## High level concept

### Working title

Rising Dough: Beat by Beat

### Concept statement

Rising Dough: Beat by Beat is a 2D horror platformer inspired by the Kolobok folktale. You are a living dough creature navigating a fungal-corrupted world through traditional platforming, with boss fights that shift into rhythm-based singing duels where every path ends in death.

### Genre(s)

Rhythm-based horror 2D platformer

### Target audience

- Players who enjoy atmospheric indie platformers and dark fairytale fiction
- Fans of rhythm-action boss fights and mechanically expressive timing systems
- Players interested in folklore reinterpretations

### Unique selling points

- Singing duels as boss encounters: shift from platforming to rhythm-based call-and-response battles drawn from the original folktale
- Folktale horror twist: Kolobok retold through fungal/yeast corruption
- Tragic loop structure: success and failure both end in perishing, with looped replay as narrative
- Optional third path: a hidden ending based on self-determined refusal of fate

## Product design

### Player experience and game POV

The player controls Kolobok from a side-view 2D perspective in a tense, forward journey. The fantasy is being a fragile lifeform fighting for autonomy through movement and voice. Target emotions are curiosity, dread, urgency, and tragic acceptance. Engagement comes from tight platforming execution during exploration and intense rhythm focus during boss singing duels, with narrative clues revealed across loops.

### Visual and audio style

Visual direction is high-contrast monochrome black silhouettes, layered parallax fog, sparse highlights, and oppressive negative space. Characters are represented as silhouettes, fungal growth is shown through shape distortion and subtle texture rather than color.

Audio design centers on ambient heartbeat percussion, breath, and damp organic textures during platforming. Boss encounters introduce vocal melodies and folk motifs that mutate across phases, with clear rhythm cues for singing duels.

### Game world fiction

Kolobok is brought to life by tainted yeast (fungal starter) used in a household baking ritual. It flees home and encounters familiar folktale animals (rabbit, wolf, bear, fox), each transformed by the same infection at different stages.

Theme: sentience does not guarantee freedom. Whether Kolobok is consumed by corruption or reaches home, it still perishes.


### Platforms, technology and scope

- Platforms: WebGL for easy access and sharing
- Technology: Unity 2D
- Team/scope: 4 main chapters + looped ending system
- Timeline target: first playable vertical slice in 2 sessions, content-complete by end of semester
- Major risks: rhythm graph design, fair difficulty curve, animation and audio workload

## Detailed & Game systems design

### Core loops

1. Explore and platform through corrupted environments using traditional 2D movement.
2. Navigate environmental hazards and discover narrative clues.
3. Encounter corrupted animal drawn by your presence, triggering boss "Singing Duel."
4. Engage in rhythm-based call-and-response battle: boss sings corrupted phrases, you respond to dodge and counter-attack.
5. Resolve encounter, advance corruption state, unlock next chapter or trigger loop reset.
6. Reach one of three ending states; restart cycle with new narrative context.

### Objectives and progression

Short-term objective: survive each stage and defeat the chapter boss.
Long-term objective: complete all chapters, understand the cycle, and unlock the hidden third path.

Progression is chapter-based with rising tempo complexity, denser pattern language, and tougher traversal pressure. Repeated loops reward mastery plus story discovery:
- Loop 1: establish world and fate
- Loop 2: expose deeper environmental clues and corruption origin hints
- Secret criteria: unlock third path

### Game systems

- Platforming movement system: run, jump, roll/dash with physics-based interactions
- Health/corruption meter: tracks damage and corruption state progression
- Rhythm input system (boss-only): beat windows, accuracy ratings, singing response validation
- Boss singing duel system: call-and-response phrases, phase-based attack patterns, vocal counter-mechanics
- Ending logic system: branches into fail ending, "home and eaten" ending, or hidden third ending

### Interactivity

**Platforming sections:** Standard 2D action controls (run, jump, dash/roll) with environmental hazards (collapsing platforms, spore vents, darkness). Focus on spatial navigation, timing jumps, and exploration. Environmental storytelling and visual cues provide lore.

**Boss singing duels:** Shift to rhythm-based input. Boss sings corrupted musical phrase (visual/audio cues), player must respond with correct timing and pattern to dodge or counter-attack. Success = damage boss and maintain health. Failure = take damage and increase corruption. Emotional interactivity driven by tension between quiet exploration and intense musical confrontation.

## Milestones

### Milestone 1

Prototype foundation:
- Playable movement (run, jump, dash) and camera in one test level
- Basic rhythm input system for boss prototype
- Health/corruption meter with fail state
- Initial art/audio style test for one environment and one boss theme

### Milestone 2

Vertical slice:
- One full chapter from intro to first boss (rabbit)
- Boss phase system with 2-3 rhythm patterns
- Corruption progression pass
- Narrative delivery pass for opening

### Milestone 3

Production and polish:
- All main chapters implemented
- Full ending flow with loop reset and hidden third path conditions
- Final audio mix, balancing, UI readability, and bug fixing
- Playtesting pass focused on rhythm clarity, difficulty curve, and narrative impact

## References

- [Kolobok](https://en.wikipedia.org/wiki/Kolobok)
- [The Pancake](https://sites.pitt.edu/~dash/type2025.html#norway)
- [The Runaway Pancake](https://ingebretsens-blog.com/scandinavian-folklore-3/)
- [Everhood](https://store.steampowered.com/app/1229380/Everhood/)
- [A musical story](https://store.steampowered.com/app/1546100/A_Musical_Story/)
- [PaRappa the Rapper](https://en.wikipedia.org/wiki/PaRappa_the_Rapper)
- [Limbo](https://playdead.com/games/limbo/)
