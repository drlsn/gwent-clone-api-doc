# Introduction

&nbsp;&nbsp;&nbsp;&nbsp; I have been thinking of an idea for some time now - to create a small web game solely for educational purposes. However, game design can be a challenging task, and at the moment my priorities lie more on a technical side of things, so I decided to create a clone of an existing game, maybe just a little bit modified to make things more interesting. I have chosen The Witcher 3 Gwent minigame to experiment upon, since I know the rules more or less and it is quite popular, so are there information about it on the internet easy to search for.
	
&nbsp;&nbsp;&nbsp;&nbsp; My main focus will be on the backend or API initially, with frontend development being probably a separate project. For educational purposes, I plan to create a bit overengineered version of the game and the knowledge gathered will serve me as a foundation for future projects.
	
&nbsp;&nbsp;&nbsp;&nbsp; I want to put much emphasis on quality attributes, so I am going to actively develop a well organized technical specification document. Besides it I am also writing this article in a form of blog post, so I can present my thought process in a natural language.

## Initial Design

&nbsp;&nbsp;&nbsp;&nbsp; First I will focus on generally describing what's in my mind in this section. I'll be more or less basing on [arc42](https://arc42.org/overview), which gives some tips on how to document a software, as well as [ISO Standard 25010](https://iso25000.com/index.php/en/iso-25000-standards/iso-25010) for quality attributes.

### Naming

&nbsp;&nbsp;&nbsp;&nbsp; The Gwent allows for using one of the few decks of cards used at a single game. There are at least 5 of them:
- Northern Kingdoms
- Nilfgaard Empire
- Scoia'tael
- Monsters
- Skellige

Since I want to change things just a little bit, I am going to change a game theme and rename decks and cards. I want it to take place in a postapo / scifi / nature environment, so the decks will named as following, with very brief description, there is no need for much storytelling really:
- Settlers - rather casual people, hard working, create new towns, try to create a normal civilization in this dangerous world
- Technocrats - possess advanced technological knowledge, but without it are defenceless, not many of them left
- Ancestrals - lived here since always in the jungles, know how to survive in such extreme conditions
- Dinosaurs - dangerous monsters
- Nomads - live in small camps, moving all the time, hiding and plundering when an occasion appears

As for names and graphics, I'm not yet sure, but I'm going to be pretty loose about it.

There is a TV series done by Steven Spielberg called "Terranova" It was about a group of people moving back in time to Mesozoic era and trying to make a living there.
Although the show didn't gain much popularity, I enjoyed it enough to use its name as title for this project.

### Feasibility Reasearch

#### Scope and Team
&nbsp;&nbsp;&nbsp;&nbsp; The game is not as big and there a lot of information in the web. The main challenge is infrastructure and presentation though.

#### Market
&nbsp;&nbsp;&nbsp;&nbsp; Due to the popularity of the game, there is no doubt there are examples of clone implementation or similar card games, but the reason is mainly for educational purposes, so doesn't matter. And.. it is gonna be a different setting / theme, to allow just for a little bit of creativity and making it different.

#### Alternative solutions
- Making another game - a game with more complex problems to solve would be interesting, not just a tic-tac-toe, but my goal is to focus on quality and technology, so better to have some smaller domain to build upon
- Making a business app - but my goal is to make a game, though probably a typical app and focusing on solving a realistic problem, could have more value, maybe for other people, maybe for, for a portfolio in more typical business industries other than gamedev.

#### Technical Feasibility
&nbsp;&nbsp;&nbsp;&nbsp; Done some backend already, but now the focus is more on quality, at least on backend side of it.

#### Other technical options
- Unity3D with a networking plugin, ex. Photon
- .NET monolith with no event architecture and Blazor Server - no need for api, would work

#### Proposed Solution
- .NET microservices, React, HTML, CSS
- Message Bus, Event driven Architecture, Vertical Slices, both REST or RPC api, NGinX, Docker / Docker Swarm,
- testing - unit, integration, E2E, performance

#### Initial Features

&nbsp;&nbsp;&nbsp;&nbsp; A project technically has to have defined a start and end, so I need to be pretty specific about I which features and qualities exactly I want to include. After getting familiar with the rules, reading the game wiki or watching some gameplays and seeing the UI I've across with of the initial ideas. These are going to be revised later in the design stage.
Also, I am going to add a "Statistics" feature, so the players can view each other progress, well.. of course I don't really foresee anyone there, but instead I might actually create some bots for testing purposes in the future, but this is going to be as a scope of another project to minimize effort, first things first.

##### Core Gameplay

| Actions 	| Views 	| 
| -------------	| -------------	| 
| Play Card  	| Card Board	|
| Pass Round    |  		|

##### Supporting
| Actions 	| Views 	| 
| -------------	| -------------	| 
| Join Game  	| Main Menu	|
| Quit Game   	|  		|

##### Statistics
| Views 	| 
| -------------	| 
| Statistics	|

##### Out of Scope

&nbsp;&nbsp;&nbsp;&nbsp; xxxx

#### Initial Qualities

#### Deliverables

&nbsp;&nbsp;&nbsp;&nbsp; backend, docs, hosted

#### Team

&nbsp;&nbsp;&nbsp;&nbsp; Alone now, later maybe when ready

