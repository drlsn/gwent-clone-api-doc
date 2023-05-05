# Introduction

&nbsp;&nbsp;&nbsp;&nbsp;I have been thinking of an idea for some time now - to create a small web game solely for educational purposes. However, game design can be a challenging task, and at the moment my priorities lie more on a technical side of things, so I decided to create a clone of an existing game, maybe just a little bit modified to make things more interesting. I have chosen The Witcher 3 Gwent minigame to experiment upon, since I know the rules more or less and it is quite popular, so are there information about it on the internet easy to search for.
	
&nbsp;&nbsp;&nbsp;&nbsp;My main focus will be on the backend or API initially, with frontend development being probably a separate project.	For educational purposes, I plan to create an overengineered version of the game and the knowledge gathered will serve me as a foundation for future projects.
	
&nbsp;&nbsp;&nbsp;&nbsp;I want to put much emphasis on quality attributes, so I am going to actively develop a well organized technical specification document. Besides it I am also writing this article in a form of blog post, so I can present my thought process in a natural language.

## Initial Design

&nbsp;&nbsp;&nbsp;&nbsp;First I will focus on generally describing what's in my mind in this section. I'll be more or less basing on [arc42](https://arc42.org/overview), which gives some tips on how to document a software, as well as [ISO Standard 25010](https://iso25000.com/index.php/en/iso-25000-standards/iso-25010) for quality attributes.

### Naming

&nbsp;&nbsp;&nbsp;&nbsp;The Gwent allows for using one of the few decks of cards used at a single game. There are at least 5 of them:
- Northern Kingdoms
- Nilfgaard Empire
- Scoia'tael
- Monsters
- Skellige

Since I want to change things just a little bit, I am going to change a game theme and rename decks and cards. I want it to take place in a postapo / scifi / nature environment, so the decks will named as following:
- Settlers - create new towns, 
- Technocrats - possess advanced technological knowledge, but without it are defenceless
- Ancestrals - lived here since always in jungles, know how to survive in such extreme conditions
- Dinosaurs - dangerous monsters living in the jungle
- Nomads - live in small camps, moving all the time, hiding and plundering when an occasion appears

As for names and graphics, I'm not yet sure, but I'm going to be pretty loose about it.

There is a TV series done by Steven Spielberg called "Terranova" It was about a group of people moving back in time to Mesozoic era and trying to make a living there.
Although the show didn't gain much popularity, I enjoyed it enough to use its name as title for this project.
