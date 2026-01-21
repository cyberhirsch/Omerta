# OMERTÀ: The City of Silence - Game Design Document

## 1. Overview
**OMERTÀ** is a digital board game that blends classic property management mechanics with a 1920s Prohibition-era mafia theme. Players take on the role of Mob Bosses vying for control over "The City of Silence," using intimidation, bribery, and strategic expansion to bankrupt their rivals and become the *Capo di tutti i capi*.

## 2. Core Gameplay Mechanics
### 2.1 The Board
The game follows a circular board structure consisting of 40 unique spaces:
- **Turf (Properties)**: Standard territories that can be acquired and improved.
- **Transportation Routes**: Strategic routes (Trucking, Harbor, Airport, Train) that increase in value the more you own.
- **Rackets (Utilities)**: Essential services (Waste Management, Power Grid) with variable tribute costs.
- **The Don's Mansion (GO)**: The starting point where Bosses collect their "cut" ($200).
- **The Cooler (Jail)**: A place where Bosses are "pinched" and must either pay a bribe or roll doubles to escape.
- **Hit List & Favors (Cards)**: Random events that can grant windfalls or sudden setbacks.
- **Laundering & Bribes (Tax)**: Flat fees that drain a Boss's cash reserves.

### 2.2 Turn Structure
Omerta uses **Hidden Mechanics** to streamline play and focus on the narrative:
1. **Automated Roll**: At the start of a turn, the dice are rolled hidden in the background.
2. **Immediate Action**: The Boss's crew moves to the new location instantly.
3. **Narrative Presentation**: The player is presented with a story-driven description of their arrival and their available options (Buy, Expand, or End Turn).

### 2.3 Expansion System (Improvements)
Instead of traditional buildings, Bosses "tighten their grip" on acquired Turf:
- **Muscle (Levels 1-4)**: Stationing soldiers at a location to increase the tribute (rent) collected from rivals.
- **Racket Hubs (Level 5)**: Establishing a permanent headquarters that maximizes income.
- **Full Neighborhood Bonus**: Improvements can only be made once a Boss controls all Turf in a specific color group. Unimproved full sets collect double the base tribute.

## 3. Thematic Elements & Narrative
### 3.1 Terminology
- **Rent** -> Tribute
- **Houses/Hotels** -> Muscle / Racket Hubs
- **Jail** -> The Cooler
- **Tax** -> Laundering Fee / Bribe The Mayor

### 3.2 Storytelling
Every move is narrated as a crew activity (e.g., "Your crew arrives at the Dive Bar"). This shifts the focus from "playing a board game" to "managing a criminal empire."

## 4. Visual & Audio Style
### 4.1 Aesthetic
- **Retro 8-Bit**: High-contrast pixel art style using neon red and yellow on deep black backgrounds.
- **Pixel Typography**: Use of "Press Start 2P" Google Font for all UI elements.
- **CRT Effect**: Subtle scanline overlays and color bleed to simulate a vintage computer terminal.

### 4.2 UI Layout
- **Top Bar**: Persistent display of active Boss, Cash, and status.
- **Center Stage**: Large narrative block with high-impact text and context-sensitive action buttons.
- **Competition Grid**: A summary of all rivals, their cash, and their current influence.
- **History Log**: A fading list of past events for reference.

## 5. Technical Stack
- **Languages**: HTML5, CSS3 (Vanilla), JavaScript (ES6+).
- **Architecture**: State-driven UI updates with a centralized `state` object.
- **Persistence**: LocalStorage for saving and loading game progress.

## 6. Development Roadmap
- [x] Core Board Logic
- [x] Hidden Rolling / Automated Movement
- [x] Story-driven UI Refactor
- [x] Retro Style & Pixel Fonts
- [x] Muscle/Expansion System
- [ ] AI Rivals for single-player mode
- [ ] Sound Effects & 8-bit Noir BGM
- [ ] Visual scene graphics for every unique location
- [ ] Trading system between Bosses
