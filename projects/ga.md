# Project 2 - Group Assignment

## Final delivery

Please submit all the information in the following form:

[https://forms.office.com/e/eEunV5sM4x](https://forms.office.com/e/eEunV5sM4x)

It includes:
- Team name
- Game Title
- Video URL (around 3 min)
- Repository URL with updated Game Design Document at the root.

## Teams Registration

Please [register your team here](https://unlpt-my.sharepoint.com/:x:/g/personal/fpb_fct_unl_pt/IQAy1msBH4DaTKuH7QATbkXlAUF3o05Sxr45anFwQ0u5eao?e=FdKYn1) until Wednesday, April 15. [**CLOSED**]

**Note**: to help you reaching out to your mates I have setup a discord group with a forum to do just that: [https://discord.gg/CGFFHNkr](https://discord.gg/CGFFHNkr).

**Deliver your Concept and Proposal**: Add your document to your repository root.

## Objectives

- [Propose and develop a game](#Part-1:-Concept-and-Proposal). [due on April 26, 23h59.]
- Develop the concept of the game and develop it, in teams of 3.
- Submit your game and final documentation.
- Present your game before your peers.

## Description

You are required to program a video game with a team of 3 elements. There are no restrictions
on the type of game, style or genre, **as long as it is a 3D game**.

The game should present challenges that need to be solved in order to win. There should be a
compelling story, and the gameplay should be as interesting as possible. It should be composed
of a general menu with options, story presentation and at least two levels/modes (whatever
makes sense in your game). The game should respect the Game Elements Tetrad. You should
propose a set of mechanics, aesthetics, story narratives and technology for your game.

Teams are envouraged to create imaginative games with their own assets and original
gameplay. Games should be different from the ones programmed in the Individual Assignment.

The development of the game should be divided into 3 stages: Concept/Proposal, Development
and Final Presentation.

One of the group members should create a team in [Github Classroom](https://classroom.github.com/a/qdTWIc9K), and invite the remaining members to it.

**IMPORTANT**: Change the repository name to ga-P1-NN, where P1 is your lab slot, and NN is your group number, as registered here: [Team registation form](https://unlpt-my.sharepoint.com/:x:/g/personal/fpb_fct_unl_pt/IQAy1msBH4DaTKuH7QATbkXlAUF3o05Sxr45anFwQ0u5eao?e=FdKYn1).

**The number of commits and the respective owners of the repository will be monitored. Start using the repository from day 1!**

## Part 1: Concept and Proposal (max 3 pages).

In this first part of the project, each team should submit one pdf document (use letter size 11) containing the
Concept and the Proposal for the game. Be creative, use the space of the A4 sheet wisely!

### Concept document (max 1 page)

- Team identification (names, numbers)
- Title
- Premise
- Player Motivation (why the character in the game wants to fulfill the goals)
- Unique Selling Proposition
- Target Market / Target age
- Genre
- Expected HW requirements (include space)
- Competitive analysis (5 other games)
- Goals

### Game proposal (max 2 pages)

- Title, Hook, Goals.
- Story Synopsis, Backstory, Characters.
- Gameplay and main Mechanics.
- Technology/Libraries/Algorithms.
  - Main Components
- Art and Audio Features, Concept Art example.
- Production Details:
  - Team: list members
  - Roles: what each team member will do (should map to tasks in the next point)
  - Tasks: one paragraph describing each task
  - Gantt Chart with tasks.
- Risk Analysis, what will be the main (technical) challenges in the development.

You can add annexes with listings of characters, concept art, drawings, screenshots or schematics (not mandatory).

This is a tentative analysis, we accept some deviations in the final game. Grading for this document is included in the evaluation of its final and updated version in [Part 3](./ga.md#part-3-game-design-document-4-points).

You can [see here](../ga-samples) some samples from last year (randomly chosen).

**Failure to deliver a complete Concept and Proposal Document** will result in a **penalty of 4 points in the final group assignment score**

## Part 2: Game Development [14 points]

Code is delivered in the repository:
- Final commit by June 8 until 23h259
- Video and Build links as well as Final Game Design Document to be submitted around the same date.

The game should be a desktop game using Unity. Any deviation from this should have a strong justification and should be discussed with the professors. The group should have at least two follow-up conversations with the professors in the practical classes, with all the team members, as per the schedule published in [lab07](../labs/lab07.md).

The game will be evaluated according to the following criteria:

- [**6 Points**] **Storytelling + Game Mechanics + Aesthetics** (a fraction of this grade will depend on peer voting)
    - Storytelling: The story should make sense; the goals are clear and the game characters
support the narrative.
    - Game Mechanics: the game should have enough different things that the player can do.
The gameplay should be natural and the mechanics original.
        - Intuitive: Didn’t need to ask for help or completed the tutorial easily.
        - Original: I’ve never seen this.
        - Balance: Have a good balance between complexity and reward.
        - Diversity: Having a complete set of simple and complex tasks.
        - Responsiveness: The elements react and animate accordingly.
    - Aesthetics: The game has a finished and polished look. The interface supports the
game. Assets (Meshes, textures, audio) created by the team will be valorized. The game
looks support the gameplay and story. The gameplay is visually compelling and
enjoyable.

- [**0 points**] Mandatory Elements (1 point penalty for each feature not implemented)
    - Cheat mode to jump to interesting evaluation points using keys 1, 2, 3, 4 or M, N,
B, V etc.
    - ‘U’ key will toggle a free moving camera with mouse and WASD controls.
    - ‘P’ key will pause the game (stop every animation) but still allow you to freely
explore with the camera with ‘U’.
    Toggle frames per second using ‘I’ key

- [**8 points**] **Technology**: the game should make use of interesting algorithms and fully explore
the capabilities of the game engine.

  The following lists can be expanded with more ideas after an initial iteration with the
professors:



  - [**4 points**] Using plugins or of-the-shelf techniques (**1 point each**):
      - Dynamic lights and shadows (not baked)
      - Environmental/reflection maps.
      - Bump/Normal maps.
      - Effects with Unity particle systems
      - Shader graph to create special effects on vertices or surfaces
      - Levels of detail/LOD Group
      - Animator controllers
      - PBR Material
      - Multiple Raycasting
      - Cinemachine
      - Mixamo
      - CharacteNavMesh
      - NavMesh
      - complex colliders
      - etc.
  - [**4 Points**] Research and Implementation of Advanced Features. The game should make use of interesting algorithms and fully explore the capabilities of the game engine. You should research, explore and fully implement advanced techniques and algorithms without, or minimizing, the use of external plugins. The researched techniques should be discussed with the professor from the practical classes. Examples of custom made programmed techniques (**2 points each**):

      - Procedural content generation (terrain, vegetation,buildings, level) with a set of expressive and complex rules (cannot be a randomly generated terrain).
      - Procedural content generation: Wave Function Collapse, Perlin Noise, etc. You should be able to show diversity of the generated content.
      - Using A* algorithm.
      - Mesh creation and simulation from GIS data.
      - Multiplayer support: UNet, Photon or Mirror.
      - Procedural-Generation of audio (Change bit samples by procedurally manuplating them using rules).
      - Complex Physics simulation, preferably on the GPU using compute shaders.
      - AR or VR complex interaction.
      - Shader effects or Compute Shaders for Simulations such as Particle Systems, Fluids, Flow Simulations.
      - Implement Planar Reflections correctly.

**Important Note**:
Each group should program the game using the assigned GIT repository. There should be enough commits from each of the team members. The correct submission of everything is very important. Failing to comply with the submission rules or low participation in the team could result in an **individual penalty of up to 6 points**. Additionally, all students should follow the rules according to the Department’s Code of Ethics document.

## Part 3: Game Design Document [4 Points]

### Game Design Document

In the second stage the team should submit one pdf document (use letter size 11) containing the Game Design Document. 

The **Game Design Document** is the final document with a maximum of 6 pages plus annexes with an updated version of the Concept/Proposal Document.

Should contain:
- 1 page synopsis with updated version of concept document.
- 5 pages with summarized description of everything and connection to listings in annexes. 

This last part should contain:
- Updated version of the Proposal.
- Game Interface description.
- Technology elements you chose (see Technology section) with description of how you solved the problems, if required create schematics and additional details in annex.
- Self-Assessment table: What do you think should be your score in the Technology and Research sections?

**Annexes** with:
- list of external assets, external plugins or addons
- listings of concepts, screenshots, drawings, concept art, level design etc.

The documents should be self-sufficient with small examples. The annexes should only provide additional information.

**Video**: The final video should have 2 to 4 minutes and should present:
- Title, story, hook
- Assets created
- The game, main mechanics
- The technology, main techniques used.

## Part 4: Final Presentation [2 Points]

Each team will have to present the game in front of the class. Each team member should present an equal time slot. The presentation should include slides, gameplay videos, images,
and sounds. 

The presentation should focus on the game tetrad elements: story, mechanics, aesthetics and technology. It should describe all the necessary elements required for the evaluation of the topics listed in the previous section.