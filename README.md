
# Explorartive Software Development: Game Development

[todo: detailed course information, like course code, etcs, course owner, teachers, date, etc]
## Introduction

Games are among the most complex forms of software out there. They bring together all facets of software development, from UX and design to algorythms and optimisation. The game development track will aim to touch on all these topics, while focussing on the technology behind games. In doing so students will be given the opportunity to work on each of the core competencies for software developers. 

The focus of the game development track is the development of real-time interactive software. The track is roughly divided into two parts. During the first few weeks students will work on developing the core technical skills necessary to develop real-time software through classes and assignments. In the second half students will be given the freedom to develop a game of their own, allowing them to apply and hone the skills they have learned so far. Furthermore they will be challanged to learn new skills as they inevitably run into problems during the development cycle.

## Reletionship with other courses

A good base in Object Oriented software development will be required, particularly in C#.


## Learning Objectives
The following learning objectives are aligned with Bloom's Taxonomy and focus on developing competencies in Professional Skills, Analysis, Design, Implementation, Research (Exploration), and Advice:

At the end of this course students will be able to:

1. *Demonstrate* effective planning, communication (written and verbal) and collaboration skills by working individually and in teams to produce professional-quality game development artifacts, including project documentation and presentations.
	
	*(Competency: Professional Skills)*  
   	*(Bloom’s Taxonomy Level: Apply)*
   [todo: add manage and control, setting up guthub, azure, etc]

2. *Analyze* requirements and user needs to identify core functionalities, constraints, and technical challenges by creating an SRS report (covering both functional and non-functional requirements). 
  	
  	*(Competency: Analysis)*   
   	*(Bloom’s Taxonomy Level: Analyze)*

3. *Create* a detailed Game Design Document (GDD) that covers design principles, structural and behavioural models ensuring alignment with project requirements.  
   
   *(Competency: Design)*   
   *(Bloom’s Taxonomy Level: Create)*

4. *Develop* functional game prototypes by applying programming to realize game functionalities and by applying systematic testing.
	
	*(Competency: Realization)*   
   	*(Bloom’s Taxonomy Level: Apply)*

5.   *Evaluate* technologies, libraries, frameworks, tools in game development to determine their potential impact on the design and development process.  
   	
   	*(Competency: Research)*   
   	*(Bloom’s Taxonomy Level: Evaluate)*
[todo: maybe later we integrate this with advice?]

6. *Propose* recommendations for optimizing game features and quality like performance, user experience, maintainability or reusability of the code justified by data and best practices. 
  	
  	*(Competency: Advice)*   
   	*(Bloom’s Taxonomy Level: Evaluate)*

---

## Weekly Program Schema

[todo: to be completed]

### Week 1: Introduction to Game Development
- **Workshop 1 Topics:** Introduction to games (why games, what types of games are there), Project 1
- **Activities:** Installing Monogame, setting up Git 
- **Workshop 2 Topics:** Monogame Game development fundamentals 
- **Activities:** Game loop, drawing text and sprites, simple movement

### Week 2: Basics of interaction and movement
- **Workshop 1 Topics:** Handling input in Monogame
- **Activities:** Reading out Input, Handling key down events, checking if a player clicks on something, check if a point is in a rectangle
- **Workshop 2 Topics:** more movement
- **Activities:** Simple physics, normals, Collision between circles and arbitrary lines, reflections, random point on a circle

### Week 3: Handling multiple objects and making the game pretty
- **Workshop 1 Topics:** GameObjects, working with lists and grids, Project 2
- **Activities:** 
- **Workshop 2 Topics:** Using sprite sheets and sound effects
- **Activities:** 

### Week 4: 
- **Workshop Topics:** Scrolling levels
- **Activities:** Multiple sprite batches, matrix transformations 101
- **Workshop 2 Topics:** Game States
- **Activities:** Game manager, singletons, pauzing, menus and levels 

### Week 5: 
- **Workshop 1 Topics:** Encapsulation vs Inherritance
- **Activities:** (abstract) factory pattern, building objecs from files
- **Workshop 2 Topics:** Saving and loading
- **Activities:** Serializing/deserializing objects, what (not to) save

### Week 6: Design Documents
- **Workshop 1 Topics:** Start of Project 3, Making a design document
- **Activities:** Creating a Game Design Document (GDD), initial prototype.
- **Workshop 2 Topics:** Modifiers
- **Activities:** Decorator pattern

### Week 7: 
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 8: UML diagrams
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:**

### Week 9: 
- **Workshop 1 Topics:** 
- **Activities:** 

### Week 10: 
- **Workshop 1 Topics:** 
- **Activities:** 

### Week 11: 
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 12: 
- **Workshop 1 Topics:**
- **Activities:**  
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 13: Pathfinding
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 14: Introducion to user testing
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 15: Advanced object collision
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:** 9

### Week 16: 
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 17: Optimization and profiling
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 18: 
- **Workshop 1 Topics:** GPU
- **Activities:** Introduction to the GPU, how to program shaders
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 19: 
- **Workshop 1 Topics:** 
- **Activities:** 
- **Workshop 2 Topics:** 
- **Activities:** 

### Week 20: Final Project Presentation
- **Workshop Topics:** Presentation and critique of final projects.
- **Activities:** Showcasing the completed game, peer and instructor feedback.


## Project Description

### Project 1 Pong (week 1/2)
Focus on: first practice with system, how to draw objects, how does movement work, simple collision, does it work functionally.
Create a basic implementation of 4 player Pong using just the framework. 
Requirements:
- There are 4 paddles that can be either player controlled or “AI” controlled.
- There is a ball that bounces back and forth whenever it hits a paddle. Depending on where the ball hits the paddle the angle at which it bounces should change.
- Whenever the ball bounces it should speed up and a sound effect should play.
- When the ball misses a paddle that player should lose 1 life.
- The “AI”  should simply try to follow the ball.

### Project 2 Platformer (week  3-5)
Focus on: Modify an existing project, learn about working with larger (arbitrary) numbers of objects, some design patterns, grids, level loading, simple animations, moving viewports v.s. static HUD, etc.
Students will be given a simplified version of the Monogame Platform2D sample and asked to make several extensions: https://github.com/MonoGame/MonoGame.Samples/tree/3.8.0/Platformer2D
- Students should: Add a trap that shoots arrows
- Make the camera follow the player to extend the level, while the HUD remains on screen
- Add functionality to load a new level upon level completion
- Give the player lives and make them invincible for a short time upon taking damage
- ?
  
### Project 3 Free project (Week 7-19)
Focus on: more freedom in design, work creating a bigger project with a group. The game should be a top down game in which both the player and NPC characters can move around 
- Students should write a short design document (week 7)
- Students should create an UML diagram to design a basic layout for their game code 
- Use inheritance and encapsulation to create multiple variants of objects
- Level editor
- Loading/saving
- Inventory and/or effects
- Students should create a questionnaire, playtest their game with other people and report on their findings
- Students should improve their game based on the feedback
- A*, AABB tree, Shaders

### Other subjects
- I want students to gain experience with:
- The basics of A* pathfinding (can be applied in P3)
- Object collision using AABB trees (can be applied in P3)
- Fundamentals of shaders (focus on fragment shaders) (can be applied in P3)
- Optimization, when and how to use a profiler


## Assessment

[todo: later.]
