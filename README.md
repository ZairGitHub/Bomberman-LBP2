# Bomberman LBP2
Repository designed to showcase Bomberman LBP2, a personal project undertaken in my own free time where I took it upon myself to explore the design philosophy of the Bomberman series and to learn about the practices of independent game development. The game is finished and fully functional, yet several planned features have been forcibly omitted as the game engine suffers from serious memory constraint issues.


## Getting Started
A [Sony PlayStation 3 (PS3) video game console](https://en.wikipedia.org/wiki/PlayStation_3) and a copy of [Media Molecule's LittleBigPlanet 2 (LBP2) video game](https://en.wikipedia.org/wiki/LittleBigPlanet_2) are required to play the game. First-time LBP2 users will need to progress through the first world of the **Story** section to unlock the required **Community** section. From the **Community** section, select **Text Search** and either search for **Bomberman LBP2** (the level title) or **XZairX** (the PlayStation Network ID of myself, the level author). The former will return a large set results pertaining to user-generated Bomberman levels whereas the latter will only return levels published by the author that was searched against. Simply navigate through the results until the Bomberman LBP2 level is located, select it, and the level encasing the game will start.


### Prerequisites
* Sony PlayStation 3 video game console
* LittleBigPlanet 2 video game


## Level Showcase
The following sections will detail the design and mechanisms of the numerous screens that the player can encounter when playing the game. These sections have been included to demonstrate the product to those who cannot meet the hardware prerequisites required to experience it first-hand. It also gives some insight into the ideology of some design decisions taken to improve the game after gathering player feedback.


### Video Demonstration
// Potential video demonstration


### TITLE Menu
This is the first thing the player sees upon entering the game. In the LittleBigPlanet series of games, players have the ability to customise the appearance of their avatars. This menu initially displays 4 default "naked" avatars in a sleeping state who will wake and be replaced by the custom avatars of players whose profiles are loaded into the game. Active avatars are backlit by a predetermined colour which corresponds to their player colour: an identifer which is later used during the main gameplay section of the game.

The menu is populated with a menu title header, a level title header, and the option to either jump to the the SETTINGS menu or the CONTROLS menu by using the displayed button prompt. All menus are solely controlled by the player who takes the position of the left-most avatar, a position which is assigned to the first profile that loads into the game.

//TITLE Menu Image


### CONTROLS Menu
This menu simply displays an interface which communicates the button mapping for the main gameplay section of the game. As the player moves through these menus, the positioning of the menu title header will shift either right or left to signify a forward or backward movement in menu progression. This menu previously featured additional button inputs which allowed for a more experimental style of play where the effects of special bombs could be chained together. These commands have since been compressed into a single input which faithfully only permits the use of one type of special bomb at any given time after user receiving user complaints of overcomplicating the control scheme of what is supposed to be a relatively simple game.

//CONTROLS Menu Image


### INSTRUCTIONS Menu
This menu holds the bulk of information used to inform the player of how the various objects they may encounter during the main gameplay function. The L1 and R1 buttons are used to toggle left and right between the objects presented to view their descriptions. These object descriptions were initially very elaborate and detailed averaging at around 4 lines each but they have since been simplified to a maximum of 2 lines. This reduction of clarity is a result of analysing player behaviours during the beta testing of the game. Players found that they would be helpless during gameplay despite having read through the object descriptions as the presented information was too profuse to be absorbed.

//INSTRUCTIONS Menu Image


### SETTINGS Menu
This menu holds a variety of customisation options which affect the inital state of the main gameplay to encourage replayability. To maintain consistentency with the control scheme of the other menus, L1 and R1 can be used to toggle left and right between the options of the settings. The Left Stick Up and Left Stick Down commands can also be used to toggle up and down between the different settings themselves. The button mapping for this functionality is not displayed as it is a natural instinct for users of the LBP2 community.

The leftmost column represents a setting's default value whereas the rightmost column is its maximum. All of these settings are self-explanatory save for "CAMERA" which increasingly reduces the number of visible objects during the main gameplay to optimise the running performance of the game.

//SETTINGS Menu Image


### PLAY
A new "PLAY" button prompt will appear on the "TITLE" menu after all of the other menus have been visited. It is accompanied by some information which informs the players of a hidden quick-start feature in the event that they should revisit the level. The "PLAY" function transports the players away from the menus and into the game arena where the main gameplay takes place.

In the earlier stages of development, the player could freely select between all of the different menus from the first screen of the level and this included the ability to select "PLAY." Unfortunately, this liberty resulted in naive newcomers haphazardly jumping straight into the main gameplay of the game with little to no clue on how to actually play the game. This robbed them of their enjoyment and jeopardised their very crucial first impressions, effectively sabotaging their own experience.
 
I aimed to redesign the menu system in a way that allowed for the game to be started as quick as possible for veterans and testing purposes, yet it also had to strike a balance that would encourage newcomers to explore the menus so that they were not left clueless by the time they entered the game arena. This compromise has resulted in a less user-friendly system that benefits from a welcome increase in player satisfaction.

// PLAY Option Image


### Gameplay (Single-player)
This screen shows the initial game state of the game arena. To the left is the player HUD and to the right is the Power-UP Key. These two components have been implemented to aid the player during gameplay as the level has been designed with newcomers to the Bomberman formula in mind. When playing alone, an information message exclusive to the single-player mode is activated to notify unwary players that the level has been designed to be enjoyed as a multiplayer experience.

// Single-player Information Message Image


### Gameplay (Multiplayer)
Players have two minutes to complete their objective: to survive as the last player standing by blowing the other players up. Players will drop bombs in an effort to remove the soft blocks that obstruct their path between one another. In doing so, they will discover power-ups which they can pick up to strengthen their ability to survive. If two or more players are alive after the alloted two minutes have passed, the game is declared to be a draw and the alive players share the victory together.

// Multiplayer Frame Image


### Photo Session
After the game ends by means of a win, loss, draw, or time out, all of the players are transported to this screen where they have a few seconds to change their avatar's built-in expression and pose for a quick photo session. This section is completely irrelevant to the game and is catered to that of the LBP2 community itself. LBP2 allows for players to upload in-game photos to their profiles as a means of sharing their experiences. Uploaded photos do not provide information for where the picture was taken when viewed in-game so the level title has been provided for a reference to help share the level. This section is optional and can be freely skipped by the winner(s) of the game without penalty.

// Photo Session Image


### Final State
// Thanks for playing


### Omitted Features
Rounds, Pressure Blocks, Bomb Kick, Bomb Throw, Bomb Punch, Penetration Bomb
(may be merged into Final State)


## Authors
* Riaz Philippe - University of Essex BSc Computer Games Graduate


## References
* [PlayStation 3](https://en.wikipedia.org/wiki/PlayStation_3)
* [LittleBigPlanet 2](https://en.wikipedia.org/wiki/LittleBigPlanet_2)
* [Bomberman LBP2 Level Link](https://lbp.me/v/q3q01np)

