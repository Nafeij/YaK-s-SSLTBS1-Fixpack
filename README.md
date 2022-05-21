 
 3.1 (Unreleased)
 
    [FIXED] Importing a save using a version of Saga 2 with the BS2 fixpack installed causes discrepancies with Nid's upgrade points. She receives 8 more points than she's supposed to and her base version has -2 points.
 
 3.0
    
    [FIXED] Due to complicated dialogue interactions, Alette's dialogue about Egil's death still does not appear after he is killed by Onef, whereas it DOES appear if he was already previously dead. Egil is literally dying so much it's breaking the causality of the game. This has hopefully been fixed for good this time round.
    
    [FIXED] When losing to Bellower after the arrow is fired, the win cutscene (Alette/Rook and Iver talking about the death) triggers regardless, due to the saga1 "bellower_fight_completed" happening shadowing the "battle_lost" happening. Added a battle victory check to circumvent this.
    
 2.2
    
    [FIXED]: Very nasty bug that caused issues on Eirik, Griss and Ekkill when importing saves to BS2 (which will transfer to BS3 too);
    
    [FIXED]: Valgard lost his white tunic in the last patch, luckily he found it again and now doesn't wear the orange tunic of a common raider anymore;
    
    [FIXED] Bellower final battle correctly awards renown and shows the ending screen again, using a different and better solution;
    
    [TWEAKED] Eyvind's kills (14), Nid's (2, that joins at Rank 2) and Sigbjorn's (14), just to make promotions in Banner Saga 2 easier and more consistent;

    [FIXED(ENG)] Several typos in the dialogues and in the descriptions (string.json).
 
 2.0
 
    [FIXED] The importing of BS1 save into BS2 being inconsistent. Now you will not lose anymore the wrong item equipped by the hero killed by Bellower, nor lose promoting done before the last fight, renown gained/spent or items bought in the market JUST before the last fight and, of course, kills done in last fight. What i have changed, in further details:

        1) The save done just after you choose who will shot the arrow is now called "sav_crafters", with a proper description "The Silver Arrow: A treacherous trick" (ENG);

        2) A new save is created (with all the right vars in place) AFTER you defeat Bellower (it's the new "sav_finale"), with a proper new image (a Boersgard panorama, free of Dredge and more focused on the river - "Onward" was playing in my mind);

        3) A new variable is created to control Boersgard's view composition (Dredge/No Dredge/Bellower Showing/Bellower clickable), "7_bellowercomes" to replace the purpose of "7 boersbellow", that's still there cause is also used as a prerequisite to import the save into BS2. Deleted also the code that zeroed "7 boersbellow" after killing him (so BS2 will correctly recognize the file). This way we could have a working and consistent importing of promoted heroes/renown/kills/items and whatever into BS2, editing files just from BS1 side, while lefting untouched BS2 files Importing tested multiple time (Rook/Alette) on the latest vesion of both games ;

    [ADDED] New and consistent icons for the Skalfing Chieftain and his gingerish, grey dressed thugs (which are present in the tutorial, in the Meadhouse battle and in the Ash Mead Battle, in Boersgard);

    [FIXED] The state of Boersgard's "Find a safe place for caravan to stay" event is not saved, so, if you reaload a game the event will bug itself (see here);

    [FIXED] Bellower Battle not awarding any renown at all and not showing the battle ending banner (with injuries, renown gain etc.);

    [TWEAKED] Bellower (phase two) is now considered a "Rank 11" enemy, so, on death it will show (and will award) a "+10 Renown" banner. Holy cow, he's the Immortal Sundr! Pay some respect!

    [FIXED] When Hakon will arrive in Boersgard, we now could have two outcomes: a) If Ludin died in Ridgehorn, we will get the usual 280 varl and 315 supplies. b) If Ludin is alive, we will get 280 varl, 62 fighters (less than half of his retinue) and 315 supplies;

    [FIXED]In Reynivik, if you help Sig (and win), following option #2 and #3, will end in having this text when you leave the village: "With some help you gather up the casks of mead and head back to the caravan, Sigbjorn and the other survivors in tow. The caravan gives the boisterous varl a large berth as you set out for Boersgard.", but no one actually joins except Sig.

    I counted every single entity in the inn during the battle and there were 42 peasants, at least 8 people with weapons (fighters)and a dog, so i added exactly 42 clansmen and 8 fighters. I am really sad not having the opportunity to add the dog. Poor dog;

    [FIXED] Rook ONLY required in party for Onef's ambush battle;

    [FIXED] When Onef attackd, text says his fighter from Frostvellr betray you (and kill some clansmen), but you don't lose any fighter at all! Now you will lose 29 fighters, assuming some of them died due to wars/events/potential starvation;

    [FIXED] In the dialogue after the fight, a bug prevented Alette's comments on Egil's death, if he died at the hands of Onef (showing always the conversation as if he died in other circumstances);

    [FIXED] In the forced camping after the battle, "Leave" button is disabled until you finish your conversation with Ekkill (if alive);

    [FIXED] In the aforementioned conversation, if he is still a prisoner, you could chose "I need to get going" (ending the conversation) only after deciding to banish him OR unbind him (and his men). It's odd to just end the dialogue and silently getting him in the roster while he's still a former prisoner;

    [FIXED] In the same case, when you unbind him you will accept his fighters too (+39, assuming some of them died during the travel) and text is modified accordingly (singular to plural etc.);

    [FIXED] Got rid of THE TWO NOTORIOUS OBNOXIOUS, FILTHY, MADDENING, FAEN TREES (In the woods were ambush occurs and on the way to Frostvellr, after Hogun's & Mogun's village;

    [FIXED] When leaving Sigrholm, if you go for "Caulk the wagons and float across", you will go back in time (-2 days), GREAT SCOTT! ;

    [FIXED] The wounded varl random event, not removing 1 supply after you left him medicine and food;

    [FIXED] The two random event involving the old man Unnarr, not adding/removing 1 clansman when he joins/vanishes from the caravan;

    [FIXED] In the abandoned giant hall random event, a bug prevents you from losing 11 clansmen;

    [FIXED] In the wildfruit random event, if you "Offer a piece to one of the animals in the caravan" and then chose "Gather as much as you can", you get the wrong ending, the same of discouraging them from gathering;

    [FIXED] In the first part of the missing supplies random event, there is an error preventing you to REALLY lose 5 supplies;

    [FIXED] In the third part of the missing supplies random event, there a couple of bugs preventing you to lose one or both clansmen (the poor boys);

    [FIXED] Two bugs that will cause Nid to acts as if Ekkill joined the caravan while he doesn't (and also potentially mess up while importing the game to Saga2;

    [FIXED] Nid ONLY required in party in her debut battle;

    [FIXED] The bug that, when Ubins joins Rook's caravan after Einartoft, causes warrior to be added ONLY if Gunnulf is dead. Also, it will award +6 varl instead of +15 fighters and +5 varl because at that point there should be no human left in Einartoft and because too many fighters will prevent the breach event in Boersgard from happening;

    [FIXED] A bug that, when leaving Einartoft without trying/destroying the bridge, grants two times the amount of volunteers/wounded varl joining (38*2) and two times the 30 moral loss. Also, since Krumr remains to help, varl from Wyrmtoe are removed from the caravan;

    [FIXED] Adjusted the "many" varl that join if you fight three days on the bridge and let Iver destroy the bridge from 23 to 43. Twentythree could not be "many", they're actually less than the wounded/volunteers that joins when you just leave;

    [FIXED] Slightly increased the varl losses in Boersgard if you don't help Iver on the wall for a balancing purpose, so the breach event will likely happens with more or less the same chances;

    [FIXED] When Eyvind awakes, after saving Iver and dream-talking with Juno, Rook tells him he slept for a couple days, but time has not adavanced;

    [FIXED] When Oddleif train more archers, if you go for "Stand by the women becoming fighters" you will lose 35 clansmen and gain 25 fighters, it should be -25/+25;

    [FIXED] In frostvellr, after you tend the wounded, choosing "We'll wait and confront them" will not advance the time of 1 day;

    [FIXED] At the beginning of Chapter 4, if you stayed outside, when avoiding the third fight with dredge, on chosing "Nobody could be alive under there...", text will tell they hopeless join you regardless, but nothing happens. Now they join (+39 clansmen), but you lose 15 morale too;

    [FIXED] In Ridgehorn, if Ludin leaves (and die horribly with his retinue) no human fighter are lost. It will makes sense if ALL the human fighter will follow their Prince;

    [FIXED] When you are in the woods, Ch3, the dialogue option "We're going to wait them out" will not correctly advancr days by 1, if selected first;

    [FIXED] The error preventing the second in-camp conversation with Ubin from happening. It will fire up at the first camping after the treasury cart event, if you'll lose the tithe (sending back some varl with the taxes will prevent the event from popping, as intended);

    [FIXED](ENG) Fasolt having Saga2's description (causing a spoiler);

    [FIXED] At the very beginning of Ch3, if you dissed Eirik, Mogr will say: "I wasn't able to get as many warriors from Strand as you wanted, and only half as many weapons." and you will gain nothing. I think that "not as many as you wanted" doesn't mean "zero", so intead of the 100 varl, 100 fighters and supplies, you will now get only 50 varl and 35 fighters;

    [FIXED] In the tutorial battle ending screen, you get +6 Renown, but Ubin's caravan start whit just 5. Do you remember that missing faen renown needed to promote that hero, buy that bloody item or that vital bunch of supplies? Well, i've found where it was hiding ;

    [FIXED] Nid lacking two stat point to allocate;

    [FIXED] Sigbjorn missing 4 WIL points (compared to his starting stats in Saga2)

    [FIXED] Gunnulf lacking the two kills from the tutorial;

    [FIXED] Grenilund location not clickable on the map;

    [RESTORED] A color version of the Raidmaster enemy unit (v.0);

    [CHANGED] Unlocked Tryggvi by default, as explained in Aleo's thread. TO STOIC: If it's a problem, just let me know and i would remove that part.

    [CHANGED] Starting difficulty is now "Hard", so it will not reset to "Normal" if you start a new game, possibly wrecking the achievement if you didn't notice it soon.

    [FIXED](ENG) Several typos in map's, item's and unit's descriptions. For a detailed list of all the changes in "strings.json, look here.

    [FIXED](ENG) Lots of typos/missing words in the dialogues. For a detailed list, ordered by file edited, look here);

    [BONUS] As a bonus, i set in place the correct values to have a working Bolverk in Saga1, just for fun. To add him enable developer mode and type in the console: 

        `saga roster_add bolverk`
        
------------------------------------------------------------------

Spare Some Love To Banner Saga 1 - version 3.0
[This version is ONLY for BS1 2.58.17]

This is the active branch of the original SSLTBS1 Fixpack for Banner Saga 1, by YaK of all Trades (YaK#2186).

This corrects all the previous nasty bugs, inconsistencies and typos in the video game Banner Saga 1 by Stoic Studios!

Many thanks to:
Gestaltzerfall, who updated TBSDecompiler - http://www.mediafire.com/file/wun36alp6ojlkjk/TBS_Decompiler3.2.3.air/file
Ratatoskr
Drake713
Nafeij
Aleo

Please report any bugs in Issues.

------------------------------------------------------------------
INSTALLATION:
    Just uncompress the .zip in your "../steamapps/common" folder. It will ask you to overwrite some files, it's all right! The archive comes with backups just in case! (the ones with a .orig extension).
UNINSTALLATION:
    Just delete the files and rename the backups OR verify the integrity of game files in Steam.
    
------------------------------------------------------------------

Mirrors -  | 
