# Lunch Fury

![lunch-fury](Media/lunch-fury.gif)

A third person action game developed in **Unreal Engine 5.5.4** that focuses on gameplay programming, AI behaviour, animation driven combat, and event driven progression systems.

The project was developed as a solo game jam project with the goal of exploring responsive melee combat, scalable enemy AI, and modular gameplay systems built entirely using Blueprint Visual Scripting.

---

## Project Overview

Lunch Fury is a fast paced action game where players fight through increasingly challenging waves of enemies using melee combat.

Enemies become progressively more aggressive based on the selected difficulty while maintaining predictable behaviour through Behaviour Trees and navigation systems.

The project combines combat mechanics, enemy AI, cinematic sequencing, and gameplay progression into a complete arcade style experience.

---

## Technical Summary

| Category | Details |
|----------|---------|
| Engine | Unreal Engine 5.5.4 |
| Programming | Blueprint Visual Scripting |
| Project Type | Third Person Action |
| AI | Behaviour Trees, EQS |
| Input | Enhanced Input |
| Architecture | Modular Blueprint System |
| Team Role | Solo Developer |

---

# Gameplay Systems

## Enemy AI

Enemy behaviour is implemented using Unreal Engine's Behaviour Tree framework together with the Environment Query System (EQS).

The AI system supports:

* Multiple difficulty levels
* Intelligent player tracking
* Navigation and pathfinding
* Combat engagement
* Progressive wave difficulty

Rather than simply increasing enemy health, each difficulty level adjusts the intensity of encounters to create a more engaging gameplay experience.

---

## Combat System

The combat system was the primary technical focus of this project.

Instead of relying on random hit reactions, attacks are animation driven.

Each attack performed by the player triggers a matching reaction animation on the enemy based on the specific attack that connects.

For example:

* A punch to the head produces a head hit reaction.
* A kick to the torso produces a torso hit reaction.

This creates more believable combat while improving player feedback and visual consistency.

Implementing this system required coordinating animation logic across multiple characters while maintaining responsive gameplay.

---

## Health System

The gameplay includes a modular health system supporting:

* Damage
* Healing
* Death handling
* Combat feedback

Health changes are integrated directly into the combat flow and enemy behaviour.

---

## Event Driven Progression

Gameplay progression is driven through gameplay events rather than scripted sequences.

The progression system manages:

* Enemy wave progression
* Difficulty scaling
* Match completion
* Ending cinematic sequence

Separating progression from individual gameplay actors keeps the overall game flow organised and easier to maintain.

---

# Artificial Intelligence

Enemy behaviour combines several Unreal Engine systems to create responsive opponents.

Features include:

* Behaviour Trees
* Environment Query System (EQS)
* Navigation
* Player detection
* Combat engagement
* Difficulty scaling

Each AI character responds dynamically to the player's position while maintaining predictable gameplay behaviour.

---

# Animation System

One of the project's primary objectives was improving communication between attacking and defending characters.

Instead of allowing enemies to randomly react to incoming attacks, the combat system maps specific player attacks to corresponding enemy reaction animations.

This creates stronger visual feedback and results in combat that feels more intentional and responsive.

---

# User Interface

The interface is implemented using Unreal Motion Graphics (UMG).

The UI manages:

* Health display
* Gameplay feedback
* Difficulty selection
* Game flow
* Player information

The interface was designed to remain simple while supporting the overall gameplay experience.

---

# Blueprint Architecture

The project follows a modular Blueprint architecture where each gameplay system is responsible for a clearly defined task.

Core systems include:

* Enemy AI
* Combat
* Health management
* Player controls
* Difficulty management
* Gameplay progression
* User Interface
* Cinematic sequencing

This separation allows gameplay systems to evolve independently while keeping the project organised.

---

# Unreal Engine Features Used

* Blueprint Visual Scripting
* Behaviour Trees
* Environment Query System (EQS)
* Enhanced Input
* Animation Blueprints
* Blueprint Interfaces
* Navigation System
* Physics
* Collision
* Niagara
* Trigger Events
* Widget Blueprints
* Unreal Motion Graphics (UMG)

---

# Technical Challenges

## Animation Driven Combat

The most technically challenging aspect of the project was designing a combat system where player attacks directly determine enemy reaction animations.

Rather than selecting reactions randomly, each attack communicates the appropriate response to the defending character.

This creates combat that feels more responsive while improving the readability of every successful hit.

Implementing this system strengthened my understanding of animation programming, gameplay communication, and Blueprint architecture.

---

## AI Behaviour

Designing enemy behaviour that remains challenging while scaling naturally across multiple difficulty levels required balancing navigation, combat behaviour, and encounter pacing.

Behaviour Trees and EQS provided a flexible foundation that can be expanded with additional enemy behaviours in future iterations.

---

# Future Improvements

If I were to continue developing Lunch Fury, I would expand the game into a larger action experience.

Planned improvements include:

* Boss encounters
* Multiple playable levels
* Expanded narrative progression
* Additional enemy archetypes
* More advanced combat abilities
* Combo system
* Additional cinematic sequences

The existing gameplay architecture was intentionally designed to support these additions without requiring significant changes to the underlying systems.

---

# Repository Structure

```
Config/
Content/
Source/
LunchFury.uproject
README.md
```

Generated Unreal Engine folders such as `Binaries`, `Intermediate`, `Saved`, and `DerivedDataCache` are intentionally excluded from source control.

---

# Skills Demonstrated

* Gameplay Programming
* AI Programming
* Behaviour Trees
* Environment Query System
* Animation Programming
* Combat System Design
* Blueprint Architecture
* Event Driven Programming
* User Interface Programming
* Unreal Engine Development

---

# Author

**Temitope S. Falade**

Gameplay Programmer | Technical Animator | Technical Artist

Portfolio  
https://topson-noble.github.io/

Game Portfolio  
https://topzone.itch.io/

LinkedIn  
https://www.linkedin.com/in/temitope-falade-578107120/
