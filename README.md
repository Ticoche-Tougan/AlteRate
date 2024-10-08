# AlteRate
rate the unique altered cards

- WHAT IS ALTERATE?

Altered TCG is an innovative collectible card game, owned by Equinox Corporation.
This app is not affiliated with Equinox, it is created by a fan for fans.
The illustrations are the property of Equinox and their authors (see: https://www.artstation.com/alteredtcg)

AlteRate is a tool that allows you to estimate the power of a single card from the game Altered. To do this you need to enter the information from
your card in the app, then a score is generated.
Since there are an infinite number of abilities, since there are an infinite number of unique cards in the world, it is impossible to implement all of them.
the abilities that will be found on the unique cards. So, the tool allows you to create a new ability using a sentence fragment.
For example, for the following capacity:
{reserve} You may put a card from your hand into Reserve. If you do: Target Character gains Anchored.
You can create it by clicking on the [+] button in the center of the card, then selecting sentence pieces from the drop-down lists:
DROP-DOWN LIST => SENTENCE PIECE
Trigger => {reserve}
Choice => You can put a card from your hand into Reserve
Punctuation => .
Condition => If you do it
Punctuation => :
Talent => A targeted Character gains Anchored
Punctuation => .
With these 7 drop-down lists you are able to add a new capability.
Just click the Save button (to save and continue creating another ability)
or Validate (to return to the card creation interface)
Note that a sentence fragment is ALWAYS present in one of the “category” lists (in green), and sometimes in several “term” lists (in blue).
So the following piece "A Targeted Character Wins Anchored" can be found in Talent, but also in Character, Target, Win.
It's up to you to choose your favorite list. Sometimes there are fewer items in one list than in another which makes searching easier.
Additionally, you can press a key on the keyboard to filter the list on that letter.


- HOW TO USE THE APPLICATION?
To launch the application, double-click on the file: Altered.exe
Fill in the values of your unique card in the following fields:
- Helping hand
- Reserve shot
- Forest value
- Mountain value
- Water value
Then select the card's capabilities from the drop-down lists (up to 3 max)
(lists are highlighted in gold when hovering over)
If the card has less than 3 abilities, do not select the additional drop-down lists.
Then select a support ability from the drop-down list if the card has one.
Select the Character name in the title at the top of the card
Finally, click on the calculate button (bottom right)
=> Scores are displayed at the bottom of the map.

If the ability does not exist in the ability list, press the "+" button in the center of the card, to
create a new unique ability, it will then appear in the ability list

- HOW TO READ THE SCORE?
It's as simple as a percentage.
Close to 0% is frankly bad.
Close to 100% it's insane!
The community can upload their maps generated by AlteRate, so you can compare your score with other unique maps:
https://drive.google.com/drive/folders/1N1m0nDZoN3GMcqzeqtkHLs9xf7A7Mh7x?usp=sharing
When you click on the calculate button, in addition to giving a score to your card, the application creates a screenshot which is placed in the
PNG directory. You just have to drag and drop this file into the shared drive directory.

- HOW IS THE CARDS PERCENTAGE SCALE CALIBRATED?
(valid from v0.27)
Very good question, thanks for asking. I use 2 reference cards that allow me to have a Min and Max value.
The Min value standard card is a (5)(5) 1/1/1 which is worth: 1.837%
The Max value standard card is a (1)(1) 5/5/5 which is worth: 99.193%
A vanilla card (1)(1) 1/1/1 is worth: 5%

Here is an example of a single card, whose score has changed depending on the scale used in different versions.
Powerful Jinn: (4)(4) 4/4/0
{main} You may pay {1}. If you do: Roll a die. On a 4+, draw a card. On a 1-3, resupply.
When I leave the Expedition Zone − You may put me into my owner's Mana Zone. If you don't, draw a card.

Scale v0.10+: 30.071%
Scale v0.25+: 75.941%
Scale v0.27+: 24.2%

- HOW TO PUT OR REMOVE SOUNDS?
Since v0.26 sounds have been added. It is possible to edit the Altered.exe.config file
To hear the sounds: <add key="SoundEnabled" value="true"/>
To not hear sounds: <add key="SoundEnabled" value="false"/>
Currently there is only one camera sound when clicking the calculate button (default is true)


/*
UPDATE NOTE [Backlog]:

Upcoming developments:
=> AlteRate version 1.0 release scheduled for September 13, 2024
- Developments after v1.0
[] Ability to filter with multiple letters entered on the keyboard
[] Notification confirming the registration of a new unique ability
[] Add logos instead of text {arrow}, {main}, {reserve}


---


v1.0 :
[o] Added a logger (Logs available in the Logs directory)
[o] An installer allows you to install AlteRate

v0.27: (02.09.2024)
[o] Improved HMI
[o] Filter in the list of Character names when typing a letter on the keyboard
[o] Sort Characters by Faction then by Name
[o] The extension logo can be changed
[o] Code optimization
[o] Taking into account KS Alt Art if the KS logo is selected
[o] Fixed some ability score
[o] The errata of the following 3 cards have been voluntarily reproduced (Illustrator errata BTG KS edition: Fahmi Fauzi):
- Amahle, Paria Asgarthi (Original BTG illustrator: Khoa Viet)
- Ouroboros inkwell (Original BTG illustrator: Khoa Viet)
- Jian, Assembly Supervisor (Original BTG Illustrator: Khoa Viet)
[o] Added new list for ability creation (Sacrifice, Boost, Card, All)
[o] automatic sorting (alphabetical order) of single ability creation lists
[o] Added background image for ability creation
[o] New Save button on the ability creation screen, to save and continue creating a new ability.
[o] When creating a new ability, automatically adds a punctuation mark if there is none.
[o] Feeding category/term drop-down lists
[o] Removed all unique abilities (scores no longer match the new scale)
[o] Added unique abilities
[o] Checking the scores of each ability piece (this profoundly changes the scores generated)

v0.26: (26.08.2024)
[o] Calculate button color adapts to faction
[o] Code optimization
[o] Improved HMI
[o] Filter on the lists of creation of a capacity
[o] Fixed some ability score
[o] Displaying a QR Code on the screenshot
[o] Added a sound (configurable) when calculating a score, at the time of the screenshot

v0.25: (24.08.2024)
[o] New illustration of the unique gem at the top of the card
[o] New gold design for faction logos
[o] Feeding category/term drop-down lists
[o] Added unique abilities
[o] Support zone does not appear on the screenshot if the unique card has no support ability
[o] Added a Faction and Out Of Faction logo in addition to the Character name
[o] Improved display of characters in the title dropdown
[o] New way to count points on a card
[o] Added subtypes of a character
[o] The illustrator's name can be seen by hovering the mouse over the Character's name
[o] Selecting a character by clicking to the left (faction) or right (OoF) of the name allows you to pre-select the faction on the map

v0.23: (22.08.2024)
- Code optimization
- Replaced the following Character files: Tinker Bell, Cloth Dancer Lyra, due to various issues
- Improved HMI
- Fixed a major bug in the calculation of support capacity
- You can see tooltips about power: biome set, ability 1, ability 2, ability 3, support.
- Animation of bars in biomes based on the number entered (either smaller or larger)

v0.22: (21.08.2024)
- Feeding of category/term drop-down lists
- Added unique abilities
- Added the release date of the version
- Fixed some ability score
- Creation of a shared directory _Our_uniques to allow players to publish the cards they have rated with AlteRate
link to this directory: https://drive.google.com/drive/folders/1N1m0nDZoN3GMcqzeqtkHLs9xf7A7Mh7x?usp=sharing
- Improved HMI
- The Reset button no longer appears on the map screenshot
- Display the backlog in order of priority (top = priority)
- Changed tab order: Hand cost > Reserve cost > Forest > Mountain > Water > Abilities
- Code optimization
- Percentage with always 3 digits after the decimal point in the PNG file name
- Raised capabilities text
- Added accents, diacritics and typography in the Character name

v0.21: (20.08.2024)
- Certain components no longer appear on the screenshot to make way for the Character illustration
- Implementation of characters that did not yet have illustrations
- Added thanks at the end of the README.txt file
- Ability to see the entire illustration if you keep clicking on it. Releasing the mouse button displays the statistics again

v0.20: (20.08.2024)
- Choose a Character by clicking on the title of the card, displays its illustration (if the illustration does not exist, one by default)
- Improved HMI
- Code optimization

v0.19: (08/19/2024)
- Ability to filter drop-down lists by typing a single letter on the keyboard
- Calculated a power percentage to give a clear indication of a single card score (instead of the average)
- Improved HMI
- Fixed some ability score

v0.18: (08/17/2024)
- Feeding of category/term drop-down lists
- Added unique abilities
- Added bottom right version of map
- Minor bug fixes
- Deduplication of unique abilities (if you create the same ability multiple times, only one will be taken into account)
- Fixed some ability score
- New format for file name: [<average>] <faction letter> <name> (<main score>_<reserve score>) <date>

v0.17: (08/14/2024)
- File name starts with average card score [(Main + Reserve) / 2]
- Added average score between hand and reserve
- Added main/reserve score in file name (in PNG directory) in the form [<Main>_<Reserve>]
- New button to completely reset the map (bottom left)

v0.16: (12.08.2024)
- Feeding of category/term drop-down lists
- Minor bug fixes
- Added capital letters in ability sentences
- Improved HMI

v0.15: (10.08.2024)
- Improved HMI
- Minor bug fixes
- Feeding of category/term drop-down lists

v0.13: (08.08.2024)
- Separation into Category and Term for the creation of a new capacity
- Major bug fixes
- Feeding of category/term drop-down lists

v0.12: (07.08.2024)
- Automatic sorting of capacities.txt and supports.txt files
- Ability to add a new ability or support via the interface (for now you have to restart AlteRate after creating an ability to see it in the list)

v0.10: (02.08.2024)
- Costs are now limited to numeric characters
- The title of a card is limited to 30 alphabetic characters and spaces
- Improved HMI
- New way to count points on a card
- Added unique abilities

v0.09: (31.07.2024)
- Improved HMI
- Code optimization
- Added abilities/supports from unique cards
- Export a screenshot to the PNG folder when clicking the Calculate button
- Possibility to give a title to the card (by clicking on UNIQUE)
- Improved performance for opening the ability and support list

v0.08: (30.07.2024)
- Improved HMI
- All abilities of the BTG set (C, R, F) are implemented
- All BTG set supports (C, R, F) are implemented
- Minor bug fixes

v0.07: (29.07.2024)
- Added icons in the text of abilities/supports
- Updated the capacities.txt and supports.txt files
- New way to count points on a card
- Added an icon for the application
- Minor bug fixes

v0.06: (27.07.2024)
- Unique card assets in the background
- Button that allows you to change the faction of the map (click on the faction logo at the top right)
- Added new abilities
- Added new support effects
- Minor bug fixes
- General improvement of the interface

v0.05: (26.07.2024)
- New interface on a single axiom card background
- Improved general stability

v0.03: (26.07.2024)
- Minor bug fixes
- Separation into 2 resource files capacities.txt and supports.txt
- Added capabilities in the file
- New way to count points on a card

v0.02: (25.07.2024)
- Minor bug fixes
- Added capabilities in the file

v0.01: (25.07.2024)
- Creation of the AlteRate application
*/

Acknowledgments:
Thanks to Régis Bonnessée for having the idea to create Altered, and to the entire Equinox team for making it a reality.
Thanks to the people (and ChatGPT) who helped me in this project, who advised me, or simply to the people who use AlteRate
Special thanks to those who have helped me a lot to move this project forward or actively participate in keeping Altered alive:
- Spiring, Pollux Troy, Keyuko, Amaury, JusteBBTV, Val & PL, ClaedeusFR, Maxildan, and I forget some


----------------------------------------------------------------------------------------------------------------------------------
If you encounter a bug, if you have a suggestion, you can write to me at Ticoche@gmail.com with the subject "AlteRate <free text>"
you can also contact me on discord: https://discord.com/invite/altered-tcg-francophone-1204719182957256774
Link to the shared drive directory: https://drive.google.com/drive/folders/1mAjCIdx8fq2zuu4UtM4W7jBZDvan4L_S?usp=sharing
Link to the unique cards screenshot database: https://drive.google.com/drive/folders/1N1m0nDZoN3GMcqzeqtkHLs9xf7A7Mh7x
----------------------------------------------------------------------------------------------------------------------------------
