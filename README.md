# Bomberman LBP2

Repository designed to showcase Bomberman LBP2, a personal project undertaken in my own free time where I took it upon myself to explore the design philosophy of the Bomberman series and to learn about the practices of independent game development. The game is finished and fully functional, yet several planned features have been forcibly omitted as the game engine suffers from serious memory constraint issues.

## Level Description

**Bomberman LBP2 (1-4 Players) by XZairX**

It's Bomberman in LBP! Lose yourself as you drop bombs to doom your friends in this faithful recreation of one of the greatest multiplayer experiences to ever grace the '90s! In addition to the classic Bomberman gameplay, this level features a HUD, life system, settings for game cusomtisation, and special bomb upgrades! Please note that playing alone will force you into "Practice Mode" where you won't have an opponent to fight against. For the true Bomberman experience, play online with other people! Enjoy!


| Table of Contents |
|-------------------|
| [Termination of Support](#termination-of-support) |
| [Getting Started](#getting-started) |
| &emsp; [Prerequisites](#prerequisites) |
| [Project Showcase](#project-showcase) |
| &emsp; [Video Demonstration](#video-demonstration) |
| &emsp; [TITLE Menu](#title-menu) |
| &emsp; [CONTROLS Menu](#controls-menu) |
| &emsp; [INFORMATION Menu](#information-menu) |
| &emsp; [SETTINGS Menu](#settings-menu) |
| &emsp; [PLAY](#play) |
| &emsp; [Gameplay (Single-player)](#gameplay-single-player) |
| &emsp; [Gameplay (Multiplayer)](#gameplay-multiplayer) |
| &emsp; [Photo Session (Optional)](#photo-session-optional) |
| &emsp; [Ending](#ending) |
| [Authors](#authors) |
| [References](#references) |

## Termination of Support

As of September 13th 2021, the online server for LittleBigPlanet 2, the game which provides the game engine necessary to run this project, has been [permanently shut down](https://twitter.com/LittleBigPlanet/status/1437415883752845318). As I can no longer provide updates to the project, it is important to note that it cannot and will no longer be maintained. This project should still be accessible via its PlayStation 4 successor LittleBigPlanet 3 which reportedly supports backwards-compatibility for creations uploaded from LittleBigPlanet 2. I will not be investing in this game to continue development for this project so I cannot speak for any changes in its functionality as a result of being accessed through a different system than what was intended. The following information in this repository will treat the project as if the online server for LittleBigPlanet 2 were still online.

- Twitter server shutdown image

The destruction of these servers has also had the unfortunate side effect of terminating the [LBP.me website](https://littlebigplanet.fandom.com/wiki/LBP.me). This ultimately means that the level information and statistics relating to this project including data metrics such as number of plays, favourites, ratings, reviews, comments, and more, are no longer viewable online.

## Getting Started

A [Sony PlayStation 3 (PS3) video game console](https://en.wikipedia.org/wiki/PlayStation_3) and a copy of [Media Molecule's LittleBigPlanet 2 (LBP2) video game](https://en.wikipedia.org/wiki/LittleBigPlanet_2) are required to play the game. First-time LBP2 users will need to progress through the first world of the **Story** section to unlock the required **Community** section. From the **Community** section, select **Text Search** and either search for **Bomberman LBP2** (the level title) or **XZairX** (the PlayStation Network ID of myself, the level author). The former will return a large set results pertaining to user-generated Bomberman levels whereas the latter will only return the author's published levels. Simply navigate through the results until the Bomberman LBP2 level is located, select it, and the level encasing the game will start.

### Prerequisites

* Sony PlayStation 3 video game console
* LittleBigPlanet 2 video game

## Project Showcase

The following sections will detail the design and mechanisms of the numerous screens that the player can encounter when playing the game. These sections have been included to demonstrate the product to those who cannot meet the hardware prerequisites required to experience it first-hand. It also gives some insight into the ideology of some design decisions that were taken to improve the game after garnering player feedback. Any information relating to the design history of the product has been provided in block quotes to clearly separate it from the main description bodies of the project showcase.

### Video Demonstration

(Potentially coming soon)

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

## Authors

* Riaz Philippe - BSc Computer Games Graduate

## References

* [Bomberman LBP2 Level Link](https://lbp.me/v/q3q01np)
* [PlayStation 3](https://en.wikipedia.org/wiki/PlayStation_3)
* [LittleBigPlanet 2](https://en.wikipedia.org/wiki/LittleBigPlanet_2)
