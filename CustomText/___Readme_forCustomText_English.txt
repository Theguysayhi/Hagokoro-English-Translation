***********************************************
*****   About HAGOKORO:English version    *****
***********************************************

Regarding non-Japanese language options for HAGOKORO, 
the most we can offer is a machine translation as well as the ability 
for users to freely edit and improve on the text by themselves. 
We cannot add a manual translation ourselves as it'd take a lot of time and 
money and hamper the actual game's development.

We hope you understand.




***********************************************
*****       Please                        *****
***********************************************

*We recommend that you make a backup of the text file before editing.

* The creator "excessm" wants an English translation by volunteers of this manual.


***********************************************
*****	Prohibited characters 	****
***********************************************

"=" : This is used to separate sentences.

"|" : This is used to separate sentences.

"@" : This is used to separate sentences.

"/" : This is used to separate sentences.

"," : This is used to separate sentences.

***********************************************
*****	Description of each text file 	****
***********************************************

[Dialogue_table.txt]
 -> The dialogue of the enemy used in the defeat event is written.
　　The text written here is used in [Text_Event.txt].


[Name_table.txt]
 -> A text file that stores the names of people.


[Text.txt]
 -> Not used for now. 


[Text_enemyWord.txt]
 -> This is the enemy dialog used in battle.


[Text_Event.txt]
 -> Contains texts used in the demoscene. 
Sexual events are also written in this file.

[Text_Item.txt]
 -> Contains names and descriptions of items, weapons, and armor.


[Text_Notice.txt]
 -> This is a text file that describes the system.


[Text_QuestData.txt]
 -> The name and description of the tactical mission are written.


[Text_UI.txt]
 -> Contains characters used for each UI, including buttons.



*****************************************************
******	Description of symbols used in each text file	******
*****************************************************

"#"
->This is used to separate sentences.Never erase or add to it.


","
-> This is used to separate sentences.Never erase or add to it.


"/"
-> This is used to separate sentences.Never erase or add to it.


First numbers such as "10005", "501", "51"
-> An index used in the game.
Never erase, add or rewrite.


Words covered in [] such as "You hear the voice of your [ba]...@" and "[Tosyu]"
-> A word that can be replaced with a unique word in the game.
Never rewrite or add to it.


****************************************************
*****	Symbols used only in Text_Event.txt	*****
****************************************************

"@"
-> This is used to separate sentences.Never erase or add to it.
　
"/"
-> This is used to separate sentences.
 This is the number written on the left side of "/"
It is used to display the person name field. For example in Text_Event.txt

"13/An intruder who masters three weapons ...
The report of the sights seems to be true. @"

Then, "13" represents the speaker. This number is associated with "Name_Table.txt"
If you look at it, you can see that it is a "Bibi" 's Dialog.


Lines starting with "]]", such as "]] 0016"
-> It is used in the production to display the enemy.
Never rewrite or erase.


Lines starting with "[[", such as "[[020000"

-> It is a description of darkening, ejaculation, posture change, etc.
Please do not rewrite or erase until you are familiar with the mechanism.
Below this is a description of each production effect.


Lines starting with  ]]] ", such as "]]]|W1|H1|t0|Y0.43|S0.20@"

-> This is a command to display the cut-in camera.
It is separated by "|" and a cut-in based on each number is inserted.
　
  W1：Specifies the width of the cut-in camera. 
	If you enter "W0.3" from 0 to 1, it will be about 30% of the screen width.
	The camera will be displayed.

　H1：Specifies the vertical width of the cut-in camera. 
	If you enter "H0.8" from 0 to 1, the height of the screen is about 80%.
	The camera will be displayed.
　
  t0：Specify the enemy to watch. If it is "t0", 
	watch the first enemy, and if it is "t2", watch the third enemy.
	It is in the form of.

　Y0.43：Specify the height to gaze at. 
	For example, the lower the number, such as "Y0.25", the lower it becomes.
	The higher the number such as "Y0.55", the more attention is paid to the upper part such as the face.

　S0.20：Specifies the zoom factor of the cut-in camera. 
	The smaller the number, the zoom in.
	"S0.20" is a considerably improved zoom rate. "S0.35" is normal


Lines starting with "[[[", such as "[[[00003@"

->Change the background. Never rewrite or erase it.



List of productions such as ["[[020000"]]

[[000001：The currently displayed enemy shifts to the trampling angle and enters the standby state.
(Do not actually trample)
* Do not use in the absence of enemies

[[000002：Trampling is performed with a probability based on the trampling probability of "various settings".
↑ "[[000001": Do after preparing for trampling

[[000003：Ignore the user settings and trample in a roundabout way.
↑ "[[000001": Do after preparing for trampling

[[000004：Ignore user settings and perform a kicking trampling.
↑ "[[000001": Do after preparing for trampling

[[000008：The currently displayed enemy shifts to a special etch attack.
* Strictly prohibited from using in the absence of enemies

[[000009：The currently displayed enemy shifts to the production etch attack.
* Strictly prohibited from using in the absence of enemies

[[000010：The currently displayed enemy shifts to the back etch attack.
* Strictly prohibited from using in the absence of enemies

[[000011：The currently displayed enemy shifts to the normal state.
* Strictly prohibited from using in the absence of enemies

[[000015：Insert a production that sounds "Dokun".

[[000017：The first enemy makes a color scheme motion.

[[000020：The enemy on the left side at the time of the actual etch attack and the back etch attack
Make a start.

[[000021：Enemies on both sides at the time of the actual etch attack and the back etch attack
Make a start.

[[000040：Ejaculate when trampled.

[[000045：Ejaculate in a special etch state.

[[000046：The movement speeds up in the special etch state.

[[000050：Ejaculate at the time of production etch attack and back etch attack.

[[000051：Resume the blame from the ejaculation state at the time of 
the actual etch attack and the back etch attack.
If there are enemies attached to the left and right, the enemy's leaning will also be canceled.

[[000052：It becomes a loose movement at the time of 
the actual etch attack and the back etch attack.

[[000099：At the time of production etch attack, back etch attack, trampling, special etch attack
Become able to ejaculate endlessly

[[000100：Erase the cut-in camera

[[000200：Enemies attached to the left and right during the actual etch attack and back etch attack
Began to actively set up a stake.

[[000201：Enemies attached to the left and right during the actual etch attack and back etch attack
It will be possible to aggressively set up strong restraints.

[[000210：Enemies attached to the left and right during the actual etch attack and back etch attack
No more aggressive work in process.

[[000300：Place weight (0.5 seconds)

[[000301：Place weight (1.0 seconds)

[[000302：Place weight (1.3 seconds)

[[000303：Blacken the screen

[[000304：Restore the blackening of the screen.

[[009999：Erase the currently displayed enemy

[[020000：Scene change production

[[012000：No change
[[012010：No change
