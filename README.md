# Bomberman LBP2

Repository designed to showcase Bomberman LBP2, a personal project undertaken in my own free time where I took it upon myself to explore the design philosophy of the Bomberman series and to learn about the practices of independent game development. The game is finished and fully functional, yet several planned features have been forcibly omitted as the game engine suffers from serious memory constraint issues.

## Level Description

**Bomberman LBP2 (1-4 Players) by XZairX**

It's Bomberman in LBP! Lose yourself as you drop bombs to doom your friends in this faithful recreation of one of the greatest multiplayer experiences to ever grace the '90s! In addition to the classic Bomberman gameplay, this level features a HUD, life system, settings for game customisation, and special bomb upgrades! Please note that playing alone will force you into "Practice Mode" where you won't have an opponent to fight against. For the true Bomberman experience, play online with other people! Enjoy!

## Termination of Support (Update 1)

As of September 13th 2021, the online server for LittleBigPlanet 2, the game which provides the game engine necessary to run this project, has been [permanently shut down](https://twitter.com/LittleBigPlanet/status/1437415883752845318). As I can no longer provide updates to the project, it is important to note that it cannot and will no longer be maintained. This project should still be accessible via the PlayStation 4 version of the LittleBigPlanet 3 game which reportedly supports backwards-compatibility for creations uploaded from LittleBigPlanet 2. I will not be investing in this game to continue development for this project so I cannot speak for any changes in its functionality as a result of being accessed through a different system than what was intended. The following information in this repository will treat the project as if the online server for LittleBigPlanet 2 were still online.

<image src="images/littlebigplanet-service-update.png">

The destruction of these servers has also had the unfortunate side effect of terminating the [LBP.me website](https://littlebigplanet.fandom.com/wiki/LBP.me). This ultimately means that the level information and statistics relating to this project including data metrics such as number of plays, favourites, ratings, reviews, comments, and more, are no longer viewable online.

## Termination of Support (Update 2)

As of April 19th 2024, [all LittleBigPlanet servers have been closed indefinitely](https://twitter.com/LittleBigPlanet/status/1781427669801820406). This means that all information relating to this project is no longer accessible.

<image src="images/littlebigplanet3-service-update.png">

## Table of Contents

| Contents |
|:---------|
| [Getting Started](#getting-started) |
| &emsp; [Prerequisites](#prerequisites) |
| [Project Showcase](#project-showcase) |
| &emsp; [TITLE Menu](#title-menu) |
| &emsp; [CONTROLS Menu](#controls-menu) |
| &emsp; [INFORMATION Menu](#information-menu) |
| &emsp; [SETTINGS Menu](#settings-menu) |
| &emsp; [PLAY](#play) |
| &emsp; [Gameplay (Single-player)](#gameplay-single-player) |
| &emsp; [Gameplay (Multiplayer)](#gameplay-multiplayer) |
| &emsp; [Photo Session (Optional)](#photo-session-optional) |
| &emsp; [Ending](#ending) |
| [Remarks](#remarks) |
| &emsp; [Scrapped Update](#scrapped-update) |
| &emsp; &emsp; [Overhauled SETTINGS Menu](#overhauled-settings-menu) |
| &emsp; &emsp; [Pierce Bombs (removal of Remote Bombs)](#pierce-bombs-removal-of-remote-bombs) |
| &emsp; [Design Philosophy](#design-philosophy) |
| &emsp; [Limitations of the LittleBigPlanet 2 Game Engine](#limitations-of-the-littlebigplanet-2-game-engine) |
| &emsp; [Future Iterations](#future-iterations) |
| [Authors](#authors) |
| [References](#references) |

## Getting Started

A [Sony PlayStation 3 (PS3) video game console](https://en.wikipedia.org/wiki/PlayStation_3) and a copy of [Media Molecule's LittleBigPlanet 2 (LBP2) video game](https://en.wikipedia.org/wiki/LittleBigPlanet_2) are required to play the game. First-time LBP2 users will need to progress through the first world of the **Story** section to unlock the required **Community** section. From the **Community** section, select **Text Search** and either search for **Bomberman LBP2** (the level title) or **XZairX** (the PlayStation Network ID of myself, the level author). The former will return a large set results pertaining to user-generated Bomberman levels whereas the latter will only return the author's published levels. Simply navigate through the results until the Bomberman LBP2 level is located, select it, and the level encasing the game will start.

### Prerequisites

* Sony PlayStation 3 video game console
* LittleBigPlanet 2 video game

## Project Showcase

The following sections will detail the design and mechanisms of the numerous screens that the player can encounter when playing the game. These sections have been included to demonstrate the product to those who cannot meet the hardware prerequisites required to experience it first-hand. It also gives some insight into the ideology of some design decisions that were taken to improve the game after garnering player feedback. Any information relating to the design history of the product has been provided in block quotes to clearly separate it from the main description bodies of the project showcase.

### TITLE Menu

<image src="images/01-title-multi.png">

This menu is the first thing the player sees upon entering the game. In the LittleBigPlanet series of games, players have the ability to customise the appearance of their avatars. Within this menu are four sleeping default avatars who will wake and be replaced by the custom avatars of players whose profiles are loaded into the game. Active avatars are backlit by a predetermined colour which act as a unique identifier that is later used during the main gameplay section of the game.

The menu is also populated with a menu title header, a level title header, and the option to either jump to the `SETTINGS` menu or the `CONTROLS` menu by using the displayed button prompt. All menus are solely controlled by the player who takes the position of the left-most avatar, a position which is assigned to the first profile that loads into the game.

### CONTROLS Menu

<image src="images/02-controls.png">

This menu simply displays an interface which communicates the button mapping for the main gameplay section of the game. As the player moves through these menus, the positioning of the menu title header will shift either right or left to signify a forward or backward movement in menu progression.

>This menu previously featured additional button inputs that allowed for a more experimental style of play where the effects of special bombs could be chained together. After receiving user complaints for overcomplicating the control scheme of what is supposed to be a relatively simple game, these commands have since been compressed into a single input. This compressed command faithfully restricts the use of special bombs so that only one type can be used at any given time.

### INFORMATION Menu

<image src="images/03-information.png">

This menu holds the bulk of information used to inform the player of the various objects that they may encounter during the main gameplay section of the game. The `L1` and `R1` buttons are used to toggle left and right between the objects presented to view a brief description of their functionality.

>The object descriptions were initially very detailed averaging at around four lines each, yet they are now limited to only display a maximum of two. This reduction of clarity is a result of analysing player behaviours during the beta testing stages of the game. Players found that they would be helpless during gameplay, despite having read through these descriptions, as the information presented was far too profuse to be absorbed.

### SETTINGS Menu

<image src="images/04-settings.png">

This menu aims to increase replayability by providing a variety of customisation options which affect the initial state of the main gameplay section of the game. To maintain consistency with the control scheme of the other menus, `L1` and `R1` can be used to toggle left and right between the options of the settings. The `Left Stick Up` and `Left Stick Down` commands can also be used to toggle up and down between the different settings themselves. The button mapping for this functionality is not displayed as it is a natural instinct for users of the LBP2 community.

The leftmost column represents a setting's default value whereas the rightmost column is its maximum. All of these settings are self-explanatory save for `CAMERA` which increasingly reduces the number of visible objects during the main gameplay section to optimise the running performance of the game. The decision to use `MAX` over the real values of the maximum settings was done to favour consistency over the need to display a fixed arbitrary value.

### PLAY

<image src="images/05-play-multi.png">

A new `PLAY` button prompt will appear on the `TITLE` menu after all of the other menus have been visited. It is accompanied by some information which informs the players of a hidden quick-start feature that promotes replayability. The `PLAY` function transports the players away from the menu system and into the game arena where the main gameplay takes place.

>In the earlier stages of development, the player could freely select between all of the different menus from the first screen of the level and this included the `PLAY` function itself. Unfortunately, this liberty resulted in naive newcomers haphazardly jumping straight into the main gameplay of the game with little to no clue on how to actually play. This robbed them of their enjoyment and jeopardised their very crucial first impressions, effectively sabotaging their own experience.
 
>I aimed to redesign the menu system in a way that allowed for the game to be started as quick as possible for veterans and testing purposes, yet it also had to strike a balance that would encourage newcomers to explore the menus so that they were not left to be so clueless by the time they entered the game arena. This compromise has ultimately resulted in a less user-friendly system that benefits from a healthy increase in player satisfaction.

### Gameplay (Single-player)

<image src="images/06-gameplay-single.png">

This screen shows the initial game state of the game arena. To the left is the player HUD and to the right is the Power-UP Key. As the level has been designed with newcomers to the Bomberman formula in mind, these two components have been implemented to aid the player during gameplay. When playing alone, an information message exclusive to the single-player mode is activated to notify unwary players that the level has been designed to be enjoyed as a multiplayer experience.

### Gameplay (Multiplayer)

<image src="images/07-gameplay-multi.png">

Players have two minutes to complete their objective: to blow up the other players and survive to win as the last player standing. Players will drop bombs in an effort to remove the soft blocks that obstruct their paths between one another. In doing so, they will discover power-ups which they can pick up to strengthen their capabilities and their odds at survival. If two or more players are alive after the allotted two minutes have passed, the game is declared to be a draw and the alive players share the victory together.

### Photo Session (Optional)

<image src="images/08-photo-multi.png">

After the game ends by means of a win, loss, draw, or time out, all of the players are transported to this screen where they have a few seconds to modify their avatar's built-in expression and pose for a quick photo session. This section is completely irrelevant to the game and is catered to that of the LBP2 community itself. LBP2 allows for players to upload in-game photos to their profiles as a means of sharing their experiences. Uploaded photos do not provide information for where the picture was taken when viewed in-game, so the level title has been provided for a reference to help share the level. This section is optional and can be freely skipped by the winner(s) of the game without penalty.

### Ending

<image src="images/09-ending.png">

The final screen of the level. A "THANKS FOR PLAYING" text is briefly seen before collapsing to allow for the final scores of the players to be assessed on the scoreboard behind it. After this process finishes, the level ends and the game host has the option to either replay or exit the level. Unfortunate memory issues prevent the crucial implementation of having multiple rounds within a single session, and it has been left to the discretion of the host to replay the level should they wish to simulate this experience.

## Remarks

### Scrapped Update

Prior to the [termination of the LittleBigPlanet 2 online server](https://twitter.com/LittleBigPlanet/status/1437415883752845318) a final update was in development that aimed to provide meaningful quality of life updates to the project. These updates formed as a result of my strengthened experience and history with the Bomberman formula thanks to owning and extensively playing Super Bomberman R (2017) and Super Bomberman R Online (2020). Though I owned and extensively played Bomberman Ultra (2009) throughout the lifespan of this project's development, it made for a poor frame of reference as that game's mechanisms are riddled with problems that render their implementation to be inconsistent with the Bomberman series. Though I strongly believe that both Super Bomberman R and Super Bomberman R Online are far from providing a definitive Bomberman multiplayer experience, they at least implement their few gameplay mechanisms in a perfectly functional manner that is consistent with the Bomberman series. Thus, they serve as a strong frame of reference when mirroring the implementation of these same features into the project. This section will detail the major changes that this final update would have brought to the project had the servers not been terminated prior to its completion.

#### Overhauled SETTINGS Menu

The biggest and most important change comes from the completely overhauled `SETTINGS` menu. This overhauled menu was redesigned with the sole purpose to implement meaningful options that actively encouraged replayability. I felt that the current options were quite arbitrary and had a very minimal impact on replayability due its heavy focus on only altering the initial state of the game. Some of these new options also explore methods in which the state of the game can be brought closer to that of the source Bomberman material now that I have a stronger understanding of it. An image of the overhauled `SETTINGS` menu has been provided below alongside a full description of the effects that each selection would have had:

- Image of overhauled `SETTINGS` menu

**HUD:** Directly affects the player HUD located on the left-hand side of the arena to address gameplay performance and stability issues.
   - `OFF` _(default)_: Removes the player HUD to significantly reduce the number of on-screen objects and directly improve game performance and stability. It is also faithful to Bomberman's minimalistic multiplayer HUD.
   - `ON`: Retains the player HUD to allow for players to view and manage their bomb count, fire range, skate speed, heart count, and their type of special bomb (if applicable). This comes at the cost of impacting the game's performance and stability as more objects need to be displayed on-screen.

This update would have also completely removed the Power-Ups key located on the right-hand side of the arena. I felt that enough information on the Power-Ups had already been covered in the `INFORMATION` menu and the Power-Ups key has a detrimental effect on gameplay performance and stability due to the many additional objects that it demands to be displayed on-screen. I ultimately concluded that it was not worth compromising the gameplay's overall performance and stability to ensure that the more careless of players who skipped through the menus could correctly identify the many power-ups that they interact with.

**STAGE:** Changes the initial state of all player inventories and the game state based on the option selected.
  - `CLASSIC` _(default)_: All players start with 1 bomb, 2 fires, 0 skate, and a single heart in a standard arena. This mirrors the rules of a classic Bomberman multiplayer game.
  - `POWER`: All players start with 8 (maximum) bombs, 8 (maximum) fires, 2 (half of the maximum) skates, and a single heart in an arena without any soft-blocks. This mirrors the rules of the Power Zone maps featured in Bomberman games.
  - `SPEED`: All players start with 1 bomb, 2 fires, 4 (maximum) skates, and a single heart in a standard arena. This mirrors the rules of the Speed Zone maps featured in Bomberman games.
 
 **HEARTS:** Determines how many hits all players can initially take before being removed from play. Also enables/disables the heart system.
  - `OFF` _(default)_: All players start with 1 heart and cannot gain any additional hearts. This is the only option to disable the heart system and it is faithful to the classic Bomberman multiplayer experience.
  - `ONE`: All players start with 1 heart and can gain additional hearts if they interact with a Heart power-up.
  - `TWO`: All players start with 2 hearts and can regain hearts if they interact with a Heart power-up after taking a hit.

This update would have limited the maximum heart count to 2, down from 3, as having to damage a player at least three times before victory within a two-minute time limit is hardly reflective of a good Bomberman experience. Whilst not entirely faithful to the Bomberman multiplayer experience (though one could make an argument that they substitute the implementation of Louies - rideable creatures that grant players an extra hit point), the heart system has been retained to allow for beginners to experiment with the game without the issue of being immediately removed from play as a result of accidently blowing themselves up. Having two hearts also permits the implementation and use of the hidden Vest power-up which is simply a nice bonus feature to have.

**POPIT:** Toggles to the use of the directional pad (D-pad) for increased manoeuvrability options at the cost of disabling the Popit.
  - `OFF` _(default)_: Disables the Popit and enables the use of the D-pad in addition to the Left Stick for movement.
  - `ON`: Enables the Popit and disables the use of the D-pad, limiting movement to only the Left Stick.

The Popit is a LittleBigPlanet 2 feature that has many capabilities. For the purposes of this project, the most important tool that the Popit provides is the universal ability to communicate with other players through the use of text chat. Because of the way the button mapping in this engine is handled, the D-pad cannot be used in gameplay unless the Popit is disabled. This creates a problem where players need to weigh the importance of being able to communicate with each other with text chat versus being able to have a stronger sense of control over their characters with the support of D-pad movement. After careful consideration, I have decided that it is better to give the players a freedom of choice in the matter than to give them no option at all. Realistically speaking, no one plays Bomberman with stick, my movement system is far from perfect, and the level of movement and precision achievable with the D-pad is far superior to that of the Left Stick.

#### Pierce Bombs (removal of Remote Bombs)

This update would have also seen the removal of Remote Bombs. I initially added Remote Bombs to the game as I wanted to experiment with their viability in online play. Many Bomberman games feature the Remote Bombs in their single-player campaigns yet mysteriously omit them from their multiplayer experiences. I now understand that this is a deliberate balancing decision as the ability to leave behind bombs that only detonate on demand (if not hit by the fire of another bomb) is not only overwhelming for opposing players but it also takes away from the strategic positioning that is fundamental to the core Bomberman experience. Remote Bombs would have been replaced by the Pierce Bomb. This special bomb transforms the appearance of all of the player's bombs, modifies the colour of their fire (to signify the change in its fire properties), and has that fire travel through and destroy any collided soft blocks and power-ups. This special bomb is more commonplace in Bomberman games and is a far more balanced and acceptable alternative to the overpowered Remote Bomb.

### Design Philosophy

This project was created with the sole purpose to play Bomberman online with others. Despite this, it is interesting to note that I was not actually aware of the Bomberman brand prior to the conception of this project. The early prototype stages of this project's development were entirely based on Playing with Fire 2 (2006), a flash game that is essentially a lesser Super Bomberman 2 (1994) clone. It was not until 2016 that I eventually discovered the Bomberman franchise, bought Bomberman Ultra, and officially rebranded the project to its current Bomberman LBP2 iteration. Having said that, aspects of development stemming from its Playing with Fire 2 prototype build still remain. Some examples of these aspects include the presentation of the player HUD, the choice of colours that are assigned to each player, and the implementation of the heart system.

  - Image of Playing with Fire 2

Following the rebranding, an important question surfaced: now that I am aware of the Bomberman franchise, how do I define what makes a good Bomberman experience? Over the many decades that Bomberman has existed, many features have persisted yet they have also been prone to change due to the constant refinement that the series experiences. I explored this issue extensively in my [Bomberman Java project](https://github.com/ZairGitHub/Bomberman-Java) (whose development coincided with this project) and formed a design philosophy consisting of four factors when considering the implementation of a feature:
1. How does the feature impact gameplay balance? How does the variation affect the feature?
2. What is my own experience with the feature? How did it affect the gameplay when it was added? How would it affect the gameplay if it was removed?
3. How was this feature implemented in Super Bomberman 2 and Saturn Bomberman? These two games being widely considered by fans to the best Bomberman games of all time.
4. How was this feature implemented in Power Bomberman? A fan game that has taken feedback from the community throughout its continuous development to understand and implement what is arguably the best possible version of a feature.

  - Image of Power Bomberman

### Limitations of the LittleBigPlanet 2 Game Engine

- No code - all done with logic circuits and gates
- No concept of OOP (4 principles)
  - No polymorphism
  - No inheritance
- Memory constraints
- Age (2011 release for 2006 tech)

### Future Iterations

- Understanding and correcting movement
- Pressure blocks
- Rounds
- Designing MVP Bomberman (basic -> utility -> special bombs)
- Bomberman Unity (Shapes) and Unreal Engine

## Authors

* Riaz Philippe - BSc Computer Games Graduate

## References

* [Bomberman LBP2 Level Link](https://lbp.me/v/q3q01np)
* [PlayStation 3](https://en.wikipedia.org/wiki/PlayStation_3)
* [LittleBigPlanet 2](https://en.wikipedia.org/wiki/LittleBigPlanet_2)
