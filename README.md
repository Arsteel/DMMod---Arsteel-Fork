![DMMoD Logo large](https://github.com/DarkMasterMan0/DMMod/assets/87884578/9c781fee-a103-4212-835b-54e764fa8f28)

# Manual Installation and Launch / D2RLaunch
Download the files by clicking the green `Code` button near the top of the page and download the ZIP, or download the files from the `Releases` tab on the right side.

Drop the top-level DMMod folder into your D2R `mods` folder (the file path will look like `Diablo II Resurrected > mods > DMMod > DMMod.mpq` if you did it correctly), if you don't have a `mods` folder then create it in your D2R folder.

Create a new shortcut of `D2R.exe` from your base D2R directory then add `-mod DMMod -txt` to the target line (it will look similar to `"H:\Games\Diablo II Resurrected\D2R.exe" -mod DMMod -txt` if you did it correctly). You can now use this shortcut to launch D2R with DMMod as the active mod.

You can also use Bonesy's D2RLaunch mod manager to launch DMMod or other D2R mods, download it from here: https://www.d2rmodding.com/d2rlaunch After you install it you can download DMMod using the `Download New Mod` button on the right side and selecting DMMod in the tab that appears. Be aware that I am currently learning D2RLaunch's functionalities so some things might break if you try using them (like the `Check for Mod Updates` button, it has some weird behavior that can brick the DMMod install and I have yet to figure out what causes it).

**BACKUP YOUR SAVES OFTEN:** Any time your computer has a hard shutdown (crash, power outage, pulled plug, etc.) it will cause the active RAM to get corrupted which includes your currently active character and the respective shared stash (softcore/hardcore). You'll find your save files in `C:\Users\username\Saved Games\Diablo II Resurrected\DMMod`, you can backup the whole folder or just the `.d2s` (character) and `.d2i` (shared stash) files. D2RLaunch has the option to automate backups, you'll find it under the `Options > QoL Options > Auto-Backup Characters` section.

You can check out older versions of DMMod at [DMMod Archive](https://github.com/DarkMasterMan0/DMMod-Archive), use the installation instructions above with the DMMod folder of whichever version you'd like.

# What is DMMod?
DMMod is a mostly vanilla (like ~95% vanilla I'd say) mod that aims to address some of the balance gaps in vanilla D2R in regards to items and skills with a combination of nerfs, buffs, and other changes while attempting to maintain the "original feel" of the game. **No changes to drop rates** (technically a change to Hell Baal's quest drop but that's about it).

Some examples of the changes include buffs/changes to lots of the weaker sets and uniques (whether that be by increasing existing stats or adding new stats), a few buffs to underused runewords (like Holy Thunder and Venom) and nerfs to overtuned runewords (Stealth, Spirit, Insight, Grief, Enigma, Mosaic outright removed, etc.), buffs/changes to weaker/underused skills (like Poison Dagger and Iron Maiden) and a few nerfs to overtuned skills (like Blessed Hammer and Holy Shield), changes to magic/rare item affixes (adding a max level cap to lower tier affixes to reduce the size of the affix pool at higher levels for example).

I may or may not make more changes in future versions, I was going to mess with crafting recipes and a few more skills (Poison Explosion, Maul, etc.) but I'm really getting the itch to actually play D2R instead of modding it so I'm not making any definite plans regarding future changes for the moment. :P

Feel free to make your own changes, that's why I included the .txt files. :) If you do decide to release your own version of DMMod publicly then you must release it with your modified source code as well as per the GPL 3.0 license.

# Credits
Thanks to:

* Blizzard Entertainment and Vicarious Visions (now Blizzard Albany) for creating D2/D2R and allowing/expanding modding capabilities (wish we had TCP/IP tho T_T).

* Bonesy for the big help with guidance on specific edits, his video guides, and the massive amount of effort he's put into the D2R modding scene in general. Check out his stuff on [D2RModding.com](D2RModding.com) and check out the D2R-Modding Discord!

* The Phrozen Keep for their many indepth guides on modding original D2, the vast majority of which are still applicable to D2R. Check them out at [d2mods.info](d2mods.info) and check out their Discord as well!

* Vaska, Pavke, and Arsteel for item ideas and various discussions.

* id Software for creating the awesome Doom games and the badass logo that I re-used for DMMod.

# Changelog
Sorted by alphabetical order when sorting by name in File Explorer. Patch changelogs are also below, the original (1.00) changelog remains mostly unchanged besides fixing typos and adding ~~strikethroughs~~ when the relevent info has been changed by a later patch and the patch that changed it will be noted in paranthesis. The original DMMod changes will be listed below the Arsteel Patch notes.

**Arsteel Patch 0.01c Changelog**

Added missing json files to data/local/lng/strings

**Arsteel Patch 0.01b Changelog**

Replaced the main directory folder with the correct version for the patch notes. Oops. 

**Arsteel Patch 0.01 Changelog**

https://docs.google.com/document/d/1oFkBNy5SQwizKXKrtklme89k9g5hvqqpdJv_08bKXeA/edit?tab=t.0

**Arsteel Patch 0.00 Changelog**

##### data\global\excel\levels.txt

* Increased the unique/champion mob density in most areas in Normal difficulty, to match the density in Nightmare difficulty. Exclusions include The Blood Moor, The Den of Evil, and the Forgotten Tower which maintain their original values. The Cold Plains has an increased elite density of 2-3 instead of 4-5 like in Nightmare.


##### data\global\excel\runes.txt

* Ancient’s Pledge
 * Changed itype1 from shld to weap (Runeword is now made in all weapons instead of shields)
 * Deleted all stats from T1Code1 to T1Max4 (Cleared all stats from the runeword)
 * Added dmg% to T1Code1, and 50/50 to T1Min1 and T1Max1 (Added 50% Enhanced Damage)
 * Added dmg-cold to T1Code2, 75 to T1Param2, and 3/14 to T1Min2 and T1Max2 (Added 14-22 Cold Damage with 3 second duration)
 * Added dmg-mag to T1Code3, and 13/19 to T1Min3 and T1Max3 (Added 13-19 Magic Damage)
 * Added swing2 to T1Code4, and 20/20 to T1Min4 and T1Max4 (Added 20% Increased Attack Speed)
 * Full stats as follows:
  * 50% Enhanced Damage
  * 20% Increased Attack Speed
  * 5-30 Fire Damage
  * 1-50 Lightning Damage
  * 3-14 Cold Damage with 3 second chill
  * 75 Poison Damage over 5 seconds
  * 13-19 Magic Damage
 * Holy Thunder
  * Deleted all stats from complete (Runeword can no longer be made)
 * White
  * Changed T1Code1 from skilltab to nec, removed 7 from T1Param1, and reduced T1Min1 and T1Max1 from 3/3 to 1/1 (Changed +3 Poison & Bone Skill to +1 Necromancer skills)
  * Reduced T1Min6 and T1Max6 from 2/2 to 1/1 (Reduced Bone Spear skills bonus from 2 to 1)
  * Reduced T1Min7 and T1Max7 from 4/4 to 3/3 (Reduced Skeleton Mastery bonus from 4 to 3)


##### data\global\excel\gems.txt

* Chipped Diamond
 * Reduced shieldMod1Min and shieldMod1Max from 6/6 to 4/4 (Reduced All Res in shields from 6 to 4)
* Flawed Diamond
 * Reduced shieldMod1Min and shieldMod1Max from 8/8 to 6/6 (Reduced All Res in shields from 8 to 6)
* Diamond
 * Reduced shieldMod1Min and shieldMod1Max from 11/11 to 8/8 (Reduced All Res in shields from 11 to 8)
* Flawless Diamond
 * Reduced shieldMod1Min and shieldMod1Max from 14/14 to 10/10 (Reduced All Res in shields from 14 to 10)
* Perfect Diamond
 * Reduced shieldMod1Min and shieldMod1Max from 19/19 to 13/13 (Reduced All Res in shields from 19 to 13)


##### data\global\excel\weapons.txt

* Military Pick
 * Increased mindam and maxdam from 7/11 to 9/14 (Increased damage from 7-11 to 9-14)
* Scepter
 * Decreased mindam and maxdam from 6/11 to 3/7 (Decreased Scepter damage from 6-11 to 3-7)
* Two-Handed Sword
 * Increased mindam and maxdam from 2/9 to 3/11 (Increased 1h damage from 2-9 to 3-11
 * Increased 2handmindam and 2handmaxdam from 8/17 to 10/21 (Increased 2h damage from 8-17 to 10-21)
* Claymore
 * Increased mindam and maxdam from 5/12 to 7/18 (increased 1h damage from 5-12 to 7-18)
 * Increased 2handmindam and 2handmaxdam from 13/30 to 15/34 (Increased 2h damage from 13-30 to 15-34
* Giant Sword
 * Increased mindam and maxdam 3/16 to 6/20 (Increased 1h damage from 3-16 to 6-20)
 * Increased 2handmindam and 2handmaxdam from 9/28 to 14/33 (Increased 2h damage from 9-28 to 14-33)
* Bastard Sword
 * Increased mindam and maxdam from 7/19 to 12/22 (Increased 1h damage from 7-19 to 12-22)
 * Increased 2handmindam and 2handmaxdam from 20/28 to 22/34 (Increased 2h damage from 20-28 to 22-34)
* Flamberge
 * Increased mindam and maxdam from 9/15 to 15/19 (Increased 1h damage from 9-15 to 15-19)
 * Increased 2handmindam and 2handmaxdam from 13/26 to 20/39 (Increased 2h damage from 13-26 to 20-39)
* Dagger
 * Increased maxdam from 4 to 5 (Increased damage range from 1-4 to 1-5)
* Dirk
 * Increased mindam and maxdam from 3/9 to 4/10 (Increased damage range from 3-9 to 4-10)
* Kris
 * Increased mindam and maxdam from 2/11 to 3/13 (Increased damage range from 2-11 to 3-13)
* Blade
 * Increased mindam and maxdam from 4/15 to 5/17 (Increased damage range from 4-15 to 5-17)
* Javelin
 * Decreased minmisdam and maxmisdam from 6/14 to 5/12 (Decreased Javelin throw damage from 6-14 to 5-12)
* Spear
 * Increased 2handmindam and 2handmaxdam from from 3/15 to 6/19 (Increased damage from 3-15 to 6-19)
* Trident
 * Increased 2handmaxdam from 15 to 24 (Increased damage from 9-15 to 9-24)
* Brandistock
 * Increased 2handmindam and 2handmaxdam from 7/17 to 16/23 (Increased damage from 7-17 to 16-23)
* Spetum
 * Increased 2handmindam and 2handmaxdam from 15/23 to 18/30 (Increased damage from 15-23 to 18-30)
* Short Bow
 * Increased 2handmaxdam from 4 to 5 (Increased damage from 1-4 to 1-5)
* Hunter’s Bow
 * Increased 2handmaxdam from 6 to 7 (Increased damage from 2-6 to 2-7)
* Composite Bow
 * Increased 2handmindam from 4 to 5 (Increased damage from 4-8 to 5-8)
* Light Crossbow
 * Increased 2handmindam and 2handmaxdam from 6/9 to 7/11 (Increased damage from 6-9 to 7-11)
* Crossbow
 * Increased 2handmindam and 2handmaxdam from 9/16 to 12/20 (Increased damage from 9-16 to 12-20)
* Heavy Crossbow
 * Increased 2handmindam and 2handmaxdam from 14/26 to 18/30 (Increased damage from 14-26 to 18-30)
* Repeating Crossbow
 * Increased 2handmindam and 2handmaxdam from 6/12 to 8/14 (Increased damage from 6-12 to 8-14)


##### data\global\excel\uniqueitems.txt

* The Gnasher
 * Decreased lvl from 7 to 3 (Reduced the required monster level for this item to drop from from 7 to 3)
 * Increased min1 and max1 from 8/8 to 12/12 (Strength bonus increased from 8 to 12)
 * Increased min4 and max4 from 60/70 to 70/90 (Enhanced Damage range increased from 60-70 to 70-90)
* Deathspade
 * Decreased lvl from 12 to 8 (Reduced the required monster level for this item to drop from from 12 to 8)
 * Increased min3 and max3 from 15/15 to 25/25 (Increased attack rating bonus from 15% to 25%)
 * Increased min5 and max5 from 60/70 to 70/85 (Enhanced Damage range increased from 60-70 to 70-85)
* Bladebone
 * Decreased lvl from 20 to 15 (Reduced the required monster level for this item to drop from from 20 to 15)
 * Increased min5 and max5 from 8/8 to 11/11 (Increased minimum fire damage from 8 to 11)
 * Increased min6 and max6 from 12/12 to 14/14 (increased maximum fire damage from 12 to 14)
 * Increased min7 and max7 from 30/50 to 111/111 (Enhanced damage range changed from 30-50 to 111)
* Mindrend (Skull Splitter)
 * Decreased lvl from 28 to 23 (Reduced the required monster level for this item to drop from from 28 to 23)
 * Changed prop3 from ltng-min to dmg-ltng/lvl. Set par3 to 16. Removed all stats from prop4 to max4 and moved the other stats over. (Changed lightning damage from 1 to 12-15, to +2 maximum lightning damage per level)
 * Increased min6 and max6 from 15/15 to 20/20 (Increased Open Wounds chance from 15 to 20)
* Rakescar
 * Reduced lvl from 36 to 27 (Reduced the required monster level for this item to drop from 36 to 27)
 * Increased min1, max1 and min2, max2 to 384 (Increased poison damage from 38 over 3 sec to 113 over 3 sec)
 * Increased min6 from 75 to 110 (Enhanced Damage range increased from 75-150 to 110-150
* Fechmars Axe (Axe of Fechmar)
 * Reduced lvl from 11 to 7 (Reduced the required monster level for this item to drop from from 11 to 7)
 * Reduced lvl req from 8 to 5 (Reduced the required level to equip from 8 to 5)
 * Added dmg-cold/lvl to prop5 and 16 to par5 (Added +2 maximum cold damage per character level)
* Goreshovel
 * Reduced lvl from 19 to 14 (Reduced the required monster level for this item to drop from 19 to 14)
 * Increased min4 and max4 from 40/50 to 70/100 (Enhanced damage range increased from 40-50 to 70-100)
* The Chieftan (The Chieftain)
 * Reduced lvl from 26 to 17 (Reduced the required monster level for this item to drop from 26 to 17)
 * Increased min1 and max1 from 100/100 to 115/115 (Enhanced damage increased from 100 to 115)
 * Increased max5 to 130 (Increased lightning damage range from 1-40 to 1-130)
* Brainhew
 * Reduced lvl from 34 to 25 (Reduced the required monster level for this item to drop from 34 to 25)
 * Reduced min4 and max 4 from 10/13 to 4/7 (Reduced mana steal range from 10-13 to 4-7)
 * Increased min5 and max5 from 50/80 to 160/200 (Enhanced damage range increased from 50-80 to 160-200)
* The Humongous (Humongous)
 * Reduced lvl from 39 to 31 (Reduced the required monster level for this item to drop from 39 to 31)
 * Increased min1 and max1 from 20/30 to 30/50 (Increased strength bonus from 20-30 to 30-50)
 * Increased min5 and max5 from 20 to 40 (Increased added requirements from 20% to 40%)
 * Increased min6 and max6 from 80/120 to 150/250 (Enhanced damage range increased from 80-120 to 150-250)
* Iros Torch (Torch of Iro)
 * Reduced lvl from 7 to 3 (Reduced the required monster level for this item to drop from 7 to 3)
* Gravenspine
 * Reduced lvl from 27 to 24 (Reduced the required monster level for this item to drop from 27 to 24)
* Umes Lament (Ume’s Lament)
 * Reduced lvl from 38 to 30 (Reduced the required monster level for this item to drop from 38 to 30)
* Felloak
 * Reduced lvl from 4 to 3 (Reduced the required monster level for this item to drop from 4 to 3)
 * Added sock to prop7 and 2 to par7 (Now spawns with 2 open sockets)
* Knell Striker
 * Reduced lvl from 7 to 5 (Reduced the required monster level for this item to drop from 7 to 5)
 * Increased min6 and max6 from 70/80 to 80/120 (Enhanced Damage range increased from 70-80 to 80-120)
* Rusthandle
 * Reduced lvl from 23 to 18 (Reduced the required monster level for this item to drop from 23 to 18)
 * Increased min2 and max2 from 3/7 to 8/18 (Increased damage added from 3-7 to 8-18)
 * Increased min7 from 1 to 3 (Now always gives +3 to Vengeance)
* Stormeye
 * Reduced lvl from 31 to 24 (Reduced the required monster level for this item to drop from 31 to 24)
 * Increased max1 from 6 to 156 (Lightning damage range is now 1-156 instead of 1-6)
 * Increased min2 and max2 from 3/5 to 44/57 (Cold damage range increased from 3-5 to 44-57)
 * Increased min4 and max4 from 80/120 to 131/131 (Enhanced damage increased from 80-120 to 131)
 * Increased min5 from 3 to 5 (Resist Lightning skill bonus increased from 3-5 to 5)
* Stoutnail
 * Reduced lvl from 7 to 4 (Reduced the required monster level for this item to drop from 7 to 4)
 * Increased min1 and max1 from 3/10 to 6/15 (Increased Attacker Takes Damage from 3-10 to 6-15)
 * Increased min3 and max3 from 7/7 to 11/13 (Increased Vitality bonus from 7 to 11-13)
 * Increased min4 and max4 from 2/2 to 5/5 (Increased Magic Damage Reduced By from 2 to 5)
* Crushflange
 * Reduced lvl from 12 to 10 (Reduced the required monster level for this item to drop from 12 to 10)
 * Increase min5 and max5 from 50/60 to 90/120 (Enhanced Damage range increased from 50-60 to 90-120)
* Bloodrise
 * Reduced lvl from 20 to 13 (Reduced the required monster level for this item to drop from 20 to 13)
 * Changed prop 6 from skill to oskill and par6 from 96 to Sacrifice (Made Sacrifice bonus an oskill for all classes)
* The Generals Tan Do Li Ga (The General’s Tan Do Li Ga)
 * Reduced lvl from 28 to 23 (Reduced the required monster level for this item to drop from 28 to 23)
 * Increased min2 and max2 from 20/20 to 24/24 (Flat damage bonus increased from 1-20 to 1-24)
 * Increased min4 and max4 from 25/25 to 50/50 (Increased Defense bonus from 25 to 50)
 * Increased min6 and max6 from 50/60 to 95/115 (Enhanced Damage bonus increased from 50-60 to 95-115)
* Ironstone
 * Reduced lvl from 36 to 29 (Reduced the required monster level for this item to drop from 36 to 29)
 * Increased min2 and max2 from 100/150 to 130/180 (Enhanced Damage bonus increased from 100-150 to 130-180)
 * Increased max5 from 10 to 20 (Increased Strength bonus from 10 to 10-20)
* Bonesob (Bonesnap)
 * Reduced lvl from 32 to 23 (Reduced the required monster level for this item to drop from 32 to 23)
* Steeldriver
 * Reduced lvl from 39 to 34 (Reduced the required monster level for this item to drop from 39 to 34)
* Blood Crescent
 * Reduced lvl from 10 to 9 (Reduced the required monster level for this item to drop from 10 to 9)
 * Increased min2 and max2 from 60/80 to 80/150 (Enhanced Damage bonus increased from 60-80 to 80-150)
* Krintizs Skewer (Skewer of Krintiz)
 * Reduced lvl from 14 to 10 (Reduced the required monster level for this item to drop from 14 to 10)
 * Increased min5 and max5 from 50/50 to 150/150 (Enhanced Damage bonus increased from 50 to 150)
* Gleamscythe
 * Reduced lvl from 18 to 15 (Reduced the required monster level for this item to drop from 18 to 15)
 * Increased min4 and max4 from 20/20 to 60/60 (Increased Attack Speed bonus increased from 20 to 60)
 * Added sock to prop7 and 1 to par7 (Now spawns with 1 open socket)
* Azurewrath (Dark Master)
 * Changed enabled from 0 to 1 (Enabled the “mini” Azurewrath from 1.09, now named Dark Master)
 * Reduced lvl from 18 to 14 (Reduced the required monster level for this item to drop from 18 to 14)
 * Changed prop1 from deadly to dmg-undead, and increased min1 and max1 from 50/50 to 200/200 (Replaced 50% Deadly Strike with 200% Damage vs Undead)
 * Increased min2 and max2 from 10/10 to 20/20 (Magic Find bonus increased from 10/10 to 20/20
 * Increased min4 and max4 from 100/100 to 100/150 (Enhanced Damage bonus increased from 100 to 100-150)
 * Increased min3 and max3 from 3/6 to 6/14 (Increased Cold Damage from 3-6 to 6-14)
 * Increased min6 and max6 from 5/10 to 15/25 (Increased Magic damage from 5-10 to 15-25)
 * Added dmg-demon to prop7, and 200/200 to min7 and max7 (Added 200% Damage vs Demons)
 * Full stats as follows:
  * Crystal Sword
  * 100-150% Enhanced Damage
  * 200% Damage to Undead
  * 200% Damage to Demons
  * 20% Magic Find
  * 6-14 Cold Damage (4 second duration)
  * 15-25 Magic Damage
  * +25 Durability (Hidden)
* Griswolds Edge (Griswold’s Edge)
 * Reduced lvl from 23 to 19 (Reduced the required monster level for this item to drop from 23 to 19)
 * Increased min4 and max4 from 10/10 to 20/20 (Increased Attack Speed bonus increased from 10 to 20)
 * Added deadly to prop8 and 50/50 to min8 and max8 (Added 50% Deadly Strike)
* Hellplague
 * Reduced lvl from 30 to 24 (Reduced the required monster level for this item to drop from 30 to 24)
 * Increased min3 and max3 from 48/48 to 96/96, and min4 and max4 from 96/96 to 144/144 (increased poison damage from 28-56 to 56-84)
 * Increased min8 and max8 from 2/2 to 3/3 (Fire Skills bonus increased from 2 to 3)
* Culwen’s Point
 * Reduced lvl from 39 to 31 (Reduced the required monster level for this item to drop from 39 to 31)
 * Increased min6 and max6 from 70/80 to 108/108 (Enhanced Damage bonus increased from 70-80 to 108)
 * Changed prop5 from att to att%, and reduced min5 and max5 from 60/60 to 20/20 (Attack Rating bonus changed from +60 to +20%)
 * Added deadly to prop7, and 20/20 to min7 and max7 (Added 20% chance of Deadly Strike)
* Shadowfang
 * Reduced lvl from 16 to 12 (Reduced the required monster level for this item to drop from 16 to 12
 * Changed prop2 from res-cold to res-all (Changed 20% Cold Resist to 20% Resist All)
 * Increased min5 and max5 from 100/100 to 125/125 (Enhanced Damage bonus increased from 100 to 125)
* Soulflay
 * Reduced lvl from 26 to 17 (Reduced the required monster level for this item to drop from 26 to 17)
 * Deleted all stats from prop1 to max2 (Removed mana and life steal)
 * Added openwounds to prop1 and 23/23 to min1 and max1 (Added 23% chance of Open Wounds)
 * Added dmg-pois to prop2, 75 to par2, and 307/307 to min2 and max2 (Added 90 poison damage over 3 seconds)
 * Increased min3 and max3 from 70/100 to 120/145 (Enhanced Damage bonus increased from 70-100 to 120/145)
* Kinemils Awl (Kinemil’s Awl)
 * Reduced lvl from 31 to 25 (Reduced the required monster level for this item to drop from 31 to 25)
 * Increased min4 and max4 from 80/100 to 100/120 (Enhanced Damage bonus increased from 80-100 to 100-120)
 * Added swing2 to prop7, and 30/30 to min7 and max7 (Added 30% Increased Attack Speed bonus)
* Blacktongue
 * Reduced lvl from 35 to 28 (Reduced the required monster level for this item to drop from 35 to 28)
 * Reduced par1 from 150 to 25 (Poison duration reduced from 6 to 1 seconds)
 * Increased min1 and max1 from 192/192 to 614/614 (Poison damage changed to 60 damage)
 * Increased min5 and max5 from 50/60 to 150/160 (Enhanced Damage bonus increased from 50-60 to 150-160)
 * Changed prop6 from *hp to hp (Enabled -10 health debuff)
* Ripsaw
 * Reduced lvl from 35 to 27 (Reduced the required monster level for this item to drop from 35 to 27)
 * Increased min4 and max4 from 80/100 to 100/200 (Enhanced Damage bonus increased from 80-100 to 100-200)
* The Patriarch
 * Reduced lvl from 39 to 33 (Reduced the required monster level for this item to drop from 39 to 33)
 * Increased min1 and max1 from 3/3 to 9/9 (Damage Reduced increased from 3 to 9)
 * Increased min2 and max2 from 3/3 to 9/9 (Magic Damage Reduced increased from 3 to 9)
 * Increased min5 and max5 from 100/120 to 200/300 (Enhanced Damage bonus increased from 100-120 to 200-300)
 * Increased min6 and max6 from 10/10 to 20/20 (Strength bonus increased from 10 to 20)
* The Diggler
 * Reduced lvl from 15 to 9 (Reduced the required monster level for this item to drop from 15 to 9)
 * Reduced lvl req from 11 to 6 (Required level to equip reduced from 11 to 6)
 * Increased min2 and max2 from 50/50 to 150/150 (Enhanced Damage bonus increased from 50 to 150)
* The Jade Tan Do
 * Reduced lvl from 26 to 17 (Reduced the required monster level for this item to drop from 26 to 17)
 * Reduced lvl req from 19 to 14 (Required level to equip reduced from 19 to 14)
 * Increased min1 and max1 from 100/150 to 200/250 (Attack Rating bonus increased from 100-150 to 200-250)
 * Increased min3 and max3 from 460 to 921 (Poison damage increased from 180 to 360)
 * Added move2 to prop6 and 40/40 to min6 and max6 (Added 40% Faster Run/Walk bonus)
* Irices Shard (Spectral Shard)
 * Reduced lvl from 34 to 23 (Reduced the required monster level for this item to drop from 34 to 23)
 * Reduced lvl req from 25 to 21 (Required level to equip reduced from 25 to 21)
 * Added fire-min and fire-max to prop5 and prop6. Added 20/20 to min5 and max5, and 40/40 to min6 and max6 (Added 20-40 fire damage)
 * Added dmg-cold to prop7, 75 to par7, and 15/25 to min7 and max7 (Added 15-25 cold damage with 3 second chill duration)
 * Added ltng-min to par8, ltng-max to par9, 1/1 to min8 and max8, and 60/60 to min9 and max9 (Added 1-60 lightning damage)
* The Dragon Chang
 * Reduced lvl from 11 to 5 (Reduced the required monster level for this item to drop from 11 to 5)
 * Reduced lvl req from 8 to 5 (Required level to equip reduced from 8 to 5)
 * Changed prop5 from dmg-fire to dmg-fire/lvl, added 16 to par5, removed 3/6 from min5/max5 (Changed fire damage from 3-6 to +2 to max fire damage per level)
* Razortine
 * Reduced lvl from 16 to 11 (Reduced the required monster level for this item to drop from 16 to 11)
 * Increased min6 and max6 from 30/50 to 80/150 (Enhanced Damage bonus increased from 30-50 to 80-150)
* Bloodthief
 * Reduced lvl from 23 to 19 (Reduced the required monster level for this item to drop from 23 to 19)
 * Increased min6 and max6 from 50/70 to 120/180 (Enhanced Damage range increased from 50-70 to 120-180)
* Lance of Yaggai
 * Reduced lvl from 30 to 24 (Reduced the required monster level for this item to drop from 30 to 24)
 * Increased min1 and max1 from 8/8 to 9/17 (Attack Takes Damage increased from 8 to 9-17)
 * Increased min3 and max3 from 60/60 to 360/360 (Increased lightning damage from 1-60 to 1-360)
* The Tannr Gorerod
 * Reduced lvl from 36 to 29 (Reduced the required monster level for this item to drop from 36 to 29)
 * Increased min8 and max8 from 80/100 to 110/190 (Enhanced damage bonus increased from 80-100 to 110-190)
* Dimoaks Hew (Dimoak’s Hew)
 * Reduced lvl from 11 to 5 (Reduced the required monster level for this item to drop from 11 to 5)
 * Reduced lvl req from 8 to 5 (Required level to equip reduced from 8 to 5)
 * Changed prop1 from dex to str (Dexterity bonus changed to Strength)
 * Decreased min4 and max4 from -8 to -18 (Defense debuff increased from -8 defense to -18)
* Steelgoad
 * Reduced lvl from 19 to 13 (Reduced the required monster level for this item to drop from 19 to 13)
 * Increased min4 and max4 from 5/5 to 6/6 (Increased Resist All bonus from 5 to 6)
 * Increased min5 and max5 from 60/80 to 160/180 (Enhanced Damage bonus increased from 60-80 to 160-180)
* Soul Harvest
 * Reduced lvl from 26 to 17 (Reduced the required monster level for this item to drop from 26 to 17)
 * Increased min4 and max4 from 50/90 to 90/150 (Enhanced Damage bonus increased from 50-90 to 90-150)
 * Changed prop5 from manasteal to mana-kill (Replaced 10% mana steal with 10 mana per kill)
 * Changed prop6 from enr to heal-kill, and increased min6 and max6 from 5/5 to 10/10 (Replaced Energy bonus with 10 life per kill)
* The Battlebranch
 * Reduced lvl from 34 to 25 (Reduced the required monster level for this item to drop from 34 to 25)
 * Increased lvl req from 25 to 29 (Required level to equip increased from 25 to 29)
 * Changed prop2 from dex to ac, and min2 and max2 from 10/10 to 100/100 (Changed Dexterity bonus to +100 armor)
 * Increased min3 and max3 from 50/70 to 220/270 (Enhanced Damage bonus increased from 50-70 to 220-270)
 * Reduced min4 and max4 from 50/100 to -100/-100 (Attack Rating bonus decreased from 50-100 to -100)
* Woestave
 * Reduced lvl from 38 to 30 (Reduced the required monster level for this item to drop from 38 to 30)
 * Increased min5 and max5 from 1/1 to 3/3 (Increased Freeze chance calculation from 1 to 3)
 * Increased min8 and max8 from 20/40 to 120/140 (Enhanced Damage bonus increased from 20-40 to 120-140)
* The Grim Reaper
 * Reduced lvl from 39 to 31 (Reduced the required monster level for this item to drop from 39 to 31)
 * Increased min4 and max4 from 20/20 to 100/100 (Enhanced Damage bonus increased from 20 to 100)
 * Changed prop6 from *hp to hp (Enabled -20 health debuff)
* Bane Ash
 * Reduced lvl from 7 to 3 (Reduced the required monster level for this item to drop from 7 to 3)
 * Increased min1 and max1 from 4/4 to 8/8, and min2 and max2 from 6/6 to 12/12 (Fire Damage bonus increased from 4-6 to 8-12)
 * Increased min7 and max7 from 5/5 to 6/6 (Fire Bolt bonus increased from 5 to 6)
 * Increased min8 and max8 from 2/2 to 3/3 (Warmth bonus increased from 2 to 3)
* Serpent Lord
 * Reduced lvl from 12 to 8 (Reduced the required monster level for this item to drop from 12 to 8)
 * Increased min1 and max1 from 40/40 to 122/122 (Poison damage increased from 12 to 36)
 * Increased min5 and max5 from 30/40 to 100/100 (Enhanced Damage bonus increased from 30-40 to 100)
* Lazarus Spire (Spire of Lazarus)
 * Reduced lvl from 24 to 20 (Reduced the required monster level for this item to drop from 24 to 20)
 * Increased min2 and max2 from 5/5 to 9/9 (Damage Reduced By increased from 5 to 9)
 * Changed prop9 from sor to allskills (+1 Sorceress Skills changed to +1 All Skills)
* The Salamander
 * Reduced lvl from 28 to 23 (Reduced the required monster level for this item to drop from 28 to 23)
 * Changed min3 and max3, min4 and max4, min5 and max5, to 1/3 (Warmth, Fire Bolt, and Fireball skill bonuses changed to vary from +1 to +3)
 * Increased min6 and max6 from 2/2 to 3/3 (Increased Fire Skills buff from +2 to +3)
* The Iron Jang Bong
 * Reduced lvl from 38 to 30 (Reduced the required monster level for this item to drop from 38 to 30)
 * Increased min1 and max1 from 30/30 to 50/130 (Increased Defense bonus from 30 to 50-130)
 * Increased min3 and max3 from 100/100 to 150/150 (Enhanced Damage bonus increased from 100 to 150)
 * Changed par5 from 48 to 52, and increased min5 and max5 from 2/2 to 4/4 (Changed +2 Nova to +4 Enchant)
 * Deleted all stats from prop6 to max7 and moved all other stats over (Removed +2 Blaze and +3 Frost Nova)
 * Added swing2 to prop7 and 50/50 to min7 and max7 (Added 50% Increased Attack Speed)
* Pluckeye
 * Reduced lvl from 10 to 3 (Reduced the required monster level for this item to drop from 10 to 3)
 * Reduced lvl req from 7 to 4 (Reduced level to equip from 7 to 4)
 * Increased min2 and max2 from 100/100 to 300/300 (Enhanced Damage bonus increased from 100 to 300)
* Witherstring
 * Reduced lvl from 18 to 6 (Reduced the required monster level for this item to drop from 18 to 6)
 * Reduced lvl req from 13 to 8 (Required level to equip reduced from 13 to 8)
 * Increased min2 and max2 from 1/1 to 6/6, and min3 and max3 from 3/3 to 9/9 (Increased bonus damage from 1-3 to 6-9)
 * Increased max6 from 50 to 60 (Enhanced Damage range increased from 40-50 to 40-60)
* Rimeraven (Raven Claw)
 * Reduced lvl from 20 to 10 (Reduced the required monster level for this item to drop from 20 to 10)
* Piercerib (Rogue’s Bow)
 * Reduced lvl from 27 to 15 (Reduced the required monster level for this item to drop from 27 to 15)
 * Reduced lvl req from 20 to 16 (Required level to equip reduced from 20 to 16)
 * Increased min2 and max2 from 30/30 to 60/60 (Increased Deadly Strike chance from 30 to 60)
 * Increased min5 and max5 from 40/60 to 70/110 (Enhanced Damage bonus increased from 40-60 to 70-110)
* Pullspite (Stormstrike)
 * Reduced lvl from 34 to 20 (Reduced the required monster level for this item to drop from 34 to 20)
 * Increased max1 from 30 to 90 (Increased max Lightning Damage from 30 to 90)
 * Changed prop2 from str to dex and increased min2 and max2 from 8/8 to 8/15 (Change Strength bonus to Dexterity and increased bonus range from 8 to 8-15)
 * Increased min6 and max6 from 70/90 to 109/109 (Enhanced Damage bonus increased from 70-90 to 109)
* Wizendraw
 * Decreased lvl from 35 to 25 (Reduced the required monster level for this item to drop from 35 to 25)
 * Changed prop2 from mana to cast2, and decreased min2 and max2 from 30/30 to 20/20 (Removed Mana bonus and added 20% Faster Cast Rate)
 * Increased min6 and max6 from 70/80 to 170/210 (Enhanced Damage bonus increased from 70-80 to 170-210)
* Hellclap
 * Reduced lvl from 36 to 30 (Reduced the required monster level for this item to drop from 36 to 30)
 * Increased min2 and max2 from 15/15 to 55/55, and min3 and max3 from 30/50 to 80/95 (Increased Fire Damage bonus from 15 to 30-50, to 55 to 80-95)
 * Increased min8 and max8 from 1/1 to 3/3 (Fire Skills bonus increased from 1 to 3)
* Blastbark
 * Reduced lvl from 38 to 33 (Reduced the required monster level for this item to drop from 38 to 33)
 * Increased min1 and max1 from 70/130 to 170/230 (Enhanced Damage bonus increased from 70-130 to 170-230)
 * Increased min2 and max2 from 5/5 to 16/16 (Strength bonus increased from 5 to 16)
 * Increased min3 and max3 from 1/1 to 2/2 (Amazon Skills bonus increased from 1 to 2)
* Leadcrow
 * Reduced lvl from 12 to 8 (Reduced the required monster level for this item to drop from 12 to 8)
 * Increased min3 and max3 from 70/70 to 130/130 (Enhanced Damage bonus increased from 70/70 to 130/130
* Ichorsting
 * Reduced lvl from 24 to 17 (Reduced the required monster level for this item to drop from 24 to 17)
 * Increased min1 and max1 from 102/102 to 412/412 (Poison Damage increased from 30 to 121)
 * Increased min5 and max5 from 50/50 to 75/75 (Enhanced Damage bonus increased from 50 to 75)
* Hellcast
 * Reduced lvl from 36 to 26 (Reduced the required monster level for this item to drop from 36 to 26)
 * Increased min6 and max6 from 70/80 to 120/175 (Enhanced Damage bonus increased from 70-80 to 120-175)
 * Increased min7 and max7 from 15/35 to 66/122 (Fire Damage bonus increased from 15-35 to 66-122)
* Doomspittle (Doomslinger)
 * Reduced lvl from 38 to 35 (Reduced the required monster level for this item to drop from 38 to 35)
 * Increased min2 and max2 from 35/35 to 60/60 (Pierce chance increased from 35 to 60)
 * Increased min5 and max5 from 60/100 to 200/260 (Enhanced Damage bonus increased from 60-100 to 200-260)
* Coif of Glory
 * Reduced lvl from 19 to 15 (Reduced the required monster level for this item to drop from 19 to 15)
 * Increased min1 and max1 from 7/7 to 14/14 (Attacker Takes Lightning Damage increased from 7 to 14)
 * Increased min3 and max3 from 15/15 to 25/25 (Lightning Resist increased from 15 to 25)
* Duskdeep
 * Reduced lvl from 23 to 17 (Reduced the required monster level for this item to drop from 23 to 17)
 * Wormskull
 * Reduced lvl from 28 to 24 (Reduced the required monster level for this item to drop from 28 to 24)
 * Reduced par5 from 200 to 100, and increased min5 and max5 from 102/102 to 204/204 (Halved duration of poison damage while keeping the total damage the same)
* Howltusk
 * Reduced lvl from 34 to 26 (Reduced the required monster level for this item to drop from 34 to 26)
 * Increased min1 and max1 from 2/2 to 7/7 (Magic Damage Reduced By increased from 2 to 7)
 * Increased min2 and max2 from 3/3 to 23/23 (Attacker Takes Damage increased from 3 to 23)
* Undead Crown
 * Reduced lvl from 39 to 31 (Reduced the required monster level for this item to drop from 39 to 31)
 * Increased min6 and max6 from 50/50 to 250/250 (Damage vs Undead increased from 50 to 250)
 * Increased min7 and max7 from 50/100 to 200/250 (Attack Rating vs Undead increased from 50-100 to 200-250)
* The Face of Horror
 * Reduced lvl from 27 to 21
 * Changed prop4 from dmg-undead to dmg-demon and increased min4 and max4 from 50/50 to 150/200
* Greyform
 * Reduced lvl from 10 to 3 (Reduced the required monster level for this item to drop from 10 to 3)
 * Reduced lvl req from 7 to 4 (Required level to equip reduced from 7 to 4)
 * Added red-dmg to prop7 and 3/3 to min7 and max7 (Added Damage Reduced By 3)
* Blinkbats Form (Blinkbat’s Form)
 * Reduced lvl from 16 to 5 (Reduced the required monster level for this item to drop from 16 to 5)
 * Reduced lvl req from 12 to 8 (Required level to equip reduced from 12 to 8)
 * Increased min2 and max2 from 10/10 to 25/25 (Faster Run/Walk bonus increased from 10 to 25)
 * Changed prop3 from ac to ac% and increased min3 and max3 from 25/25 to 125/125 (Changed +25 Defense to 125% Enhanced Defense)
 * Increased min4 and max4 from 3/3 to 5/5, increased min5 and max5 from 6/6 to 9/9 (Fire damage bonus increased from 3-6 to 5-9)
* The Centurion
 * Reduced lvl from 19 to 7 (Reduced the required monster level for this item to drop from 19 to 7)
 * Reduced lvl req from 14 to 8 (Required level to equip reduced from 14 to 8)
 * Changed prop1 from ac to ac% and increased min1 and max1 from 30/30 to 175/200 (Replaced +30 Defense with 175-200% Enhanced Defense)
 * Increased min3 and max3 from 2/2 to 6/6 (Damage Reduced By increased from 2 to 6)
 * Increased min7 and max7 from 5/5 to 10/10 (Replenish Life increased from 5 to 10)
* Twitchthroe
 * Reduced lvl from 22 to 11 (Reduced the required monster level for this item to drop from 22 to 11)
 * Reduced lvl req from 16 to 10 (Level required to equip reduced from 16 to 10)
 * Increased min1 and max1 from 20/20 to 25/25 (Increased Attack Speed bonus increased from 20 to 25)
 * Increased min6 and max6 from 20/20 to 25/25 (Faster Hit Recovery bonus increased from 20 to 25)
* Darkglow
 * Reduced lvl from 19 to 13 (Reduced the required monster level for this item to drop from 19 to 13)
 * Increased min5 and max5 from 10/10 to 25/25 (Resist All bonus increased from 10 to 25)
* Hawkmail
 * Reduced lvl from 20 to 15 (Reduced the required monster level for this item to drop from 20 to 15)
 * Increased min1 and max1 from 80/100 to 100/120 (Enhanced Defense bonus increased from 80-100 to 100-120)
 * Increased min2 and max2 from 15/15 to 20/20 (Maximum Cold Resist bonus increased from 15 to 20)
 * Increased min3 and max3 from 15/15 to 75/75 (Cold Resist bonus increased from 15 to 75)
* Sparkling Mail
 * Reduced lvl from 23 to 15 (Reduced the required monster level for this item to drop from 23 to 15)
 * Increased min1 and max1 from 75/85 to 125/145 (Enhanced Defense bonus increased from 75-85 to 125-145)
 * Increased max2 from 20 to 46 (Lightning Damage bonus increased from 1-20 to 1-46)
 * Increased min3 and max3 from 10/14 to 20/28 (Attacker Takes Lightning Damage increased from 10-14 to 20-28)
 * Increased min4 and max4 from 30/30 to 45/45 (Lightning Resist increased from 30 to 45)
* Venomsward (Venom Ward)
 * Reduced lvl from 27 to 22 (Reduced the required monster level for this item to drop from 27 to 22)
* Iceblink
 * Reduced lvl from 30 to 24 (Reduced the required monster level for this item to drop from 30 to 24)
 * Increased min1 and max1 from 1/1 to 3/3 (Increased freeze chance calculation from 1 to 3)
 * Increased min4 and max4 from 1/1 to 4/6 (Magic Damage Reduced increased from 1 to 4-6)
* Boneflesh
 * Reduced lvl from 35 to 25 (Reduced the required monster level for this item to drop from 35 to 25)
 * Increased max1 from 5 to 8 (Increased life steal from 5 to 5-8)
 * Increased min2 and max2 from 100/120 to 150/170 (Enhanced Defense bonus increased from 100-120 to 150-170)
 * Increased min3 and max3 from 35/35 to 75/85 (Attack Rating bonus increased from 35 to 75-85)
* Rockflesh (Rockfleece)
 * Reduced lvl from 38 to 30 (Reduced the required monster level for this item to drop from 38 to 30)
 * Increased min2 and max2 from 100/130 to 130/200 (Enhanced Defense bonus increased from 100-130 to 130-200)
 * Increased min4 and max4 from 5/5 to 11/11 (Damage Reduced By increased from 5 to 11)
* Rattlecage
 * Reduced lvl from 39 to 34 (Reduced the required monster level for this item to drop from 39 to 34)
 * Changed prop1 from howl to dmg%, and increased min1 and max1 from 52/52 to 75/100 (Replaced Hit Causes Monster to Flee with 75-100% Enhanced Damage)
* Goldskin
 * Increased min3 and max3 from 10/10 to 36/36 (Attacker Takes Damage increased from 10 to 36)
 * Added mag% to prop7, and added 50/50 to min7 and max7 (Added 50% Magic Find)
* Heavenly Garb
 * Increased min2 and max2 from 10/10 to 23/23 (Resist All bonus increased from 10 to 23)
 * Increased min3 and max3 from 25/25 to 60/60 (Regenerate Mana bonus increased from 25 to 60)
 * Deleted all data from prop5 through max6 (Removed bonuses vs undead)
 * Added cast2 to prop5, and 20/20 to min5 and max5 (Added 20% Faster Cast Rate)
* Umbral Disk
 * Reduced lvl from 12 to 6 (Reduced the required monster level for this item to drop from 12 to 6)
 * Reduced lvl req from 9 to 5 (Required level to equip reduced from 9 to 5)
 * Increased min4 and max4 from 20/20 to 25/25 (Life bonus increased from 20 to 25)
* Stormguild
 * Reduced lvl from 18 to 13 (Reduced the required monster level for this item to drop from 18 to 13)
 * Increased min1 and max1 from 1/1 to 4/4 (Magic Damage Reduced By increased from 1 to 4)
 * Increased max4 from 6 to 26 (Lightning Damage bonus increased from 1-6 to 1-26)
 * Increased min7 and max7 from 3 to 18 (Attacker Takes Lightning Damage increased from 3 to 18)
* Wall of the Eyeless
 * Reduced lvl from 27 to 21 (Reduced the required monster level for this item to drop from 27 to 21)
 * Increased min3 and max3 from 20/20 to 25/35 (Faster Cast Rate increased from 20 to 25-35)
* Swordback Hold
 * Reduced lvl from 20 to 16 (Reduced the required monster level for this item to drop from 20 to 16)
 * Increased lvl req from 15 to 35 (Required level to equip increased from 15 to 35)
 * Increased min1 and max1 from 5/5 to 57/57. Deleted all stats from prop6 to max6 and moved other stats over. (Attacker Takes Damage increased from 10 to 57. Removed second instead of Attack Takes Damage)
 * Added dmg-min to prop7, added 21/21 to min7 and max7. Added dmg-max to prop8, added 36/36 to min8 and max8 (Added 21-36 damage)
* Steelclash
 * Reduced lvl from 23 to 18 (Reduced the required monster level for this item to drop from 23 to 18)
 * Increased min3 and max3 from 3/3 to 4/7 (Damage Reduced By bonus increased from 3 to 4-7)
 * Increased min7 and max7 from 15/15 to 35/35 (Resist All increased from 15 to 35)
* Bverrit Keep
 * Increased min1 and max1 from 30/30 to 50/60 (Increased Defense bonus from 30 to 50-60)
 * Increased min3 and max3 from 5/5 to 15/15 (Increased Strength bonus from 5 to 15)
 * Increased min4 and max4 from 5/5 to 9/9 (Magic Damage Reduced By increased from 5 to 9)
 * Increased min6 and max6 from 10/10 to 20/20 (Block Chance bonus increased from 10 to 20)
* The Ward
 * Reduced lvl from 35 to 30 (Reduced the required monster level for this item to drop from 35 to 30)
 * Increased min2 and max2 from 2/2 to 12/12 (Magic Damage Reduced By increased from 2 to 12)
 * Increased min7 and max7 from 2 to 12 (Physical Damage reduction increased from 0 to 10, +2% from being a medium heavy shield from the base DMMod)
* The Hand of Broc
 * Reduced lvl from 7 to 3 (Reduced the required monster level for this item to drop from 7 to 3)
 * Reduced lvl req from 5 to 4 (Required level to equip reduced from 5 to 4)
 * Increased max1 from 3 to 5 (Increased mana steal range from 3 to 3-5)
 * Increased max2 from 3 to 5 (Increased life steal range from 3 to 3-5)
 * Increased min6 and max6 from 10/20 to 30/50 (Enhanced Defense bonus increased from 10-20 to 30-50)
* Chance Guards
 * Reduced lvl from 20 to 16 (Reduced the required monster level for this item to drop from 20 to 16)
 * Increased min6 and max6 from 20/30 to 40/60 (Enhanced Defense bonus increased from 20-30 to 40-60)
* Magefist
 * Reduced lvl from 31 to 22 (Reduced the required monster level for this item to drop from 31 to 22)
* Frostburn
 * Reduced lvl from 39 to 30 (Reduced the required monster level for this item to drop from 39 to 30)
 * Increased par4 from 50 to 100 (Increased cold damage duration from 2 to 4 seconds)
 * Increased min4 and max4 from 1/6 to 13/26 (Increased cold damage from 1-6 to 13-26)
 * Increased min5 and max5 from 10/20 to 50/70 (Enhanced Defense bonus increased from 10-20 to 50-70)
* Hotspur
 * Reduced lvl from 7 to 3 (Reduced the required monster level for this item to drop from 7 to 3)
 * Reduced lvl req from 5 to 4 (Required level to equip reduced from 5 to 4)
 * Increased min6 and max6 from 10/20 to 20/30 (Enhanced Defense bonus increased from 10-20 to 20-30)
* Gorefoot
 * Reduced lvl from 12 to 8 (Reduced the required monster level for this item to drop from 12 to 8)
 * Increased min3 and max3 from 2/2 to 4/4 (Mana steal increased from 2 to 4)
 * Increased min4 and max4 from 2/2 to 6/6 (Attacker Takes Damage increased from 2 to 6)
 * Increased min6 and max6 from 20/30 to 50/80 (Enhanced Defense bonus increased from 20-30 to 50-80)
 * Increased min7 and max7 from 2/2 to 3/3 (Leap skill bonus increased from 2 to 3)
* Treads of Cthon
 * Reduced lvl from 20 to 14 (Reduced the required monster level for this item to drop from 20 to 14)
 * Increased min1 and max1 from 30/30 to 50/50 (Faster Run/Walk bonus increased from 30 to 50)
* Goblin Toe
 * Reduced lvl from 30 to 23 (Reduced the required monster level for this item to drop from 30 to 23)
 * Increased min2 and max2 from 1/1 to 3/3 (Damage Reduced By increased from 1 to 3)
 * Increased min3 and max3 from 1/1 to 3/3 (Magic Damage Reduced By increased from 1 to 3)
* Tearhaunch
 * Reduced lvl from 39 to 30 (Reduced the required monster level for this item to drop from 39 to 30)
 * Increased min2 and max2 from 5/5 to 10/10 (Strength bonus increased from 5 to 10)
 * Increased min3 and max3 from 5/5 to 10/10 (Dexterity bonus increased from 5 to 10)
 * Increased min5 and max5 from 10/10 to 15/20 (Resist All bonus increased from 10 to 15-20)
* Lenyms Cord (Lenymo)
 * Reduced lvl from 10 to 3 (Reduced the required monster level for this item to drop from 10 to 3)
 * Reduced lvl req from 7 to 4 (Required level to equip reduced from 7 to 4)
 * Increased min2 and max2 from 30/30 to 45/45 (Mana Regeneration bonus increased from 30 to 45)
 * Increased min3 and max3 from 5/5 to 10/10 (Resist All bonus increased from 5 to 10)
* Snakecord
 * Decreased lvl from 16 to 11 (Reduced the required monster level for this item to drop from 16 to 11)
 * Increased min1 and max1 from 40/40 to 112/112 (Increased poison damage from 12 to 33)
 * Increased min5 and max5 from 5/5 to 8/8 (Replenish Life increased from 5 to 8)
* Nightsmoke
 * Reduced lvl from 27 to 14 (Reduced the required monster level for this item to drop from 27 to 14)
 * Reduced lvl req from 20 to 18 (Required level to equip reduced from 20 to 18)
 * Increased min1 and max1 from 10 to 15 (Resist All increased from 10 to 15)
 * Increased min4 and max4 from 2 to 3 (Damage Reduced By increased from 2 to 3)
* Goldwrap
 * Reduced lvl from 36 to 24 (Reduced the required monster level for this item to drop from 36 to 24)
* Bladebuckle
 * Reduced lvl from 39 to 30 (Reduced the required monster level for this item to drop from 39 to 30)
 * Increased min1 and max1 from 8 to 16 (Attacker Takes Damage increased from 8 to 16)
 * Increased max3 from 3 to 5 (Damage Reduced By range increased from 3 to 3-5)
 * Changed prop4 from str to dmg%, and increased min4 and max4 from 5/5 to 30/50 (Replaced Strength bonus with 30-50% Enhanced Damage)
* Grim’s Burning Dead
 * Increased min6 and max6 from 3/3 to 5/5 (Necromancer skills bonus increased from 3 to 5)
 * Deleted all data from prop10 to max10 and moved all other stats over (Removed +1 Fire Skills, from the base DMMod)

#### data\local\lng\item-names.json

* Appended "Dark Master" to the end of the file with id 51500, for the unique Crystal Sword.



###### Regular DMMod patch notes

**Patch 1.03b Changelog** (12-31-23)
  * quick patch mostly to properly fix a critical bug that I attempted to hotfix earlier this morning but failed (all runewords were poofing due to the new Akara Potion Upgrade not having anything in the "code" column)

  * data>global>excel
    * misc.txt
      * Minor Mana Potion
        * changed "AkaraMin" and "AkaraMax" to 1/1 from blank (Akara sells mana potions again)
      * deleted Akara Potion Upgrade entry (I can't currently figure out how to remove minor mana potions from Normal Akara while having Nightmare and Hell Akara still sell greater mana potions so I'll just abort this change for now)
    * uniques.txt
      * The Rising Sun
        * decreased "min7" to 4 from 10 (enemy fire resistance decreased to -4-10% from -10%)

**Patch 1.03 Changelog** (12-30-23)
  * Happy Holidays and also Happy New Year!
  * even more fixing of typos and clarification/rephrasing of changes

  * data>global>excel
    * armor.txt
      * set "ShowLevel" to 1 for all armor (displays item level in parenthesis, was accidently reverted before DMMod 1.00 launched)

    * misc.txt
      * set "ShowLevel" to 1 for Amulet, Ring, Small Charm, Large Charm, Grand Charm, and Jewel (displays item level in parenthesis)
      * ~~Minor Mana Potion~~ (see patch 1.03b)
        * ~~changed "AkaraMin" and "AkaraMax" to blank from 1/1 (Akara no longer sells minor mana potions in Normal)~~
      * ~~Akara Potion Upgrade~~ (see patch 1.03b)
        * ~~created new entry for "Akara Potion Upgrade" (cloned row 86)~~
        * ~~changed code to blank from mp1 (prevents minor mana potion graphic from appearing in Akara's vendor menu)~~ (see patch 1.03b)~~
        * ~~set "invwidth" and "invheight" to 0/0 (prevents the now invisible minor mana potion from having a tile/"clickbox" in her vendor menu)~~

    * runes.txt
      * Ancient's Pledge
        * decreased "T1Min2" and "T1Max2" to 4/4 from 13/13 (all resistances decreased to 4% to 13% [added to rune bonus])
        * decreased "T1Min3" and "T1Max3" to 20/20 from 50/50 (enhanced defense decreased to 20% from 50%)
      * Insight
        * decreased "T1Min1" and "T1Max1" to 42/77 from 90/120 (enhanced damage decreased to 42-77% from 90-120%)
        * deleted all stats from "T1Code3" through "T1Max4" and moved the other stats over (removed 23% magic find and level 1-3 Critical Strike oskill)
        * decreased new "T1Min3" and "T1Max3" to 10/10 from 35/35 (faster cast rate decreased to 10% from 35%)
      * Lore
        * deleted all stats from "T1Code1" through "T1Max1" and moved the other stats over (removed 10 energy)
        * deleted all stats from new "T1Code3" through "T1Max3" (removed 2 mana after each kill)
        * added move1 to "T1Code3, set "T1Min3" and "T1Max3" to -20/-20 (-20% faster run/walk)
      * Stealth
        * decreased "T1Min3" and "T1Max3" to 8/8 from 10/10 (faster run/walk decreased to 8% from 10%)
        * deleted all stats from "T1Code4" through "T1Max4" (removed 10% faster cast rate)
        * added light to "T1Code4", set "T1Min4" and "T1Max4" to -3/-3 (-3 light radius)
      * Valor
        * changed "*RunesUsed" to NefIth, changed "Rune1" to r04 from r07 (first rune is Nef rune instead of Tal rune [this breaks existing Valors, you'll have to make new ones. Sorry.])
        * increased "T1Min1" and "T1Max1" to 2/2 from 1/1 (damage reduced increased to 2 from 1)
        * deleted all stats from "T1Code3" through "T1Max3" and moved the other stat over (removed 10% faster run/walk)
        * changed new "T1Code3" to all-stats from swing2, decreased "T1Min3" and "T1Max3" to 3/3 from 10/10 (3 to all attributes instead of 10% increased attack speed)
      * Hustle (armor)
        * decreased "T1Min1" and "T1Max1" to 23/23 from 33/33 (faster run/walk decreased to 23% from 33%)
        * decreased "T1Min3" and "T1Max3" to 20/20 from 25/25 (increased attack speed decreased to 20% from 25%)
        * deleted all stats from "T1Code4" through "T1Max4" and moved the other stat over (removed all resistances 10%)
        * decreased new "T1Min4" and "T1Max4" to 1/1 from 2/2 (Evade oskill level decreased to 1 from 2)
      * Hustle (weapon)
        * decreased "T1Min1" and "T1Max1" to 12/12 from 15/15 (faster run/walk decreased to 12% from 15%)
        * decreased "T1Min2" and "T1Max2" to 60/85 from 95/110 (enhanced damage decreased to 60-85% from 95-110%)

    * skilldesc.txt
      * firegolem
        * changed "desccalca2" to sklvl('Holy Fire'.ln56.edmn)*(100+skill('Corpse Explosion'.blvl)*par7)/100 from sklvl('Holy Fire'.ln56.edmn) (Corpse Explosion synergy added to the Holy Fire minimum fire damage tooltip calculation)
        * changed "desccalcb2" to sklvl('Holy Fire'.ln56.edmx)* ((100+sklvl('Holy Fire'.ln56.par6))/100) * (100+skill('Corpse Explosion'.blvl) * par7)/100 from sklvl('Holy Fire'.ln56.edmx)*((100+sklvl('Holy Fire'.ln56.par6))/100) (Corpse Explosion synergy added to the Holy Fire maximum fire damage tooltip calculation)
        * changed "desccalca3" to (edmn-10)+sklvl('Holy Fire'.ln56.edmn)*sklvl('Holy Fire'.ln56.par5) from edmn+sklvl('Holy Fire'.ln56.edmn)*sklvl('Holy Fire'.ln56.par5) (fire damage tooltip is slightly more accurate, originally it adds the Fire Golem's innate physical damage [10 minimum in Normal difficulty] which causes slight inaccuracies)
        * changed "desccalcb3" to (edmx-27)+sklvl('Holy Fire'.ln56.edmx)*sklvl('Holy Fire'.ln56.par5) from edmx+sklvl('Holy Fire'.ln56.edmx)*sklvl('Holy Fire'.ln56.par5) (fire damage tooltip is slightly more accurate, originally it adds the Fire Golem's innate physical damage [27 maximum in Normal difficulty] which causes slight inaccuracies)
        * NOTE: Fire damage tooltip does not take the Corpse Explosion synergy into account, I will fix this in a future patch after I figure out the correct calculation.
        * set "dsc3line7" to 76, set "dsc3texta7" to Firedplev, set "dsc3textb7" to skillname74, set "dsccalca7" to par7 (added Corpse Explosion synergy to the tooltip)

    * skills.txt
      * Clay Golem
        * increased "Param8" to 35 from 20 (attack rating per level and synergy to other golems increased to 35 from 20)
      * BloodGolem (Blood Golem)
        * increased "Param8" to 9 from 5 (maximum life per level synergy to other golems increased to 9% from 5%)
      * IronGolem (Iron Golem)
        * increased "Param8" to 60 from 35 (defense per level and synergy to other golems increased to 60 from 35)
      * FireGolem (Fire Golem)
        * added passive_fire_mastery to "passivestat5", set "passivecalc5" to skill('Corpse Explosion'.blvl)*par7 (Corpse Explosion gives 5% fire skill damage per hard point [increases all of Fire Golem's fire damage by 5% per hard point, Holy Fire attack damage increased twice])
        * changed "sumsk1calc" to "min(ln56,45)" from "min(ln56,30)" (maximum Holy Fire level increased to 45 from 30)
        * decreased "lvlmana" to 6 from 8 (mana cost increase per level decreased to 6 from 8)
        * increased "Param8" to 11 from 6 (enhanced damage per level synergy to other golems increased to 11% from 6%)
        * set "Param7" to 5, set "*Param7 Description" to Damage synergy (5% fire skill damage synergy)
        * increased "EMinLev1" through "EMinLev5" to 11/13/16/20/27 from 9/10/11/12/13 (minimum fire damage per level increased to 11 from 9 at level 1-8, 13 from 10 at level 9-16, 16 from 11 at level 17-22, 20 from 12 at level 23-28, and 27 from 13 at level 29+)
        * increased "EMaxLev1" through "EMaxLev5" to 12/14/17/21/29 from 10/11/12/13/14 (maximum fire damage per level increased to 12 from 10 at level 1-8, 14 from 11 at level 9-16, 17 from 12 at level 17-22, 21 from 13 at level 23-28, and 29 from 13 at level 29+)
      * Holy Fire
        * increased "Param7" to 13 from 10 (Salvation damage synergy increased to 13% per level from 10%)
        * decreased "Param8" to 18 from 21 (Resist Fire damage synergy decreased to 18% per level from 21%)
      * Meditation
        * changed "aurastatcalc1" to ln34/3 from ln34 (regenerate mana decreased to 1/3 effectiveness for allies)
        * set "passivestat1" to manarecoverybonus, set "passivecalc1" to ln34 (regenerate mana remains at full effectiveness for the aurawielder)
        * decreased "Param3" to 100 from 300 (regenerate mana baseline decreased to 100% from 300%)
        * increased "Param4" to 35 from 25 (regenerate mana per level increased to 35% from 25%)

    * weapons.txt
      * set "ShowLevel" to 1 for all weapons (displays item level in parenthesis)
      * increased "StrBonus" and "DexBonus" of all amazon javelins to 95/65 from 80/60 (amazon javelins gain 0.95/0.65% enhanced damage per strength/dexterity)

  * data>hd>global>excel
    * desecratedzones.json
      * increased "terror_duration_min" to 30 from 25 (Terror Zones change every 30 minutes instead of 25 minutes)

  * data>local>lng>strings
    * skills.json
      * updated Lycanthropy tooltip for patch 1.02 changes

**Patch 1.02 Changelog (12-15-23)**
  * more fixing of typos and clarification/rephrasing of changes
  * Holy Shield visual fixed (with some caveats, original shield no longer disappears so clipping may occur and also a bug where the HS graphic doesn't disappear when you unequip your shield), legacy graphics is "buggy" (floating, not swaying with movement or blocking, etc.) because it's now an overlay instead of part of the paladin's animations but it's "good enough" for now

  * data>global>excel
    * overlay.txt
      * holyshieldoverlay (part of a fix for Holy Shield visual to appear again)
        * added new entry for "holyshieldoverlay" (cloned row 5)
        * set "*ID" to 294
        * added holyshieldoverlay to "Filename"

    * skilldesc.txt
      * shape shifting
        * changed "desctexta3" to StrSkillLycanthropyWerewolfVelocity from StrSkill89, changed "desccalca3" to (skill('Shape Shifting'.blvl) < 1) ? 1 : skill('Shape Shifting'.blvl)*3/2 from ln56 (updated tooltip for 1.02 Lycanthropy changes)
        * set "descline4" to 74, set "desctexta4" to StrSkillLycanthropyWerebearCrushingBlow, set "desccalca4" to (skill('Shape Shifting'.blvl) < 1) ? 1 : skill('Shape Shifting'.blvl) (added Werebear crushing blow bonus to the tooltip)
        * NOTE: There's an issue with using blvl in skilldesc.txt calcs, the ingame tooltip won't calculate the "next level" stats properly. This is only a tooltip bug, the stats will increase as expected.

    * skills.txt
      * Bash
        * increased "Param2" to 10 from 8 (enhanced damage per level increased to 10% from 8%)
        * changed "ToHitCalc" to 13+lvl* 7+skill('Concentrate'.blvl) * par7 from 15+lvl*7+skill('Concentrate'.blvl) * par7 (attack rating baseline decreased to 20% from 22%)
      * Skeleton Mastery
        * increased "Param4" to 15 from 10 (Revive damage per level increased to 15% from 10%)
      * Wearwolf (Werewolf)
        * changed "aurastatcalc5" to skill('Shape Shifting'.blvl)*3/2 from skill('Shape Shifting'.ln56) (Lycanthropy increases Werewolf velocity by 1.5% per hard point instead of 2% per level)
      * Shape Shifting (Lycanthropy)
        * deleted all stats from "Param5" to "*Param6 Description" (removed velocity parameters)
      * Wearbear (Werebear)
        * changed "aurastat5" to item_crushingblow from velocitypercent, changed "aurastatcalc5" to skill('Shape Shifting'.blvl) from skill('Shape Shifting'.ln56) (Lycanthropy gives Werebear 1% crushing blow per hard point instead of velocity)

    * states.txt
      * holyshieldclone
        * added holyshieldoverlay to "overlay1" (see overlay.txt)

  * data>global>overlays
    * holyshieldoverlay.dcc (cloned and renamed from pashhshnu1hs.dcc) (part of a fix for Holy Shield visual to appear again in legacy graphics)

  * data>hd>overlays>paladin
    * holyshieldoverlay.json (part of a fix for Holy Shield visual to appear again)

  * data>local>lng>strings
    * skills.json
      * added new entry for "id" 52002 (StrSkillLycanthropyWerewolfVelocity)
      * added new entry for "id" 52003 (StrSkillLycanthropyWerebearCrushingBlow)

**Patch 1.01 Changelog (12-4-23)**
  * removed DMMod Changes.txt (obsoleted by this README)
  * fixed some typos and clarified/rephrased some changes

  * data>global>excel
    * armor.txt
      * increased "durability" of normal/exceptional/elite armor by 33/75/125% (decimals 0.0-0.4 rounded down, 0.5+ rounded up) (does not apply retroactively to any armor found during DMMod 1.00, you'll need to find newly dropped armor to have the increased durability)

    * runes.txt
      * Leaf
        * decreased "T1Min1" and "T1Max1" to 2/2 from 3/3 (fire skills decreased to 2 from 3)
        * decreased "T1Min3" and "T1Max3" to 12/12 from 33/33 (cold resist decreased to 12% from 33%)
        * decreased "T1Min4" and "T1Max4" to 1/1 from 3/3 (Inferno level decreased to 1 from 3)
        * decreased "T1Min5" and "T1Max5" to 1/1 from 3/3 (Fire Bolt level decreased to 1 from 3)
        * decreased "T1Min6" and "T1Max6" to 1/1 from 3/3 (Warmth level decreased to 1 from 3)
      * Splendor
        * changed "*RunesUsed" back to EthLum from EthDol
        * changed "Rune2" back to r17 from r14 (changed second rune back to Lum from Dol)

    * skilldesc.txt
      * conversion
        * copied and deleted all stats from "dsc2line2" through "dsc2calcb2" and pasted them to "descline2" through "descalcb2" (moved duration location on the tooltip)
        * changed "desccalca2" to par1+skill('Conversion'.blvl)*par2 from ln12
        * NOTE: There's an issue with using blvl in skilldesc.txt calcs, the ingame tooltip won't calculate the "next level" stats properly. This is only a tooltip bug, the stats will increase as expected.

    * skills.txt
      * buff-type offensive and defensive aura radius baseline increased by 37.5% ("Param1" increased to 22 from 16 [Fanaticism "Param1" increased to 15 from 11])
      * Revive
        * decreased "Param3" to 4200 from 4250 (combined with "Param4" change the base duration remains 4500 frames/180 seconds)
        * increased "Param4" to 300 from 250 (Revive duration increased to 300 frames/12 seconds per hard point from 250 frames/10 seconds per hard point)
      * Thorns
        * decreased "perdelay" to 5 from 50 (Thorns updates every 5 frames/0.2 seconds instead of every 50 frames/2 seconds, should reduce the chance of nuking yourself by attacking a monster that unconverts with Thorns active)
      * Conversion
        * changed "auralencalc" to par1+skill('Conversion'.blvl)*par2 from ln12 (Conversion duration increases by 20 frames/0.8 seconds per hard point)
        * decreased "Param1" to 380 from 400 (combined with "Param2" change the base duration remains 16 seconds)
        * increased "Param2" to 20 from 0 (Conversion duration increases by 20 frames/0.8 seconds per hard point)

**1.00 Changelog (11-27-23)**

[data>global>excel](https://github.com/DarkMasterMan0/DMMod#dataglobalexcel)

* [armor.txt](https://github.com/DarkMasterMan0/DMMod#armortxt)

* [automagic.txt](https://github.com/DarkMasterMan0/DMMod#automagictxt)

* [hireling.txt](https://github.com/DarkMasterMan0/DMMod#hirelingtxt)

* [itemstatcost.txt](https://github.com/DarkMasterMan0/DMMod#itemstatcosttxt)

* [magicprefix.txt](https://github.com/DarkMasterMan0/DMMod#magicprefixtxt)

* [magicsuffix.txt](https://github.com/DarkMasterMan0/DMMod#magicsuffixtxt)

* [misc.txt](https://github.com/DarkMasterMan0/DMMod#misctxt)

* [missiles.txt](https://github.com/DarkMasterMan0/DMMod#missilestxt)

* [monprop.txt](https://github.com/DarkMasterMan0/DMMod#monproptxt)

* [monstats.txt](https://github.com/DarkMasterMan0/DMMod#monstatstxt)

* [properties.txt](https://github.com/DarkMasterMan0/DMMod#propertiestxt)

* [runes.txt](https://github.com/DarkMasterMan0/DMMod#runestxt)

* [setitems.txt](https://github.com/DarkMasterMan0/DMMod#setitemstxt)

* [sets.txt](https://github.com/DarkMasterMan0/DMMod#setstxt)

* [skilldesc.txt](https://github.com/DarkMasterMan0/DMMod#skilldesctxt)

* [skills.txt](https://github.com/DarkMasterMan0/DMMod#skillstxt)

* [states.txt](https://github.com/DarkMasterMan0/DMMod#statestxt)

* [treasureclassex.txt](https://github.com/DarkMasterMan0/DMMod#treasureclassextxt)

* [uniqueitems.txt](https://github.com/DarkMasterMan0/DMMod#uniqueitemstxt)

* [weapons.txt](https://github.com/DarkMasterMan0/DMMod#weaponstxt)

[data>global>monsters](https://github.com/DarkMasterMan0/DMMod#dataglobalmonsters)

[data>global>animdata.d2](https://github.com/DarkMasterMan0/DMMod#dataglobalanimdatad2)

[data>hd>character](https://github.com/DarkMasterMan0/DMMod#datahdcharacter)

* [monsters.json](https://github.com/DarkMasterMan0/DMMod#monstersjson)

[data>hd>global>ui>logoanimation](https://github.com/DarkMasterMan0/DMMod#datahdglobaluilogoanimation)

[data>hd>global>ui>spells>hireables](https://github.com/DarkMasterMan0/DMMod#datahdglobaluispellshireables)

[data>hd>global>excel](https://github.com/DarkMasterMan0/DMMod#datahdglobalexcel)

* [desecratedzones.json](https://github.com/DarkMasterMan0/DMMod#desecratedzonesjson)

[data>hd>global>video](https://github.com/DarkMasterMan0/DMMod#datahdglobalvideo)

[data>local>lng>strings](https://github.com/DarkMasterMan0/DMMod#datalocallngstrings)

* [item-modifiers.json](https://github.com/DarkMasterMan0/DMMod#item-modifiersjson)

* [item-names.json](https://github.com/DarkMasterMan0/DMMod#item-namesjson)

* [skills.json](https://github.com/DarkMasterMan0/DMMod#skillsjson)

### data>global>excel
#### armor.txt
  * set "ShowLevel" to 1 (displays item level)
  * added "Medium Armor" and "Heavy Armor" affix groups to "auto prefix" column (see automagic.txt) for medium and heavy armor/shields respectively

  * normal and exceptional paladin shields
    * decreased "gemsockets" to 3 from 4 (max sockets decreased to 3 from 4)

#### automagic.txt
  * Shimmering
    * changed "frequency" to 12 from 8 (chance to select a specific affix is the frequency divided by the sum of frequences in that affix group, so would be 12/30)

  * Rainbow
    * increased "mod1min" to 11 from 8 (all resistances increased to 11-15% from 8-15%)
    * changed "frequency" to 10 from 7

  * Scintillating
    * decreased "mod1max" to 25 from 30 (all resistances decreased to 16-25% from 16-30%)
    * changed "frequency" to 8 from 6

  * Prismatic
    * changed "spawnable" to blank from 1 (paladin shields can no longer roll this affix)

  * Chromatic
    * changed "spawnable" to blank from 1

  * Medium Armor
    * added new entry for "Medium Armor" (cloned row 34)
    * set "levelreq" to 1
    * set "group" to 500
    * set "mod1code1" to red-dmg%, set "mod1min" and "mod1max" to 2/2 (2% physical damage reduction)

  * Heavy Armor
    * added new entry for "Heavy Armor" (cloned row 34)
    * set "levelreq" to 1
    * set "group" to 501
    * set "mod1code1" to red-dmg%, set "mod1min" and "mod1max" to 5/5 (5% PDR)

#### hireling.txt
  * Barbarian (Frenzy)
    * swapped all stats from "Skill2" through "LvlPerLvl2" and "Skill3" through "LvlPerLvl3" (swapped Iron Skin and Taunt location on Frenzy Act 5 merc skill list)
    * changed new "Skill2" to Double Swing from Taunt (Frenzy A5 mercs now use Double Swing instead of Taunt due to Frenzy synergy changes)
    * changed new "Mode2" to 4 from 5 (changes Double Swing animation type to attacking from casting)
    * decreased new "Level2" to 4/7/9 from 7/13/17 (Double Swing level baseline reduced to 4/7/9 from 7/13/17)
    * decreased new "LvlPerLvl2" to 3 from 6 (Double Swing level scaling halved)

#### itemstatcost.txt
  * increased armorclass_vs_hth "Save Bits" to 9 from 8 (increased range of defense vs melee to 0-511 from 0-255)
  * increased maxfireresist, maxlightresist, maxcoldresist, and maxpoisonresist "Save Bits" to 6 from 5 and changed "Save Add" to 30 from 0 (increases range of maximum fire/light/cold/poison resist to -30-33 from 0-31)
  * increased poisonmindam and poisonmaxdam "Save Bits" to 11 from 10 (increased range of poison damage bitrate to 0-2047 from 0-1023)
  * increased hpregen "Save Bits" to 7 from 6 and changed "Save Add" to 50 from 30 (increased range of replenish life to -50-77 from -30-33)
  * increased item_attackertakeslightdamage "Save Bits" to 8 from 5 (increased range of attacker takes lightning damage to 0-255 from 0-31)

  * item_heavenlyburden
    * added new entry for "item_heavenlyburden" (cloned row 155)
    * set "*ID" to 361
    * set "Add" and "Multiply" to blank
    * set "1.09-Save Bits" to blank
    * set "descpriority" to 1
    * set "descfunc" to 19
    * set "descstrpos" and "descstrneq" to ModStrHeavenlyBurden (see item-modifiers.json)

#### magicprefix.txt
  * Defense
    * Stout (row 121)
      * added 41 to "maxlevel"
    * Stout (122)
      * added 41 to "maxlevel"
    * Stout (123)
      * added 41 to "maxlevel"
    * Stout (130)
      * added 44 to "maxlevel"
    * Stout (131)
      * added 44 to "maxlevel"
    * Stout (132)
      * added 44 to "maxlevel"
    * Stout (137)
      * added 47 to "maxlevel"
    * Stout (138)
      * added 47 to "maxlevel"
    * Blanched (141)
      * added 31 to "maxlevel"

  * Enhanced Defense
    * Sturdy (145)
      * added 24 to "maxlevel"
    * Sturdy (146)
      * added 30 to "maxlevel"
    * Strong (147)
      * added 35 to "maxlevel"
    * Glorious (148)
      * added 49 to "maxlevel"

  * Enhanced Damage
    * Jagged (188)
      * added 25 to "maxlevel"
    * Deadly (189)
      * added 31 to "maxlevel"
    * Vicious (190)
      * added 40 to "maxlevel"
    * Brutal (191)
      * added 55 to "maxlevel"

  * Stamina
    * Rugged (206)
      * added 20 to "maxlevel"
    * Rugged (209)
      * added 20 to "maxlevel"
    * Rugged (212)
      * added 20 to "maxlevel"
    * Rugged (214)
      * added 15 to "maxlevel"

  * Attack Rating
    * Brone (220)
      * added 48 to "maxlevel"
    * Bronze (221)
      * added 48 to "maxlevel"
    * Bronze (222)
      * added 48 to "maxlevel"
    * Bronze (229)
      * added 51 to "maxlevel"
    * Bronze (230)
      * added 51 to "maxlevel"
    * Bronze (231)
      * added 51 to "maxlevel"
    * Bronze (236)
      * added 56 to "maxlevel"
    * Bronze (237)
      * added 56 to "maxlevel"
    * Bronze (240)
      * added 21 to "maxlevel"
    * Iron (241)
      * added 26 to "maxlevel"
    * Steel (242)
      * added 31 to "maxlevel"

  * Attack Rating/Enhanced Damage
    * Sharp (259)
      * added 46 to "maxlevel"
    * Fine (260)
      * added 55 to "maxlevel"

  * Mana
    * Lizard's (306)
      * added 29 to "maxlevel"
    * Snake's (307)
      * added 36 to "maxlevel"

  * All Resistances
    * Shimmering (325)
      * added 38 to "maxlevel"
    * Shimmering (330)
      * added 41 to "maxlevel"

  * Cold Resist
    * Azure (340)
      * added 29 to "maxlevel"
    * Azure (344)
      * added 34 to "maxlevel"
    * Azure (348)
      * added 39 to "maxlevel"

  * Fire Resist
    * Crimson (360)
      * added 29 to "maxlevel"
    * Crimson (364)
      * added 34 to "maxlevel"
    * Crimson (368)
      * added 39 to "maxlevel"

  * Lightning Resist
    * Tangerine (379)
      * added 29 to "maxlevel"
    * Tangerine (383)
      * added 34 to "maxlevel"
    * Tangerine (387)
      * added 39 to "maxlevel"

  * Poison Resist
    * Beryl (399)
      * added 29 to "maxlevel"
    * Beryl (403)
      * added 34 to "maxlevel"
    * Beryl (407)
      * added 39 to "maxlevel"

  * Attack Rating/Damage to Demons
    * Assamic (425) (Lunar)
      * added 44 to "maxlevel"

  * Maximum Damage Per Level
    * Gritty (533) (Grinding)
      * increased "mod1param" to 9 from 6 (maximum damage per level increased to 1.125 from 0.75)

  * Cold Damage
    * Snowflake (543) (Snowy)
      * added 69 to "maxlevel"

  * Fire Damage
    * Ember (547) (Fiery)
      * added 76 to "maxlevel"

  * Lightning Damage
    * Static (552)
      * added 75 to "maxlevel"

  * Poison Damage
    * Septic (557)
      * added 34 to "maxlevel"

  * Increased Stack Size
    * Compact (594)
      * added 37 to "maxlevel"

  * Attack Rating/Damage to Undead
    * Consecrated (597)
      * added 34 to "maxlevel"

  * Minimum Damage
    * Bloody (606)
      * increased "mod1min" and "mod1max" to 5/5 from 3/3 (minimum damage increased to 5 from 3)
    * Red (609)
      * decreased "level" to 80 from 90 (item level requirement decreased to 80 from 90)
      * decreased "levelreq" to 75 from 82 (level requirement decreased to 75 from 82)
    * Bloody (672) ("medium"/large charms)
      * added new entry for "Bloody" (cloned row 608)
      * set "level" to 90
      * set "levelreq" to 82
      * set "mod1min" and "mod1max" to 4/4 (4 minimum damage)
    * Sanguinary (673) (small charms)
      * added new entry for "Sanguinary" (cloned row 609)
      * set "level" to 94
      * set "levelreq" to 85
      * set "mod1min" and "mod1max" to 2/2 (2 minimum damage)

  * Maximum Damage
    * Forked (611)
      * increased "mod1min" and "mod1max" to 7/7 from 2/2 (maximum damage increased to 7 from 2)
    * Serrated (612)
      * increased "mod1min" and "mod1max" to 11/11 from 3/3 (maximum damage increased to 11 from 3)
    * Jagged (613)
      * increased "mod1min" and "mod1max" to 2/2 from 1/1 (maximum damage increased to 2 from 1)
    * Forked (614)
      * increased "mod1min" and "mod1max" to 6/6 from 2/2 (maximum damage increased to 6 from 2)
    * Jagged (615)
      * increased "mod1min" and "mod1max" to 3/3 from 1/1 (maximum damage increased to 3 from 1)
    * Serrated (674)
      * added new entry for "Serrated' (cloned row 614)
      * set "level" to 82
      * set "levelreq" to 72
      * set "mod1min" and "mod1max" to 8/8 (8 maximum damage)

  * Cold Damage
    * Snowflake (616) (Snowy)
      * added 44 to "maxlevel"
    * Snowflake (620) (Snowy)
      * added 68 to "maxlevel"
    * Snowflake (624) (Snowy)
      * added 90 to "maxlevel"

  * Fire Damage
    * Ember (628)
      * added 42 to "maxlevel"
    * Ember (632)
      * added 66 to "maxlevel"
    * Ember (636)
      * added 88 to "maxlevel"

  * Lightning Damage
    * Static (640)
      * added 43 to "maxlevel"
    * Static (644)
      * added 67 to "maxlevel"
    * Static (648)
      * added 89 to "maxlevel"

  * Poison Damage
    * Septic (652)
      * added 41 to "maxlevel"
    * Septic (656)
      * added 65 to "maxlevel"
    * Septic (660)
      * added 87 to "maxlevel"

#### magicsuffix.txt
  * Damage Reduced
    * of Health (row 117)
      * added 25 to "maxlevel" (no longer spawns on ilvl 26+ items)
    * of Protection (118)
      * added 34 to "maxlevel"
    * of Protection (122)
      * added 40 to "maxlevel"
    * of Absorption (123)
      * added ring to "itype4" (now spawns on rings)
    * of Life (124)
      * added ring to "itype4"

  * Magic Damage Reduced
    * of Warding (126)
      * added 31 to "maxlevel"

  * Ignore Target's Defense
    * of Piercing (160)
      * added spea to "itype4"

  * Attacker Takes Damage
    * of Thorns (163)
      * added 33 to "maxlevel"
    * of Spikes (164)
      * added 46 to "maxlevel"
    * of Malice (167)
      * increased "mod1min" and "mod1max" to 3/9 from 1/5 (attacker takes damage increased to 3-9 from 1-5)

  * Increased Attack Speed
    * of Readiness (168)
      * added 45 to "maxlevel"
    * of Swiftness (170)
      * changed "itype" to weap from mele (now spawns on missile weapons)
    * of Quickness (171)
      * changed "itype" to weap from mele

  * Faster Cast Rate
    * of the Apprentice (176)
      * added head to "itype6" (now spawns on necromancer heads)
    * of the Magus (177)
      * deleted scep from "etype1" (now spawns on scepters)

  * Cold Damage
    * of Frost (178)
      * added 26 to "maxlevel"
    * of the Icicle (179)
      * added 44 to "maxlevel"
      * increased "mod1max" to 3 from 1, increased "mod2min" and "mod2max" to 4/6 from 3/4 (cold damage increased to 1-3 minimum/4-6 maximum from 1/3-4)
    * of the Glacier (180)
      * increased "mod1min" and "mod1max" to 6/8 from 2/4, increased "mod2min" and "mod2max" to 11/18 from 4/15 (cold damage increased to 6-8 minimum/11-18 maximum from 2-4/4-15)
    * of Winter (181)
      * increased "mod1min" and "mod1max" to 13/17 from 5/9, increased "mod2min" and "mod2max" to 29/71 from 16/50 (cold damage increased to 13-17 minimum/29-71 maximum from 5-9/16-50)
    * of Frost (182)
      * decreased "level" to 39 from 55 (now spawns at ilvl 39+ instead of 55+)
    * of Frigidity (183)
      * added 36 to "maxlevel"

  * Fire Damage
    * of Flame (185)
      * added 24 to "maxlevel"
    * of Fire (186)
      * added 42 to "maxlevel"
      * increased "mod1min" and "mod1max" to 7/9 from 1/4, increased "mod2min" and "mod2max" to 12/15 from 6/11 (fire damage increased to 7-9 minimum/12-15 maximum from 1-4/6-11)
    * of Burning (187)
      * increased "mod1min" and "mod1max" to 15/18 from 5/9, increased "mod2min" and "mod2max" to 22/26 from 10/20 (fire damage increased to 15-18 minimum/22-26 maximum from 5-9/10-20)
    * of Incineration (188)
      * increased "mod1min" and "mod1max" to 31/36 from 10/20, increased "mod2min" and "mod2max" to 43/109 from 21/75 (fire damage increased to 31-36 minimum/43-109 maximum from 10-20/21-75)
    * of Flame (189)
      * increased "mod1min" and "mod1max" to 10/15 from 1/1, increased "mod2min" and "mod2max" to 23/28 from 2/6 (fire damage increased to 10-15 minimum/23-28 maximum from 1/2-6)

  * Lightning Damage
    * of Passion (190)
      * added 56 to "maxlevel"
    * of Shock (191)
      * added 24 to "maxlevel"
    * of Lightning (192)
      * added 33 to "maxlevel"
      * increased "mod2min" and "mod2max" to 13/21 from 9/16 (lightning damage increased to 13-21 maximum from 9-16)
    * of Thunder (193)
      * increased "mod2min" and "mod2max" to 28/53 from 17/40 (lightning damage increased to 28-53 maximum from 17-40)
    * of Storms (194)
      * increased "mod2min" and "mod2max" to 62/141 from 41/120 (lightning damage increased to 62-141 maximum from 41-120)
    * of Shock (195)
      * increased "mod2min" and "mod2max" to 44/91 from 11/23 (lightning damage increased to 44-91 maximum from 11-23)
    * of Ennui (196)
      * added 56 to "maxlevel"

  * Maximum Damage
    * of Craftsmanship (197)
      * added 10 to "maxlevel"
    * of Quality (198)
      * added 13 to "maxlevel"
    * of Maiming (199)
      * added 18 to "maxlevel"
    * of Slaying (200)
      * added 24 to "maxlevel"
    * of Craftsmanship (209)
      * added 44 to "maxlevel"

  * Minimum Damage
    * of Worth (225)
      * added 47 to "maxlevel"
    * of Measure (226)
      * added 75 to "maxlevel"
    * of Worth (230)
      * added 58 to "maxlevel"

  * Poison Damage
    * of Blight (236)
      * added 24 to "maxlevel"
    * of Venom (237)
      * added 32 to "maxlevel"

  * Dexterity
    * of Dexterity (242)
      * added 42 to "maxlevel"
    * of Skill (243)
      * added 58 to "maxlevel"
    * of Dexterity (248)
      * added 55 to "maxlevel"
    * of Dexterity (253)
      * added 45 to "maxlevel"

  * Gold Find
    * of Greed (284)
      * increased "mod1min" and "mod1max" to 8/15 from 5/10 (gold find increased to 8-15% from 5-10%)
    * of Greed (285)
      * increased "mod1min" and "mod1max" to 16/30 from 11/22 (gold find increased to 16-30% from 11-22%)
    * of Avarice (287)
      * increased "mod1min" and "mod1max" to 15/35 from 10/30 (gold find increased to 15-35% from 10-30%)

  * Energy
    * of Energy (295)
      * added 20 to "maxlevel"
    * of the Mind (296)
      * added 30 to "maxlevel"
    * of Energy (301)
      * added 30 to "maxlevel"
    * of Energy (306)
      * added 15 to "maxlevel"

  * Light Radius
    * of Light (312)
      * added 16 to "maxlevel"

  * Life
    * of the Jackal (315)
      * added 24 to "maxlevel"
    * of the Fox (316)
      * added 29 to "maxlevel"
    * of the Jackal (323)
      * added 58 to "maxlevel"
    * of the Jackal (329)
      * added 67 to "maxlevel"

  * Strength
    * of Strength (374)
      * added 57 to "maxlevel"
    * of Might (375)
      * added 70 to "maxlevel"
    * of Strength (380)
      * added 73 to "maxlevel"

  * Faster Run/Walk
    * of Inertia (401)
      * increased "mod1min" and "mod1max" to 8/8 from 7/7 (faster run/walk increased to 8% from 7%)
    * of Inertia (402)
      * increased "mod1min" and "mod1max" to 7/7 from 5/5 (faster run/walk increased to 7% from 5%)

  * Life Per Level
    * of the Kraken (409) (Centaur)
      * increased "mod1param" to 14 from 6 (life per level increased to 1.75 from 0.75)

  * Mana Per Level
    * of Memory (410)
      * increased "mod1param" to 14 from 6 (mana per level increased to 1.75 from 0.75)

  * Life Per Level/Mana Per Level
    * of the Elephant (411)
      * increased "mod1param" to 10 from 4 (life per level increased to 1.25 from 0.5)
      * increased "mod2param" to 6 from 2 (mana per level increased to 0.75 from 0.25)

  * Chance to Cast
    * of Firebolts (421)
      * added 19 to "maxlevel"
    * of Firebolts (422)
      * increased "mod1max" to 6 from 4 (Fire Bolt on attack level increased to 6 from 4)
    * of Charged Shield (423) (of Charged Bolt)
      * added 25 to "maxlevel"
    * of Icebolt (426)
      * increased "mod1min" to 8 from 5 (Ice Bolt on attack proc chance increased to 8% from 5%)
    * of Nova Shield (436)
      * added 37 to "maxlevel"
    * of Lightning (439)
      * increased "mod1min" to 8 from 5 (Lightning on attack proc chance increased to 8% from 5%)
    * of Chain Lightning (444)
      * added 44 to "maxlevel"
    * of Hydra Shield (456)
      * increased "mod1max" to 5 from 3 (Hydra when struck level increased to 5 from 3)
    * of Damage Amplification (664)
      * increased "mod1min" to 8 from 5 (Amplify Damage on striking proc chance increased to 8% from 5%)

  * Poison Damage
    * of Blight (684)
      * added 20 to "maxlevel"
    * of Blight (688)
      * added 32 to "maxlevel"
    * of Blight (692)
      * added 43 to "maxlevel

  * Cold Damage
    * of Frost (696)
      * added 22 to "maxlevel"
    * of Frost (700)
      * added 34 to "maxlevel"
    * of Frost (704)
      * added 45 to "maxlevel"

  * Fire Damage
    * of Flame (708)
      * added 21 to "maxlevel"
    * of Flame (712)
      * added 33 to "maxlevel"
    * of Flame (716)
      * added 44 to "maxlevel"

  * Lightning Damage
    * of Shock (720)
      * added 21 to "maxlevel"
    * of Shock (724)
      * added 33 to "maxlevel"
    * of Shock (728)
      * added 44 to "maxlevel"

#### misc.txt
  * set "ShowLevel" to 1 for amulets/rings/charms/jewels (shows item level)

  * Minor Mana Potion
    * changed "HellUpgrade" to mp4 from mp5 (vendors only sell greater mana potions instead of super mana potions in Hell)

  * Light Mana Potion
    * changed "LysanderMin" and "LysanderMax" to blank from 1 (Lysander no longer sells light mana potions in Normal)
    * changed "DrognanMin" and "DrognanMax" to blank from 1 (Drognan no longer sells light mana potions in Normal)
    * changed "HellUpgrade" to mp4 from mp5 (vendors only sell greater mana potions instead of super mana potions in Hell)

  * Mana Potion
    * changed "OrmusMin" and "OrmusMax" to blank from 1 (Ormus no longer sells mana potions in Normal)
    * changed "HellUpgrade" to mp4 from mp5 (vendors only sell greater mana potions instead of super mana potions in Hell)

  * Greater Mana Potion
    * changed "MalahMin" and "MalahMax" to blank from 1 (Malah no longer sells greater mana potions in Normal)
    * changed "JamellaMin" and "JamellaMax" to blank from 1 (Jamella no longer sells greater mana potions in Normal)
    * changed "HellUpgrade" to xxx from mp5 (vendors only sell greater mana potions instead of super mana potions in Hell)

#### missiles.txt
  * throwaxe
    * increased "Range" to 30 from 20 (throwing axes travel 50% farther)

  * throwknife
    * increased "Vel" and "MaxVel" to 32 from 24 (throwing knives travel 33% faster)
    * increased "Range" to 23 from 20 (throwing knives travel 53% farther overall with velocity increase)

  * coldarrow
    * increased "Range" to 40 from 20 (makes it equal range with other elemental arrows)

  * diablight
    * increased "Range" to 40 from 30 (makes his Red Lightning hit at melee range in Nightmare and Hell)

#### monprop.txt
  * added 6 new rows for Dclone and the Ubers
  * diabloclone (Dclone)
    * added res-curse to "prop1 (H)", set "min1 (H)" and "max1 (H)" to 80/80 (Diablo Clone now has 80% curse length reduction)

  * ubermephisto (Uber Mephisto)
    * added cast2 to "prop1 (H)", set "min1 (H)" and "max2 (H)" to 30/30 (Uber Mephisto has his usual 30% faster cast rate)
    * added swing2 to "prop2 (H)", set "min2 (H)" and "max2 (H)" to 30/30 (has his usual 30% increased attack speed)
    * added res-curse to "prop3 (H)", set "min3 (H)" and "max3 (H)" to 80/80 (now has 80% curse length reduction)

  * uberdiablo (Uber Diablo/Pandemonium Diablo)
    * added curse_resistance to "prop1 (H)", set "min1 (H)" and "max1 (H)" to 80/80 (Uber Diablo now has 80% curse length reduction)

  * uberizual (Uber Izual)
    * added res-curse to "prop1 (H)", set "min1 (H)" and "max1 (H)" to 80/80 (Uber Izual now has 80% curse length reduction)

  * uberandariel (Lilith)
    * added res-curse to "prop1 (H)", set "min1 (H)" and "max1 (H)" to 80/80 (Lilith now has 80% curse length reduction)

  * uberduriel (Uber Diablo)
    * added res-curse to "prop1 (H)", set "min1 (H)" and "max1 (H)" to 80/80 (Uber Duriel now has 80% curse length reduction)

  * uberbaal (Uber Baal)
    * added res-curse to "prop1 (H)", set "min1 (H)" and "max1 (H)" to 80/80 (Uber Baal now has 80% curse length reduction)

#### monstats.txt
  * andariel
    * decreased "ToBlock(N)" to 15 from 20 (Nightmare Andariel block chance decreased to 15% from 20%)
    * decreased "ToBlock(H)" to 25 from 40 (Hell block chance decreased to 25% from 40%)
    * increased "AC(N)" to 123 from 110 (Nightmare Andariel defense increased by ~12%, for example at level 49 she has 841 defense instead of 752 defense)
    * increased "AC(H)" to 154 from 110 (Hell defense increased by ~40%, at level 75 she has 2271 defense instead of 1622 defense)

  * duriel
    * decreased duriel "ToBlock(N)" to 20 from 25 (Nightmare Duriel block chance decreased to 20% from 25%)
    * decreased duriel "ToBlock(H)" to 30 from 50 (Hell block chance decreased to 30% from 50%)
    * increased duriel "AC(N)" to 136 from 120 (Nightmare Duriel defense increased by ~13%, for example at level 55 he has 1028 defense instead of 907 defense)
    * increased duriel "AC(H)" to 216 from 120 (Hell defense increased by 80%, at level 88 he has 3680 defense instead of 2044 defense)

  * mephisto
    * set "flying" to 1 (allows Mephisto to float over the moat, be careful not to kill him over the moat otherwise he won't drop any loot)
    * decreased "ToBlock" to 15 from 20 (Normal Mephisto block chance decreased to 15% from 20%)
    * decreased "ToBlock(N)" to 20 from 40 (Nightmare block chance decreased to 20% from 40%)
    * decreased "ToBlock(H)" to 30 from 50 (Hell block chance decreased to 30% from 50%)
    * increased "AC" to 140 from 124 (Normal Mephisto defense increased by ~13%, for example at level 26 he has 218 defense instead of 193 defense)
    * increased "AC(N)" to 266 from 160 (Nightmare defense increased by ~66%, at level 59 he has 2138 defense instead of 1286 defense)
    * increased "AC(H)" to 288 from 160 (Hell defense increased by 80%, at level 87 he has 4855 defense instead of 2697 defense)

  * diablo
    * decreased "ToBlock" to 20 from 25 (Normal Diablo block chance decreased to 20% from 25%)
    * decreased "ToBlock(N)" to 25 from 40 (Nightmare block chance decreased to 25% from 40%)
    * decreased "ToBlock(H)" to 30 from 50 (Hell block chance decreased to 30% from 50%)
    * increased "AC" to 98 from 87 (Normal Diablo defense increased by ~13%, for example at level 40 he has 235 defense instead of 208 defense)
    * increased "AC(N)" to 210 from 140 (Nightmare defense increased by 50%, at level 62 he has 1764 defense instead of 1176 defense)
    * increased "AC(H)" to 252 from 140 (Hell defense increased by 80%, at level 94 he has 4561 defense instead of 2534 defense)

  * diabloclone (Dclone)
    * added diabloclone to "MonProp" (uses diabloclone entry in monprop.txt)
    * decreased "Level(H)" to 100 from 110 (Diablo Clone level decreased to 100 from 110)
    * decreased "ToBlock(H)" to 30 from 50 (block chance reduced to 30% from 50%)
    * increased "MinHP(H) and "MaxHP(H) to 8128/8128 from 6427/6427 (combined with decrease to "Level(H)" life remains roughly the same at 642680)
    * increased "AC(H)" to 303 from 140 (defense increased by ~96%, at level 100 he has 5802 defense instead of 2940 defense at level 110)
    * increased "A1MinD(H)", "A1MaxD(H)", and "A1TH(H)" to 116/219/353 from 100/190/215 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 1 remain roughly the same at 131-247 and 14042 respectively)
    * increased "A2MinD(H)", "A2MaxD(H)", and "A2TH(H)" to 127/265/329 from 110/230/200 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 2 remain roughly the same at 143-299 and 13087 respectively)

  * baalcrab (Baal)
    * decreased "ToBlock" to 25 from 40 (Normal Baal block chance decreased to 25% from 40%)
    * decreased "ToBlock(N)" to 30 from 45 (Nightmare block chance decreased to 30% from 45%)
    * decreased "ToBlock(H)" to 30 from 55 (Hell block chance decreased to 30% from 55%)
    * increased "AC" to 130 from 87 (Normal Baal defense increased by ~50%, for example at level 60 he has 468 defense instead of 313 defense)
    * increased "AC(N)" to 231 from 150 (Nightmare defense increased by 54%, at level 75 he has 2300 defense instead of 1494 defense)
    * increased "AC(H)" to 316 from 150 (Hell defense increased by ~111%, at level 99 he has 5997 defense instead of 2847 defense)
    * changed "TreasureClassQuest(H)" to BaalQSpecial from Baalq (H) (quest Hell Baal will drop the BaalQSpecial TC in treasureclassex.txt)

  * baalclone (Baal Clone)
    * decreased "ToBlock" to 25 from 40 (Normal Baal Clone block chance decreased to 25% from 40%)
    * decreased "ToBlock(N)" to 30 from 45 (Nightmare block chance decreased to 30% from 45%)
    * decreased "ToBlock(H)" to 30 from 55 (Hell block chance decreased to 30% from 55%)
    * increased "AC" to 130 from 87 (Normal Baal Clone defense increased by ~50%, for example at level 60 he has 468 defense instead of 313 defense)
    * increased "AC(N)" to 246 from 160 (Nightmare defense increased by ~54%, at level 69 he has 2273 defense instead of 1478 defense)
    * increased "AC(H)" to 338 from 160 (Hell defense increased by ~111%, at level 95 he has 6175 defense instead of 2923 defense)

  * ubermephisto (Uber Mephisto)
    * changed "MonProp" to ubermephisto from mephisto (uses ubermephisto entry in monprop.txt instead of mephisto)
    * decreased "Level(H)" to 100 from 110 (Uber Mephisto level decreased to 100 from 110)
    * increased "Drain(H) to 10 from blank (drain effectiveness increased to 10% from 0%)
    * decreased "ToBlock(H)" to 30 from 50 (block chance decreased to 30% from 50%)
    * increased "MinHP(H) and "MaxHP(H) to 8221/8347 from 6500/6600 (combined with decrease to "Level(H)" life remains roughly the same at 650034-659997)
    * increased "AC(H)" to 343 from 160 (defense increased by ~95%, at level 100 he has 6568 defense instead of 3360 defense at level 110)
    * increased "A1MinD(H)", "A1MaxD(H)", and "A1TH(H)" to 431/507/329 from 375/440/200 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 1 remain roughly the same at 487-572 and 13087 respectively)

  * uberdiablo (Uber Diablo/Pandemonium Diablo)
    * added uberdiablo to "MonProp" (uses uberdiablo entry in monprop.txt)
    * decreased "Level(H)" to 100 from 110 (Uber Diablo level decreased to 100 from 110)
    * decreased "ToBlock(H)" to 30 from 50 (block chance decreased to 30% from 50%)
    * increased "MinHP(H) and "MaxHP(H) to 8221/8347 from 6500/6600 (combined with decrease to "Level(H)" life remains roughly the same at 650034-659997)
    * increased "AC(H)" to 300 from 140 (defense increased by ~96%, at level 100 he has 5745 defense instead of 2940 defense at level 110)
    * increased "A1MinD(H)", "A1MaxD(H)", and "A1TH(H)" to 426/438/353 from 370/380/215 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 1 remain roughly the same at 481-494 and 14042 respectively)
    * increased "A2MinD(H)", "A2MaxD(H)", and "A2TH(H)" to 127/265/329 from 110/230/200 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 2 remain roughly the same at 143-299 and 13087 respectively)

  * uberizual (Uber Izual)
    * added uberizual to "MonProp" (uses uberizual entry in monprop.txt)
    * decreased "Level(H)" to 100 from 110 (Uber Izual level decreased to 100 from 110)
    * decreased "ToBlock(H)" to 30 from 50 (block chance decreased to 30% from 50%)
    * increased "MinHP(H) and "MaxHP(H) to 8221/8347 from 6500/6600 (combined with decrease to "Level(H)" life remains roughly the same at 650034-659997)
    * increased "AC(H)" to 258 from 120 (defense increased by ~96%, at level 100 he has 4940 defense instead of 2520 defense at level 110)
    * increased "A1MinD(H)", "A1MaxD(H)", and "A1TH(H)" to 403/461/329 from 350/400/200 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 1 remain roughly the same at 455-520 and 13087 respectively)
    * increased "El1MinD(H)" and "El1MaxD(H)" to 58/93 from 50/80 (combined with decrease to "Level(H)" cold damage for melee attack 1 remains roughly the same at 65-105)

  * uberandariel (Lilith)
    * added uberandariel to "MonProp" (uses uberandariel entry in monprop.txt)
    * decreased "Level(H)" to 100 from 110 (Lilith level decreased to 100 from 110)
    * decreased "ToBlock(H)" to 30 from 40 (block chance decreased to 30% from 40%)
    * increased "AC(H)" to 176 from 110 (defense increased by ~46%, at level 100 she has 3370 defense instead of 2310 defense at level 110)
    * increased "A1MinD(H)", "A1MaxD(H)", and "A1TH(H)" to 461/507/772 from 400/440/470 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 1 remain roughly the same at 520-572 and 30710 respectively)
    * increased "El1MinD(H)" and "El1MaxD(H)" to 38/38 from 33/33 (combined with decrease to "Level(H)" poison damage for melee attack 1 remains roughly the same at 754 over 18 seconds)

  * uberduriel (Uber Duriel)
    * added uberduriel to "MonProp" (uses uberduriel entry in monprop.txt)
    * decreased "Level(H)" to 100 from 110 (Uber Duriel level decreased to 100 from 110)
    * decreased "ToBlock(H)" to 30 from 50 (block chance decreased to 30% from 50%)
    * increased "MinHP(H) and "MaxHP(H) to 8221/8347 from 6500/6600 (combined with decrease to "Level(H)" life remains roughly the same at 650034-659997)
    * increased "AC(H)" to 258 from 120 (defense increased by ~96%, at level 100 he has 4940 defense instead of 2520 defense at level 110)
    * increased "A1MinD(H)", "A1MaxD(H)", and "A1TH(H)" to 415/438/181 from 360/380/110 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 1 remain roughly the same at 468-495 and 7200 respectively)
    * increased "A2MinD(H)", "A2MaxD(H)", and "A2TH(H)" to 132/190/246 from 115/165/150 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 2 remain roughly the same at 149-214 and 9785 respectively)

  * uberbaal (Uber Baal)
    * added uberbaal to "MonProp" (uses uberbaal entry in monprop.txt)
    * decreased "Level(H)" to 100 from 110 (Uber Baal level decreased to 100 from 110)
    * decreased "ToBlock(H)" to 30 from 55 (block chance decreased to 30% from 55%)
    * increased "MinHP(H) and "MaxHP(H) to 8221/8347 from 6500/6600 (combined with decrease to "Level(H)" life remains roughly the same at 650034-659997)
    * increased "AC(H)" to 375 from 150 (defense increased by ~128%, at level 100 he has 7181 defense instead of 3150 defense at level 110)
    * increased "A1MinD(H)", "A1MaxD(H)", and "A1TH(H)" to 380/438/411 from 330/380/250 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 1 remain roughly the same at 429-495 and 16349 respectively)
    * increased "A2MinD(H)", "A2MaxD(H)", and "A2TH(H)" to 190/277/411 from 165/240/250 (combined with decrease to "Level(H)" physical damage and attack rating for melee attack 2 remain roughly the same at 214-313 and 16349 respectively)
    * increased "El1MinD(H)" and "El1MaxD(H)" to 139/231 from 120/200 (combined with decrease to "Level(H)" fire damage for melee attack 1 remains the same at 157-261)
    * increased "El2MinD(H)" and "El2MaxD(H)" to 139/185 from 120/160 (combined with decrease to "Level(H)" cold damage for melee attack 2 remain roughly the same at 157-209)

  * trangvampire
    * added new entry for "trangvampire" (cloned row 137)
    * set "hcIdx" to 742 and "Code" to Z4 (this is part of a change to allow Trang vampires to use necro casting frames instead of slow vampire casting frames)

#### properties.txt
  * res-curse
    * added new entry for "res-curse" (cloned row 33)
    * set "stat1" to curse_resistance
    * set "*Tooltip" to Curse Resist +#%

  * heavenlyburden
    * added new entry for "heavenlyburden" (cloned row 117)
    * set "stat1" to item_heavenlyburden (see item_heavenlyburden entry in itemstatcost.txt)
    * set "*Tooltip" to Heavenly Burden

#### runes.txt
  * Beast
    * added mace to "itype4" (allows Beast to be created in maces)
    * changed "T1Code5" to oskill from charged, changed "T1Param5 to Maul from Summon Grizzly, decreased "T1Min5" and "T1Max5" to 3/3 from 5/13 (level 3 Maul oskill instead of Summon Grizzly charges)

  * Brand
    * changed "T1Code4" to hit-skill from gethit-skill, decreased "T1Min4" and "T1Max4" to 18/9 from 35/14 (Amplify Damage on striking instead of when struck, proc chance decreased to 18% from 35%, level decreased to 9 from 14)

  * Chains of Honor
    * increased "T1Min2" and "T1Max2" to 100/100 from 70/70 (enhanced defense increased to 100% from 70%)

  * Doom
    * added mace to "itype4"

  * Enigma
    * changed "T1Code1" to ac% from ac and decreased "T1Min1" and "T1Max1" to 100/130 from 750/775 (100-130% enhanced defense instead of 750-775 defense)
    * decreased "T1Min2" and "T1Max2" to 5/5 from 14/14 (life after each kill decreased to 5 from 14)
    * deleted all stats from "T1Code3" through "T1Max4" and moved the other stats over (removed 45% faster run/walk and 0.75 strength per level)
    * decreased new "T1Param4" to 4 from 8 (magic find per level decreased to 0.5 from 1)

  * Famine
    * added mace to "itype3"
    * increased "T1Min5" and "T1Max5" to 240/270 from 180/200 (magic damage increased to 240-270 from 180-200)
    * increased "T1Min6" and "T1Max6" to 100/300 from 50/200 (elemental damage increased to 100-300 from 50-200)

  * Flickering Flame
    * decreased "T1Min2" and "T1Max2" to 1/1 from 4/8 (Resist Fire aura level decreased to 1 from 4-8)

  * Grief
    * changed "T1Code1" to dmg% from dmg-dem/lvl, set "T1Min1" and "T1Max1" to 180/200 (180-200% enhanced damage instead of damage to demons per level)
    * decreased "T1Min2" and "T1Max2" to 120/140 from 340/400 (+damage decreased to 120-140 from 340-400)
    * increased "T1Min3" to 35 from 30 (increased attack speed increased to 35-40% from 30-40%)

  * Heart of the Oak
    * added hamm to "itype3"
    * changed "T1Code2" to oskill from from charged, decreased "T1Min2" and "T1Max2" to 1/1 from 25/4 (Oak Sage charges changed to oskill, level decreased to 1 from 4)
    * decreased "T1Min1" and "T1Max1" to 30/30 from 40/40 (faster cast rate decreased to 30% from 40%)
    * decreased "T1Min4" and "T1Max4" to 2/2 from 3/3 (all skills decreased to 2 from 3)
    * decreased "T1Min6" and "T1Max6" to 25/30 from 30/40 (all resistances decreased to 25-30% from 30-40%)

  * Holy Thunder
    * changed "*RunesUsed" to EthRalOrt from EthRalOrtTal
    * deleted stats in "Rune4" (removed Tal rune)
    * decreased "T1Min2" and "T1Max2" to 10/30 from 20/60 (lightning damage decreased to 10-30 from 20-60)
    * decreased "T1Min4" and "T1Max4" to 40/40 from 60/60 (lightning resist decreased to 40% from 60%)

  * Insight
    * ~~decreased "T1Min1" and "T1Max1" to 90/120 from 200/260 (enhanced damage decreased to 90-120% from 200-260%)~~ (see patch 1.03)
    * decreased "T1Min2" and "T1Max2" to 35/60 from 180/250 (attack rating decreased to 35-60% from 180-250%)
    * ~~decreased "T1Min4" and "T1Max4" to 1/3 from 1/6 (Critical Strike oskill level decreased to 1-3 from 1-6)~~ (see patch 1.03)
    * decreased "T1Min6" and "T1Max6" to 1/3 from 12/17 (Meditation level decreased to 1-3 from 12-17)

  * King's Grace
    * added mace to "itype3"
    * added spea to "itype4"
    * increased "T1Min5" and "T1Max5" to 175/175 from 100/100 (attack rating against demons increased to 175 from 100)
    * increased "T1Min6" and "T1Max6" to 175/175 from 100/100 (attack rating against undead increased to 175 from 100)
    * added swing2 to "T1Code7", set "T1Min7" and "T1Max7" to 15/15 (15% increased attack speed)

  * Kingslayer
    * added spea to "itype3"
    * increased "T1Min2" and "T1Max2" to 260/310 from 230/270 (enhanced damage increased to 260-310% from 230-270%)
    * increased "T1Min3" and "T1Max3" to 35/35 from 25/25 (target defense increased to -35% from -25%)
    * increased "T1Min6" and "T1Max6" to 4/4 from 1/1 (Vengeance oskill level increased to 4 from 1)
    * increased "T1Min7" and "T1Max7" to 120/120 from 40/40 (gold find increased to 120% from 40%)

  * Last Wish
    * changed "itype1" to weap and deleted all stats from "itype2" to "itype3" (allows Last Wish to be created in any weapon type)
    * increased "T1Min1" and "T1Max1" to 410/433 from 330/375 (enhanced damage increased to 410-433% from 330-375%)
    * increased "T1Min4" to 13 from 6 (Fade when struck proc chance increased to 13% from 6%)

  * Lawbringer
    * added mace to "itype4"
    * added club to "itype5"

  * Oath
    * added hamm to "itype4"

  * Obsession
    * decreased "T1Min3" and "T1Max3" to 55/55 from 65/65 (faster cast rate decreased to 55% from 65%)
    * decreased "T1Min4" and "T1Max4" to 35/35 from 60/60 (faster hit recovery decreased to 35% from 60%)

  * Voice of Reason
    * added spea to "itype3"

  * Spirit
    * decreased "T1Min1" and "T1Max1" to 15/15 from 55/55 (faster hit recovery decreased to 15% from 55%)
    * decreased "T1Min2" and "T1Max2" to 21/32 from 89/112 (mana decreased to 21-32 from 89-112)
    * decreased "T1Min3" and "T1Max3" to 100/100 from 250/250 (defense vs missile decreased to 100 from 250)
    * deleted all stats from "T1Code4" through "T1Max4" and moved the other stats over (removed 22 vitality)
    * decreased new "T1Min4" and "T1Max4" to 15/20 from 25/35 (faster cast rate decreased to 15-20% from 25-35%)
    * decreased new "T1Min6" and T1Max6" to 1/1 from 2/2 (all skills decreased to 1 from 2)

  * ~~Splendor~~ (see patch 1.01)
    * ~~changed "*RunesUsed" to EthDol from EthLum~~
    * ~~changed "Rune2" to r14 from r17 (changed second rune to Dol from Lum)~~
    * ~~increased "T1Min6" and "T1Max6" to 15/15 from 10/10 (faster cast rate increased to 15% from 10%)~~

  * Stealth
    * deleted all stats from "T1Code2" through "T1Max2" and moved the other stats over (removed 6 dexterity)
    * ~~decreased new "T1Min3" and "T1Max3" to 10/10 from 25/25 (faster run/walk decreased to 10% from 25%)~~ (see patch 1.03)
    * ~~decreased "T1Min4" and "T1Max4" to 10/10 from 25/25 (faster cast rate decreased to 10% from 25%)~~ (see patch 1.03)
    * deleted all stats from "T1Min6" through "T1Max6" (removed faster hit recovery)

  * Steel
    * added hamm to "itype4"
    * added club to "itype5"

  * Treachery
    * increased "T1Min2" to 12 from 5 and decreased "T1Max2" to 3 from 15 (Fade when struck proc chance increased to 12% from 5%, level decreased to 3 from 15)

  * Valor
    * new body armor runeword added to DMMod
    * set "complete" to 1 (allows Valor to be created)
    * added DMMod 1.0 to "*Patch Release"
    * added tors to "itype1" (allows Valor to be created in body armor)
    * ~~added TalIth to "*RunesUsed", added r07 and r06 to "Rune1" and "Rune2" (first rune is Tal rune, second rune is Ith rune)~~ (see patch 1.03)
    * ~~added red-dmg to "T1Code1", set "T1Min1" and "T1Max1" to 1/1 (damage reduced by 1)~~ (see patch 1.03)
    * added stam to "T1Code2", set "T1Min2" and "T1Max2" to 25/25 (25 stamina)
    * ~~added move2 to "T1Code3", set "T1Min3" and "T1Max3" to 10/10 (10% faster run/walk)~~ (see patch 1.03)
    * ~~added swing2 to "T1Code4", set "T1Min4" and "T1Max4" to 10/10 (10% increased attack speed)~~ (see patch 1.03)

  * Venom
    * changed "*RunesUsed" to TalMal from TalDolMal
    * deleted stats from "Rune2" and moved the other stats over (removed Dol rune)
    * decreased "T1Param1" to 75 from 125, increased "T1Min1" and "T1Max1" to 1521/1521 from 312/312 (poison length decreased to 75 frames/3 seconds from 125 frames/5 seconds, poison bitrate increased to 1521 from 312 [poison damage increased to 654 over 4 seconds from 273 over 6 seconds when averaged with Tal rune])
    * changed "T1Param3" to 278 from 83, decreased "T1Min3" to 7 from 27, increased "T1Max3" to 17 from 15 (Poison Explosion charges changed to Venom, charge count decreased to 7 from 27, level increased to 17 from 15)
    * changed "T1Code4" to pierce-pois from charged, deleted stats from "T1Param4", decreased "T1Min4" and "T1Max4" to 12/16 from 11/13 (-12-16% enemy poison resistance instead of Poison Nova charges)
    * added swing2 to "T1Code6", set "T1Min6" and "T1Max6" to 25/25 (25% increased attack speed)

  * Wind
    * increased "T1Min2" and "T1Max2" to 65/65 from 40/40 (increased attack speed increased to 65% from 40%)
    * increased "T1Min3" and "T1Max3" to 25/25 from 20/20 (faster run/walk increased to 25% from 20%)
    * changed "T1Param6" to 258 from 240, decreased "T1Min6" and "T1Max6" to 16/6 from 127/13 (Twister charges changed to Burst of Speed, charge count decreased to 16 from 127, level decreased to 6 from 13)

  * Wrath
    * increased "T1Min3" and "T1Max3" to 71/330 from 41/240 (lightning damage increased to 71-330 from 41-240)
    * increased "T1Min4" and "T1Max4" to 133/177 from 85/120 (magic damage increased to 133-177 from 85-120)
    * increased "T1Max5" to 14 from 10 (Life Tap on striking level increased to 14 from 10)
    * increased "T1Max6" to 6 from 1 (Decrepify on striking level increased to 6 from 1)

  * Zephyr
    * increased "T1Min3" and "T1Max3" to 55/55 from 33/33 (enhanced damage increased to 55% from 33%)

  * Hustle (armor)
    * changed "*RunesUsed" to ShaelEldIo from ShaelKoEld
    * changed "Rune2" to r02 from r18 (changed second rune to Eld from Ko)
    * changed "Rune3" to r16 from r02 (changed third rune to Io from Eld)
    * ~~decreased "T1Min1" and "T1Max1" to 33/33 from 65/65 (faster run/walk decreased to 33% from 65%)~~ (see patch 1.03)
    * ~~decreased "T1Min3" and "T1Max3" to 25/25 from 40/40 (increased attack speed decreased to 25% from 40%)~~ (see patch 1.03)
    * ~~decreased "T1Min5" and "T1Max5" to 2/2 from 6/6 (Evade oskill level decreased to 2 from 6)~~ (see patch 1.03)

  * Hustle (weapon)
    * changed "*RunesUsed" to ShaelEldIo from ShaelKoEld
    * changed "Rune2" to r02 from r18 (changed second rune to Eld from Ko)
    * changed "Rune3" to r16 from r02 (changed third rune to Io from Eld)
    * deleted all stats from "T1Code1" to "T1Max1" and moved the other stats over (removed chance to cast Burst of Speed on striking)
    * changed new "T1Code1" to move2 from swing2, increased "T1Min1" and "T1Max1" to 15/15 (15% faster run/walk instead of 10% increased attack speed)
    * decreased new "T1Min2" and "T1Max2" to 95/110 from 180/200 (enhanced damage decreased to 95-110% from 180-200%)
    * increased new "T1Min3" and "T1Max3" to 2/2 (Fanaticism aura level increased to 2 from 1)

  * Mosaic
    * changed "complete" to blank from 1 (prevents Mosaic from being created)

#### setitems.txt
  * all medium and heavy armor/shields have the "Medium Armor" and "Heavy Armor" bonuses added to their set stats (automagic.txt affixes don't apply to set/unique items)

  * Natalya's Odium
    * changed "add func" to 2 from blank (Natalya set now has item set bonuses)
    * Natalya's Totem
      * increased "min5" and "max5" to 6/6 from 3/3 (magic damage reduced increased to 6 from 3)
    * Natalya's Mark
      * increased "par4" to 150 from 100, increased "min4" and "max4" to 163/163 from 50/50 (cold length increased to 150 frames/6 seconds from 100 frames/4 seconds, cold damage increased to 163 from 50)
      * increased "min5" and "max5" to 225/225 from 12/17 (fire damage increased to 225 from 12-17)
      * added skilltab to "aprop1a", set "apar1a" to 20 and "amin1a" and "amax1a" to 1/1 (1 martial arts for 2 piece set bonus)
      * added deadly to "aprop2a", set "amin2a" and "amax2a" to 24/24 (24% chance of deadly strike for 3 piece set bonus)
    * Natalya's Shadow
      * increased "min1" and "max1" to 235/310 from 150/225 (defense increased to 235-310 from 150-225)
      * increased "par2" to 13 from 8 (life per level increased to 1.625 from 1)
      * increased "min5" and "max5" to 30/45 from 25/25 (poison resist increased to 30-45% from 25%)
      * added res-pois to "aprop1a", set "amin1a" and "amax1a" to 20/20 (poison resist 20% for 2 piece set bonus)
      * added extra-pois to "aprop2a", set "amin2a" and "amax2a" to 10/10 (10% poison skill damage for 3 piece set bonus)
    * Natalya's Soul
      * increased "par3" to 5 from 3 (heal stamina plus per level increased to 0.625% from 0.25%)
      * added move2 to "aprop1a", set "amin1a" and "amax1a" to 17/17 (17% faster run/walk for 2 piece set bonus)
      * added skilltab to "aprop2a", set "apar2a" to 20 and "amin2a" and "amax2a" to 1/1 (1 martial arts for 3 piece set bonus)
      * added crush to "aprop3a", set "amin3a" and "amax3a" to 30/30 (30% crushing blow for full set bonus)

  * Aldur's Watchtower
    * Aldur's Stony Gaze
      * changed "prop1" to ac% from ac, increased "min1" and "max1" to 100/100 from 90/90 (100% enhanced defense instead of 90 defense)
      * increased "min2" and "max2" to 27/27 from 17/17 (regenerate mana increased to 27% from 17%)
      * increased "amin2a" and "amax2a" to 20/20 from 15/15 (energy increased to 20 from 15 for 3 piece set bonus)
      * increased "amin3a" and "amax3a" to 25/25 from 15/15 (energy increased to 25 from 15 for full set bonus)
    * Aldur's Deception
      * increased "min1" and "max1" to 450/450 from 300/300 (defense increased to 450 from 300)
      * increased "amin2a" and "amax2a" to 20/20 from 15/15 (vitality increased to 20 from 15 for 3 piece set bonus)
      * increased "amin3a" and "amax3a" to 25/25 from 15/15 (vitality increased to 25 from 15 for full set bonus)
    * Aldur's Gauntlet (Aldur's Rhythm)
      * changed "prop1" to dmg% from dmg-norm, increased "min1" and "max1" to 200/200 from 40/62 (200% enhanced damage instead of adds 40-62 damage)
      * increased "amin2a" and "amax2a" to 20/20 from 15/15 (strength increased to 20 from 15 for 3 piece set bonus)
      * increased "amin3a" and "amax3a" to 25/25 from 15/15 (strength increased to 25 from 15 for full set bonus)
    * Aldur's Advance
      * increased "amin2a" and "amax2a" to 20/20 from 15/15 (dexterity increased to 20 from 15 for 3 piece set bonus)
      * increased "amin3a" and "amax3a" to 25/25 from 15/15 (dexterity increased to 25 from 15 for full set bonus)

  * Immortal King
    * Immortal King's Soul Cage
      * increased "min2" to 8 from 5 (Enchant when struck proc chance increased to 8% from 5%)
    * Immortal King's Pillar
      * changed "aprop4a" to nofreeze from half-freeze (cannot be frozen instead of half freeze duration for 5 piece set bonus)

  * Tal Rasha's Wrappings
    * Tal Rasha's Horadric Crest
      * added cast2 to "aprop2a", set "amin2a" and "amax2a" to 10/10 (10% faster cast rate for 3 piece set bonus)

  * Griswold's Legacy
    * Griswold's Valor
      * increased "min6" and "max6" to 20/20 from 5/5 (all resistances increased to 20% from 5%)
    * Griswold's Honor
      * decreased "min5" and "max5" to 30/30 from 45/45 (all resistances decreased to 30% from 45%)

  * Trang-Oul's Avatar
    * now uses necro casting frames instead of slow vampire casting frames
    * Trang-Oul's Guise
      * increased "min3" and "max3" to 75/75 from 20/20 (attacker takes damage increased to 75 from 20)
      * increased "min5" and "max5" to 11/11 from 5/5 (replenish life increased to 11 from 5)
    * Trang-Oul's Scales
      * increased "min2" and "max2" to 275/275 from 100/100 (defense vs missiles increased to 275 from 100)
    * Trang-Oul's Wing
      * changed "prop1" to ac% from ac, increased "min1" and "max1" to 170/170 from 125/125 (170% enhanced defense instead of 125 defense)
      * increased "amin3a" and "max3a" to 18/18 from 15/15 (replenish life increased to 18 from 15 for 4 piece set bonus)
    * Trang-Oul's Girth
      * increased "min2" and "max2" to 130/130 from 30/30 (stamina increased to 130 from 30)
      * increased "min3" and "max3" to 11/11 from 5/5 (replenish life increased to 11 from 5)

  * M'avina's Battle Hymn
    * M'avina's True Sight
      * increased "min2" and "max2" to 20/20 from 10/10 (replenish life increased to 20 from 10)
    * M'avina's Embrace
      * increased "min1" and "max1" to 16/11 from 10/3 (Glacial Spike when struck proc chance increased to 16% from 10%, level increased to 11 from 3)
    * M'avina's Caster
      * increased "min1" and "max1" to 233/233 from 188/188 (enhanced damage increased to 233% from 188%)
      * increased "min3" and "max3" to 13/13 from 1/1 (fires magic arrows level increased to 13 from 1)
      * increased "min4" and "max4" to 125/125 from 50/50 (attack rating increased to 125 from 50)
      * increased "amin2a" and "amax2a" to 13/22 from 10/15 (Nova on striking proc chance increased to 13% from 10%, level increased to 22 from 15)
      * added pierce-cold to "aprop4a", set "amin4a" and "amax4a" to 25/25 (-25% enemy cold resistance for full set bonus)

  * The Disciple
    * changed "add func" to 2 from blank (Disciple set now has item set bonuses)
    * Telling of Beads
      * increased "min4" and "max4" to 37/44 from 8/10 (attacker takes damage increased to 37-44 from 8-10)
      * added cast2 to "aprop2a", set "amin2a" and "amax2a" to 10/10 (10% faster cast rate for 3 piece set bonus)
      * added allskills to "aprop3a", set "amin3a" and "amax3a" to 1/1 (1 all skills for 4 piece set bonus)
    * Laying of Hands
      * decreased "min4" and "max4" to 100/100 from 350/350 (damage to demons decreased to 100% from 350%)
      * increased "max5" to 14 from 3 (Holy Bolt on striking level increased to 14 from 3)
      * added dmg-demon to "aprop1a", set "amin1a" and "amax1a" to 100/100 (100% damage to demons for 2 piece set bonus)
      * added dmg-demon to "aprop3a", set "amin3a" and "amax3a" to 150/150 (150% damage to demons for 4 piece set bonus)
    * Rite of Passage
      * increased "min4" and "max4" to 55/80 from 15/25 (stamina increased to 55-80 from 15-25)
      * added nofreeze to "aprop3a", set "amin3a" and "amax3a" to 1/1 (cannot be frozen for 4 piece set bonus)
    * Spiritual Custodian (Dark Adherent)
      * changed "par3" to Frost Nova from 48, decreased "min3" to 17 from 25, increased "max3" to 5 from 3 (Frost Nova when struck instead of Nova, proc chance decreased to 17% from 25%, level increased to 5 from 3)
      * increased "min4" and "max4" to 1250/1750 from 125/175 (poison bitrate increased to 1250-1750 from 125-175 [poison damage increased to 240-340 over 2 seconds from 24-34 over 2 seconds)
      * added regen-mana to "aprop1a", set "amin1a" and "amax1a" to 18/18 (regenerate mana 18% for 2 piece set bonus)
    * Credendum
      * added regen-mana to "aprop2a", set "amin2a" and "amax2a" to 27/27 (regenerate mana 27% for 3 piece set bonus)
      * added cast2 to "aprop4a", set "amin4a" and "amax4a" to 15/15 (15% faster cast rate for full set bonus) 

  * Heaven's Brethren
    * Dangoon's Teaching
      * increased "par1" to 20 from 12 (maximum damage per level increased to 2.5 from 1.5)
      * increased "min4" and "max4" to 60/80 from 20/30 (fire damage increased to 60-80 from 20-30)
      * added dmg% to "prop5", set "min5" and "max5" to 50/50 (50% enhanced damage)
    * Heaven's Taebaek (Taebaek's Glory)
      * increased "min1" and "max1" to 200/200 from 50/50 (defense increased to 200 from 50)
      * increased "min3" and "max3" to 40/40 from 30/30 (lightning resist increased to 40% from 30%)
      * increased "min4" and "max4" to 120/120 from 30/30 (attacker takes damage increased to 120 from 30)
      * increased "min6" and "max6" to 45/45 from 25/25 (increased chance to block increased to 45% from 25%)
      * increased "min7" and "max7" to 40/40 from 30/30 (faster block rate increased to 40% from 30%)
      * added res-cold to "prop9", set "min9" and "max9" to 25/25 (cold resist 25%)
    * Haemosu's Adament (Haemosu's Adamant)
      * increased "min2" and "max2" to 275/275 from 35/35 (defense vs missile increased to 275 from 35)
      * increased "min4" and "max4" to 325/325 from 40/40 (defense vs melee increased to 325 from 40)
    * Ondal's Almighty
      * increased "min1" and "max1" to 100/100 from 50/50 (defense increased to 100 from 50)
      * increased "min4" and "max4" to 20/20 from 10/10 (strength increased to 20 from 10)

  * Hwanin's Majesty
    * Hwanin's Refuge
      * increased "min4" to 13 from 10 (Static Field when struck proc chance increased to 13% from 10%)
    * Hwanin's Seal (Hwanin's Blessing)
      * increased "min1" and "max1" to 5/55 from 3/33 (lightning damage increased to 5-55 from 3-33)
    * Hwanin's Justice
      * increased "min3" and "max3" to 12/6 from 10/3 (Ice Blast on striking proc chance increased to 12% from 10%, level increased to 6 from 3)
      * increased "min6" and "max6" to 25/140 from 5/25 (lightning damage increased to 25-140 from 5-25)

  * Sazabi's Grand Tribute
    * Sazabi's Cobalt Redeemer
      * increased "min1" and "max1" to 200/200 from 150/150 (enhanced damage increased to 200% from 150%)
      * increased "min2" and "max2" to 75/95 from 25/35 (cold damage increased to 75-95 from 25-35)
      * decreased "min4" and "max4" to 268/268 from 318/318 (damage to demons decreased to 268% from 318%)

  * Bul-Kathos' Children
    * Bul-Katho's Sacred Charge
      * increased "min4" and "max4" to 275/275 from 200/200 (enhanced damage increased to 275% from 200%)
    * Bul-Kathos' Tribal Guardian
      * increased "min2" and "max2" to 1536/1536 from 255/255 (poison bitrate increased to 1536 from 255 [poison damage increased to 300 over 2 seconds from 50 over 2 seconds)
      * increased "min5" and "max5" to 275/275 from 200/200 (enhanced damage increased to 275% from 200%)

  * Cow King's Leathers
    * Cow King's Horns
      * increased "min4" and "max4" to 30/30 from 10/10 (attacker takes damage increased to 30 from 10)

  * Naj's Ancient Vestige
    * Naj's Puzzler
      * increased "min2" and "max2" to 180/180 from 150/150 (enhanced damage increased to 180% from 150%)
      * increased "min4" and "max4" to 35/35 from 30/30 (faster cast rate increased to 35% from 30%)
      * increased "min5" and "max5" to 23/319 from 6/45 (lightning damage increased to 23-319 from 6-45)
    * Naj's Circlet
      * added cast2 to "prop6", set "min6" and "max6" to 10/10 (10% faster cast rate)

  * Sander's Folly
    * McAuley's Paragon (Sander's Paragon)
      * increased "min2" and "max2" to 18/18 from 8/8 (attacker takes damage increased to 18 from 8)
    * McAuley's Taboo (Sander's Taboo)
      * increased "min4" and "max4" to 90/108 from 30/36 (poison bitrate increased to 90-108 from 30-36 [poison damage increased to 27-33 over 3 seconds from 9-11 over 3 seconds])

#### sets.txt

  * Aldur's Watchtower
    * copied and deleted all stats from "PCode4a" through "PMax4a" and pasted them to "FCode8" through "FMax8" (10% life steal for full set bonus now works)
    * increased "FMin3" and "FMax3" to 400/400 from 150/150 (defense increased to 400 from 150 for full set bonus)

  * Tal Rasha's Wrappings
    * increased "PMin2a" and "PMax2a" to 14/14 from 10/10 (replenish life increased to 14 from 10 for 2 piece set bonus)

  * Trang-Oul's Avatar
    * increased "PMin2b" and "PMax2b" to 22/22 from 18/18 (Fire Ball level increased to 22 from 18 for 2 piece set bonus)
    * increased "PMin3a" and "PMin3b" to 20/20 from 15/15 (regenerate mana increased to 20% from 15% for 3 piece set bonus)
    * increased "PMin3b" and "PMax3b" to 17/17 from 13/13 (Fire Wall level increased to 17 from 13 for 3 piece set bonus)
    * increased "PMin4a" and "PMax4a" to 25/25 from 15/15 (regenerate mana increased to 25% from 15% for 4 piece set bonus)
    * increased "PMin4b" and "PMax4b" to 14/14 from 10/10 (Meteor level increased to 14 from 10 for 4 piece set bonus)
    * increased "FMin6" and "FMax6" to 30/30 from 15/15 (regenerate mana increased to 30% from 15% for full set bonus)
    * increased "FMin7" and "FMax7" to 6/6 from 3/3 (Fire Mastery level increased to 6 from 3 for full set bonus)

  * M'avina's Battle Hymn
    * added att to "PCode4a", set "PMin4a" and "PMax4a" to 75/75 (75 attack rating for 4 piece set bonus)
    * increased "FMin3" and "FMax3" to 200/200 from 100/100 (defense increased to 200 from 100 for full set bonus)
    * increased "FMin4" and "FMax4" to 125/125 from 100/100 (attack rating increased to 125 from 100 for full set bonus)

  * The Disciple
    * increased "PMin3a" and "PMax3a" to 1500/1500 from 75/75 (poison bitrate increased to 1500 from 75 for 3 piece set bonus [poison damage increased to 440 over 3 seconds from 22 over 3 seconds])
    * copied and deleted all stats from "PCode5a" through "PMax5a" and pasted them to "FCode4" through "FMax4" (10 dexterity for full set bonus now works)
    * added addxp to "FCode5", set "FMin5" and "FMax5" to 10/10 (adds 10% to experience gained for full set bonus)
    * added ac to "FCode6", set "FMin6" and "FMax6" to 150/150 (150 defense for full set bonus)

  * Heaven's Brethren
    * increased "PParam3b" to 32 from 24 (fire damage per level increased to 4 from 3 for 3 piece set bonus)

  * Orphan's Call
    * increased "PMin3a" and "PMax3a" to 66/66 from 5/5 (attacker takes damage increased to 66 from 5 for 3 piece set bonus)
    * copied and deleted all stats from "PCode4a" through "PMax4a" and pasted them to "FCode7" through "FMax7" (100 defense for full set bonus now works)
    * increased "FMin5" and "FMax5" to 25/25 from 15/15 (all resistances increased to 25% from 15%)
    * added att to "FParam8", set "FMin8" and "FMax8" to 125/125 (125 attack rating for full set bonus)

  * Bul-Kathos' Children
    * increased "FMin1" and "FMax1" to 325/325 from 200/200 (fire damage increased to 325 from 200 for full set bonus)
    * increased "FMin3" and "FMax3" to 275/275 from 200/200 (attack rating increased to 275 from 200 for full set bonus)
    * increased "FMin4" and "FMax4" to 250/250 from 200/200 (defense increased to 250 from 200 for full set bonus)

  * Cow King's Leathers
    * increased "PMin2a" and "PMax2a" to 45/45 from 25/25 (poison resist increased to 45% from 25% for 2 piece set bonus)
    * increased "FMin1" and "FMax1" to 200/200 from 100/100 (stamina increased to 200 from 100 for full set bonus)
    * increased "FMin3" and "FMax3" to 250/250 from 100/100 (gold find increased to 250% from 100% for full set bonus)
    * increased "FMin4" and "FMax4" to 150/150 from 100/100 (magic find increased to 150% from 100% for full set bonus)

#### skilldesc.txt
  * slow missiles
    * copied and deleted all stats from "dsc2line3" through "dsc2calca4" and pasted them to "descline2" through "desccalca3" (moved ranged attacks slowed and physical damage received stat locations on Inner Sight's tooltip and also makes it show the next level preview stats)

  * frozen armor
    * changed "desccalca2" to ln56*(100+((skill('Glacial Spike'.blvl)+skill('Frost Nova'.blvl))* par8))/100 from ln56*(100+((skill('Shiver Armor'.blvl)+skill('Chilling Armor'.blvl))*par8))/100
    * changed "dsc3textb2" to skillname55 from skillname50 (changed freeze length synergy skill tooltip to Glacial Spike from Shiver Armor)
    * changed "dsc3textb4" to skillname44 from skillname60 (changed freeze length synergy skill tooltip to Frost Nova from Chilling Armor)

  * shiver armor
    * changed "dsc3textb2" to skillname44 from skillname40 (changed cold damage synergy skill tooltip to Frost Nova from Frozen Armor)
    * deleted all stats from "dsc3line4" through "dsc3calca4" and moved the other stats over (removed Chilling Armor

  * chilling armor
    * changed "dsc3textb2" to skillname39 from skillname40 (changed cold damage synergy skill tooltip to Ice Bolt from Frozen Armor)
    * changed "dsc3textb4" to skillname44 from skillname50 (changed cold damage synergy skill tooltip to Frost Nova from Shiver Armor)

  * iron maiden
    * added 74 to "dsc2line3", added StrSkill37 to "dsc2texta3", added par7 + (skill('Amplify Damage'.blvl))*par8 to "dsc2calca3" (added damage taken to Iron Maiden's tooltip)
    * added 40 to "dsc3line1", added Sksyn to "dsc3texta1", added skillname76 to "dsc3textb1", added 2 to "dsc3calca1" (added the green "receives bonuses from" synergy text)
    * added 76 to "dsc3line2", added StrSkillDamageTakenPerLevel to "dsc3texta2", added skillname66 to "dsc3textb2", added par8 to "dsc3calca2" (added Amplify Damage damage taken synergy to Iron Maiden's tooltip)

  * life tap
    * copied and deleted all stats from "dsc2line2" through "dsc2calca2" and pasted them to "descline3" through "desccalca3" (moved life returned duration on the tooltip)

  * decrepify
    * changed "dsc2calca4" to par5 from 0 (now properly shows damage taken on the tooltip)

  * revive
    * copied and deleted all stats from "dsc2line2" through "dsc2calcb2" and pasted them to "descline2" through "descalcb2" and moved the other stats over (moved duration location on the tooltip)
    * changed "desccalca2" to par3+skill('Revive'.blvl)*par4 from ln34
    * NOTE: There's an issue with using blvl in skilldesc.txt calcs, the ingame tooltip won't calculate the "next level" stats properly. This is only a tooltip bug, the stats will increase as expected.
    * deleted all stats from "dsc3line3" and "dsc3texta3" (removed Summon Resist synergy from tooltip because SR doesn't actually apply to Revives)

  * defiance
    * changed "desctexta2" to StrSkillDefensePassive from StrSkill21, changed "desccalca2" to (skill('Defiance'.blvl) < 1) ? par8 : skill('Defiance'.blvl) * par8 from ln34 (shows passive defense bonus)
    * added 74 to "descline3, StrSkillDefenseActive to "desctexta3", ln34 to "desccalca3" (shows active defense bonus)

  * double swing
    * set "HireableIconCel" to 29 (changed the Frenzy Act 5 merc skill icon to Double Swing from Taunt)

  * taunt
    * deleted all stats in "HireableIconCel" (removed Taunt from the Frenzy Act 5 merc skill list)

  * stun
    * deleted all stats from "dsc3line3" through "dsc3calca4" (removed Concentrate and War Cry synergies from the tooltip)

  * frenzy
    * copied and deleted all stats from "dsc2line2" through "dsc2calcb2", pasted them to "descline5" through "desccalcb5" and moved the other stats over (moved duration location on the tooltip)
    * changed "desccalca5" to par7+skill('Frenzy'.blvl)*2+skill('Increased Stamina'.blvl)*8 from par7+skill('Increased Stamina'.blvl)*10 (each hard point in Frenzy increases duration on the tooltip by 0.08 seconds, each hard point in Increased Stamina increases duration on tooltip by 0.32 seconds)
    * NOTE: There's an issue with using blvl in skilldesc.txt calcs, the ingame tooltip won't calculate the "next level" stats properly. This is only a tooltip bug, the stats will increase as expected.
    * deleted all stats from "dsc3line3" through "dsc3calca3" and moved the other stats over (removed Taunt synergy from the tooltip)
    * decreased new "dsc3calcb3" to 32 from 4 (Increased Stamina duration synergy on tooltip decreased to 0.32 seconds from 0.4 seconds)

  * berserk
    * changed "IconCel" to 54 from 52 (swapped skill icon with Natural Resistance)

  * natural resistance
    * changed "IconCel" to 52 from 54 (swapped skill icon with Berserk)

  * shape shifting (Lycanthropy)
    * added 74 to "descline3", ~~added StrSkill89 to "desctexta3", added ln56 to "desccalca3" (added run/walk speed to the tooltip)~~ (see patch 1.02)

#### skills.txt
  * Jab
    * added knif to "itypea2" (allows daggers/throwing knives to be used with Jab)

  * Multiple Shot
    * decreased "manashift" to 6 from 8 (changes the precision of the skill mana cost, 6 is a multipler of 64/256 or 25% while 8 is a multiplier of 256/256 or 100%)
    * increased "mana" to 12 from 4 (combined with "manashift" change the initial mana cost decreased to 3 from 4)
    * increased "lvlmana" to 3 from 1 (mana cost increase per level decreased to 0.75 from 1)

  * Power Strike
    * added knif to "itypea2"

  * Impale
    * added knif to "itypea2"
    * increased "Param2" to 40 from 25 (enhanced damage per level increased to 40% from 25%)

  * Charged Strike
    * added knif to "itypea2"

  * Fend
    * added knif to "itypea2"

  * Lightning Strike
    * added knif to "itypea2"

  * Frozen Armor
    * changed "calc1" to ln56*(100+((skill('Glacial Spike'.blvl)+skill('Frost Nova'.blvl))* par8))/100 from ln56*(100+((skill('Shiver Armor'.blvl)+skill('Chilling Armor'.blvl))*par8))/100 (freeze length synergy skills changed to Glacial Spike/Frost Nova from Shiver Armor/Chilling Armor)

  * Shiver Armor
    * increased "Param8" to 18 from 9 (cold damage synergy per level increased to 18% from 9%)
    * changed "EDmgSymPerCalc" to (skill('Frost Nova'.blvl))*par8 from (skill('Frozen Armor'.blvl)+skill('Chilling Armor'.blvl))*par8 (cold damage synergy skills changed to Frost Nova from Frozen Armor/Chilling Armor)

  * Chilling Armor
    * changed "EDmgSymPerCalc" to (skill('Ice Bolt'.blvl)+skill('Frost Nova'.blvl))*par8 from (skill('Frozen Armor'.blvl)+skill('Shiver Armor'.blvl))*par8 (cold damage synergy skills changed to Ice Bolt/Frost Nova from Frozen Armor/Shiver Armor)

  * Poison Dagger
    * increased "EMin" to 45 from 18 (minimum poison bitrate baseline increased to 90 from 36)
    * increased "EMinLev1" through "EMinLev5" to 30/48/65/75/86 from 10/15/20/23/26 (minimum poison bitrate increased to 60 from 20 at level 1-8, 96 from 30 at level 9-16, 130 from 80 at level 17-22, 150 from 92 at 23-28, and 172 from 104 at level 29+)
    * increased "EMax" to 96 from 40 (maximum poison bitrate baseline increased to 192 from 80)
    * increased "EMaxLev1" through "EMaxLev5" to 32/48/66/75/86 from 10/15/20/23/26 (maximum poison bitrate increased to 64 from 20 at level 1-8, 96 from 30 at level 9-16, 132 from 80 at level 17-22, 150 from 92 at 23-28, and 172 from 104 at level 29+)
    * decreased "ELen" to 20 from 50 (poison length baseline decreased to 20 frames/0.8 seconds from 50 frames/2 seconds)
    * decreased "ELevLen1" through "ELevLen3" to 3 from 10 (poison length per level decreased to 3 frames/0.12 seconds from 10 frames/0.4 seconds)

  * Iron Maiden
    * added damageresist to "aurastat1", -par7 - (skill('Amplify Damage'.blvl) * par8) to "aurastatcalc1", set "Param7" to 33 and "Param8" to 2 (reduces physical resistance by 33% baseline and an additional 2% per hard point in Amplify Damage)
    * increased "Param6" to 35 from 25 (damage returned per level increased to 35% from 25%)

  * Life Tap
    * decreased "Param5" to 20 from 50 (life returned baseline decreased to 20% from 50%)
    * increased "Param6" to 1 from 0 (life returned per level increased to 1% from 0%)

  * Lower Resist
    * added magicresist to "aurastat5", set "aurastatcalc5" to -dm56 (reduces magic resist once again)

  * Bone Spirit
    * increased "EMinLev5" and "EMaxLev5" to 27/28 from 20/21 (magic damage per level at level 29+ increased to 27-28 from 20-21)

  * ~~Revive~~ (see patch 1.01)
    * ~~changed "calc2" to par3+skill('Revive'.blvl)*par4 from ln34 (Revive duration increases by 250 frames/10 seconds per hard point)~~
    * ~~decreased "Param3" to 4250 from 4500 (combined with "Param4" change the base duration remains 4500 frames/180 seconds)~~
    * ~~increased "Param4" to 250 from 0 (Revive duration increases by 250 frames/10 seconds per hard point)~~

  * Thorns
    * increased "Param4" to 45 from 40 (damage returned per level increased to 45% from 40%)

  * Defiance
    * added ironskin to "passivestate", skill_armor_percent to "passivestat1", skill('Defiance'.blvl) * par8 to "passivecalc1" (Defiance now passively gives 5% skill enhanced defense per hard point)
    * set "Param8" to 5, set "*Param8 Description" to Armor % passive synergy

  * Vengeance
    * decreased "manashift" to 5 from 6 (changes the precision of the skill mana cost, 5 is a multipler of 32/256 or 12.5% while 6 is a multiplier of 64/256 or 25%)
    * increased "mana" to 20 from 16 (combined with "manashift" change the initial mana cost decreased to 2.5 from 4 and mana cost increase per level decreased to 0.125 from 0.25)
    * increased "Param2" to 7 from 6 (elemental damage per level increased to 7% from 6% to compensate for Resist Fire/Cold/Lightning damage synergy reduction)
    * increased "Param7" to 3 from 2 (Salvation damage synergy increased to 3% per level from 2%)
    * decreased "Param8" to 8 from 10 (Resist Fire/Cold/Lightning damage synergies decreased to 8% per level from 10%)

  * Blessed Hammer
    * decreased "Param1" to 0 from 4 (Concentration damage synergy removed)
    * doubled all stats from "EMin" through "EMaxLev5" (doubled damage)

  * Holy Shield
    * changed "aurastate" to holyshieldclone from holyshield (no longer sets block rate to 2 frames and removes Holy Shield graphic, see states.txt)
    * added skill_armor_percent to "aurastat2" (makes the defense bonus work again, the above change to the "aurastate" caused it to stop working)
    * added item_fasterblockrate to "aurastat3", set "aurastatcalc3" to 16 (gives 16% faster block rate)
    * decreased "Param8" to 10 from 15 (Defiance defense synergy decreased to 10% per level from 15%)

  * Salvation
    * changed "srvdofunc" to 66 from 65
    * changed "aurastatcalc1", "aurastatcalc2", and "aurastatcalc3" to (stat('item_heavenlyburden'.accr)==1)?((stat('vitality'.base)==0)?(dm34/6):dm34):dm34 from dm34 (all resist bonus decreased to 1/6 when equipped by a mercenary with heavenly burden)
    * added velocitypercent to "passivestat1", set "passivecalc1" to (stat('item_heavenlyburden'.accr)==1)?((stat('vitality'.base)==0)?(0+par5):0):0 (-75% velocity when equipped by a mercenary with heavenly burden)
    * added attackrate to "passivestat2", set "passivecalc2" to (stat('item_heavenlyburden'.accr)==1)?((stat('vitality'.base)==0)?(0+par5):0):0 (-75% attack rate when equipped by a mercenary with heavenly burden)
    * added damageresist to "passivestat3", set "passivecalc3" to (stat('item_heavenlyburden'.accr)==1)?((stat('vitality'.base)==0)?(0+par6):0):0 (-100% PDR when equipped by a mercenary with heavenly burden)
    * NOTE: Salvation still works as normal for paladins using Salvation as their active aura and for anyone wearing Tyrael's Might on their character, only mercs wearing TM and Iron Golems made from TM are affected.
    * added fireresist to "passivestat4", set "passivecalc4" to dm34 (makes the fire resist bonus work again, the above change to "srvdofunc" caused it to stop working)
    * added coldresist to "passivestat5", set "passivecalc5" to dm34 (makes the cold resist bonus work again, the above change to "srvdofunc" caused it to stop working)
    * added lightresist to "passivestat6", set "passivecalc6" to dm34 (makes the lightning resist bonus work again, the above change to "srvdofunc" caused it to stop working)
    * set "Param5" to -75, set "*Param5 Description" to Slow %
    * set "Param6" to -100, set "*Param6 Description" to Damage Resistance %

  * ~~Bash~~ (see patch 1.02)
    * ~~increased "Param2" to 8 from 5 (enhanced damage per level increased to 8% from 5%)~~
    * ~~changed "ToHitCalc" to 15+lvl*7+skill('Concentrate'.blvl)* par7 from 15+lvl*5+skill('Concentrate'.blvl)*par7 (attack rating per level increased to 7% from 5%)~~

  * Double Swing
    * increased "LevToHit" to 8 from 5 (attack rating per level increased to 8% from 5%)

  * Stun
    * deleted all stats from "Param6" through "*Param7 Description" (removed War Cry stun length synergy and Concentrate attack rating synergy)
    * increased "Param1" to 63 from 30 (base stun length increased to 63 frames/2.52 seconds from 30 frames/1.2 seconds)
    * increased "Param2" to 10 from 5 (stun length per level increased to 10 frames/0.4 seconds from 5 frames/0.2 seconds)
    * set "ToHit" to 25 (25% base attack rating)
    * set "LevToHit" to 25 (25% attack rating per level)
    * deleted stats from "ToHitCalc" (removed Concentrate attack rating synergy)
    * increased "ELen" to 63 from 30 (base stun length increased to 63 frames/2.52 seconds from 30 frames/1.2 seconds)
    * increased "ELevLen1", "ELevLen2", and "ELevLen3" to 10/10/10 from 5/5/2 (stun length per level increased to 10 frames/0.4 seconds from 5 frames/0.2 seconds and removed the stun length per level reduction from level 17+)
    * deleted stats from "ELenSymPerCalc" (removed War Cry stun length synergy)

  * Frenzy
    * changed "auralencalc" to par7+skill('Frenzy'.blvl)*2+skill('Increased Stamina'.blvl)*8 from par7+skill('Increased Stamina'.blvl)*10 (now gains 2 frames/0.08 second duration per hard point in Frenzy, Increased Stamina duration synergy decreased to 8 frames/0.32 seconds from 10 frames/0.4 seconds)
    * changed "calc1" to ln12+skill('Double Swing'.blvl)*par8 from ln12+(skill('Double Swing'.blvl) + skill('Taunt'.blvl))*par8, increased "Param8" to 16 from 8 (removed Taunt synergy, doubled bonus from Double Swing synergy)
    * decreased "Param7" to 148 from 150 (combined with "auralencalc" change the base duration remains 6 seconds)
    * increased "LevToHit" to 9 from 7 (attack rating per level increased to 9% from 7%)

  * Whirlwind
    * increased "param2" to 6 from 5 (enhanced damage per level increased to 6% from 5%)
    * increased "LevToHit" to 7 from 5 (attack rating per level increased to 7% from 5%)

  * War Cry
    * decreased "lvlmana" to 2 from 3 (mana increase per level decreased to 0.5 from 0.75)

  * ~~Wearwolf (Werewolf)~~ (see patch 1.02)
    * ~~added velocitypercent to "aurastat5", set "aurastatcalc5" to skill('Shape Shifting'.ln56) (Lycanthropy gives 2% velocity per level to Werewolf)~~

  * ~~Shape Shifting (Lycanthropy)~~ (see patch 1.02)
    * ~~set "Param5" to 2, set "*Param5 Description" to Velocity % per level (Lycanthropy gives 2% velocity baseline to Werewolf and Werebear)~~
    * ~~set "Param6" to 2, set "*Param6 Description" to Velocity % per level (Lycanthropy gives 2% additional velocity per level to Werewolf/Werebear, level 20 would give 2 + (2 * 19) = 40% velocity for example)~~

  * ~~Wearbear (Werebear)~~ (see patch 1.02)
    * ~~added velocitypercent to "aurastat5", set "aurastatcalc5" to skill('Shape Shifting'.ln56) (Lycanthropy gives 2% velocity per level to Werebear)~~

  * Fury
    * set "AttackNoMana" to 1 (Fury now performs a regular attack when used while out of mana)
    * set "interrupt" to 0 (Fury is now uninterruptable)

#### states.txt
  * monsterset
    * changed "gfxclass" to 742 from 135 (this is part of a change to allow Trang vampires to use necro casting frames instead of slow vampire casting frames)

  * holyshieldclone
    * added a new entry for "holyshieldclone" (cloned row 103) (Holy Shield no longer sets block rate to 2 frames and removes Holy Shield graphic)

#### treasureclassex.txt
  * BaalQSpecial
    * added new entry for "BaalQSpecial" (cloned row 861)
    * set "Picks" to -2 (forces two "picks"/drops)
    * set "NoDrop" to 0 (prevents the picks from selecting NoDrop)
    * added Arpaska's Medallion to "Item1", set "Prob1" to 1 (guarantees quest Hell Baal will drop an Arpaska's Medallion)
    * added Baalq (H) to "Item2", set "Prob2" to 1 (guarantees quest Hell Baal to drop his quest drop)

#### uniqueitems.txt
  * All medium and heavy armor/shields have the "Medium Armor" and "Heavy Armor" bonuses added to their unique stats (automagic.txt affixes don't apply to set/unique items)

  * Coldkill
    * increased "min2" and "max2" to 35/50 from 15/15 (cold resist increased to 35-50% from 15%)
-increased "min5" and "max5" to 15/11 from 10/10 (Ice Blast on striking proc chance increased to 15% from 10%, level increased to 11 from 10)
-increased "min6" to 12 from 10 (Frost Nova when struck proc chance increased to 12% from 10%)

  * Islestrike
    * changed "prop6" to ac from ac-miss, increased "min6" and "max6" to 125/150 from 50/50 (defense instead of defense vs missile, increased to 125-150 from 50)
    * increased "min9" and "max9" to 2/3 from 1/1 (Maul level bonus increased to 2-3 from 1)
    * increased "min10" and "max10" to 2/3 from 1/1 (Fury level bonus increased to 2-3 from 1)

  * Pompeii's Wrath
    * increased "min1" and "max1" to 13/10 from 4/8 (Volcano on striking proc chance increased to 13% from 4%, level increased to 10 from 8)
    * increased "min3" to 79 from 35 (fire damage increased to 79-150 from 35-150)
    * added pierce-fire to "prop6", set "min6" and "max6" to 9/13 (-9-13% enemy fire resistance)
    * added hit-skill to "prop7", set "par7" to 87, set "min7" and "max7" to 17/1 (17% chance to cast level 1 Decrepify on striking)

  * Guardian Naga
    * increased "min1" to 9 from 5 (Poison Nova on striking proc chance increased to 9% from 5%)
    * increased "min2" and "max2" to 30/45 from 15/15 (attacker takes damage increased to 30-45 from 15)
    * increased "max3" to 45 from 30 (poison resist increased to 30-45% from 30%)
    * added extra-pois to "prop7", set "min7" and "max7" to 8/12 (8-12% poison skill damage)

  * Warlord's Trust
    * increased "min1" and "max1" to 250/250 from 75/75 (defense increased to 250 from 75)
    * increased "min2" and "max2" to 25/25 from 20/20 (replenish life increased to 25 from 20)
    * increased "par3" to 7 from 4 (vitality per level increased to 0.875 from 0.5)
    * increased "min4" and "max4" to 20/20 from 10/10 (all resistances increased to 20% from 10%)

  * Spellsteel
    * increased "min4" and "max4" to 20/20 from 10/10 (faster cast rate increased to 20% from 10%)
    * increased "min7" to 30 from 20 (Teleport charge count increased to 30 from 20)
    * increased "max8" to 8 from 3 (Decrepify charge level increased to 8 from 3)
    * changed "par9" to 116 from 101 (Conversion charges instead of Holy Bolt)
    * changed "par10" to 240 from 225 (Twister charges instead of Firestorm)
    * added swing2 to "prop11", set "min11" and "max11" to 15/15 (15% increased attack speed)
    * added allskills to "prop12", set "min12" and "max12" to 1/1 (1 all skills)

  * Stormrider
    * increased "min1" to 11 from 5 (Chain Lightning on striking proc chance increased to 11% from 5%)
    * increased "min2" to 13 from 10 (Charged Bolt on striking proc chance increased to 13% from 10%)
    * increased "max3" to 350 from 200 (lightning damage increased to 1-350 from 1-200)
    * changed "par8" to 42 from 38 (Static Field when struck instead of Charged Bolt)
    * added abs-ltng% to "prop9", set "min9" and "max9" to 15/20 (15-20% lightning absorb)
    * added move2 to "prop10", set "min10" and "max10" to 25/25 (25% faster run/walk)

  * Boneslayer Blade
    * increased "par1" to 20 from 10 (attack rating against undead per level increased to 10 from 5)
    * increased "prop2" to 40 from 20 (damage to undead per level increased to 5% from 2.5%)
    * increased "min3" and "max3" to 15/15 from 8/8 (strength increased to 15 from 8)
    * increased "min5" and "max5" to 50/70 from 35/35 (attack rating increased to 50-70% from 35%)
    * added dmg-mag to "prop9", set "min9" and "max9" to 95-125 (95-125 magic damage)

  * The Minataur (The Minotaur)
    * changed "prop1" to dmg-ac from stupidity, changed "min1" and "max1" to -90/-90 from 2/2 (-90 monster defense per hit instead of hit blinds target +2)
    * changed "prop2" to nofreeze from half-freeze (cannot be frozen instead of half freeze duration)
    * increased "max3" to 25 from 20 (strength increased to 15-25 from 15-20)
    * increased "min7" and "max7" to 200/300 from 140/200 (enhanced damage increased to 200-300% from 140-200%)

  * Carin Shard
    * increased "par1" to 12 from 10 (life per level increased to 1.5 from 1.25)
    * increased "min2" and "max2" to 15/15 from 10/10 (faster cast rate increased to 15% from 10%)
    * increased "par3" to 12 from 10 (mana per level increased to 1.5 from 1.25)
    * increased "min5" and "max5" to 13/13 from 5/5 (replenish life increased to 13 from 5)
    * added regen-mana to "prop8", set "min8" and "max8" to 25/25 (regenerate mana 25%)
    * added res-all to "prop9", set "min9" and "max9" to 20/20 (all resistances 20%)

  * Blackhand Key
    * changed "par1" to 7 from 6 (poison and bone skills instead of curses)

  * Dark Clan Crusher
    * increased "min5" and "max5" to 35/50 from 20/25 (attack rating increased to 35-50% from 20-25%)
    * added crush to "prop7", set "min7" and "max7" to 35/35 (35% crushing blow)

  * Zakarum's Hand
    * increased "min5" to 9 from 6 (Blizzard on striking proc chance increased to 9% from 6%)
    * increased "min8" and "max8" to 3/4 from 2/2 (Holy Freeze level increased to 3-4 from 2)
    * increased "min9" and "max9" to 3/4 from 2/2 (Holy Shock level increased to 3-4 from 2)

  * The Fetid Sprinkler
    * increased "min2" to 8 from 5 (Decrepify on striking proc chance increased to 8% from 5%)
    * changed "par3" to 91 from 81, decreased "min3" to 8 from 10 (Lower Resist on striking instead of Confuse, proc chance decreased to 8% from 10%)

  * Hand of Blessed Light
    * increased "min10" to 10 from 5 (Fist of the Heavens on striking proc chance increased to 10% from 5%)

  * Sureshrill Frost
    * increased "min4" and "max4" to 10/15 from 5/10 (adds damage increased to 10-15 from 5-10)
    * changed "prop6" to hit-skill from charged, changed "par6" to 44 from 64, changed "min6" and "max6" to 12/5 from 50/9 (12% chance to cast level 5 Frost Nova on striking instead of 50 level 9 Frozen Orb charges)
    * added pierce-cold to "prop7", set "min7" and "max7" to 8/12 (-8-12% enemy cold resistance)

  * Moonfall
    * increased "min1" to 10 from 5 (Meteor on striking proc chance increased to 10% from 5%)
    * increased "min2" and "min3" to 85/130 from 55/115 (fire damage increased to 85-130 from 55-115)
    * changed "prop6" to res-fire from charged, changed "min1" and "min2" to 25/30 from 60/11 (fire resist 25-30% instead of 60 level 11 Meteor charges)
    * added red-dmg% to "prop8", set "min8" and "max8" to 9/12 (physical damage reduced [PDR] by 9-12%)

  * Baezil's Vortex
    * increased "min1" and "max1" to 12/11 from 5/8 (Nova on striking proc chance increased to 12% from 5%, level increased to 11 from 8)
    * increased "max2" to 235 from 150 (lightning damage increased to 1-235 from 1-150)
    * changed "prop7" to hit-skill from charged, changed "par7" to 86 from 48, changed "min7" and "max7" to 8/3 from 80/15 (8% chance to cast level 3 Attract on striking instead of 80 level 15 Nova charges)

  * Earthshaker
    * increased "min1" to 12 from 5 (Fissure on striking proc chance increased to 12% from 5%)
    * increased "min7" and "max7" to 112/112 from 50/50 (durability bonus increased to 112 from 50)
    * added cast2 to "prop8", set "min8" and "max8" to 15/15 (15% faster cast rate)

  * Bloodtree Stump
    * increased "min7" and "max7" to 90/90 from 40/40 (durability bonus increased to 90 from 40)
    * added openwounds to "prop8", set "min8" and "max8" to 20/20 (20% chance of open wounds)

  * The Gavel of Pain
    * increased "min1" and "max1" to 14/3 from 5/1 (Amplify Damage on striking proc chance increased to 14% from 5%, level increased to 3 from 1)
    * changed "prop2" to aura from gethit-skill, changed "par2" to Thorns from 76, changed "min2" and "max2" to 1/3 (level 1-3 Thorns aura when equipped instead of Iron Maiden when struck)
    * increased "max3" to 33 from 26 (attacker takes damage increased to 26-33 from 26)
    * increased "min7" to 5 from 3 (AD charge count increased to 5 from 3)

  * Bloodletter
    * increased "min9" and "max9" to 68/68 from 30/30 (durability bonus increased to 68 from 30)
    * added openwounds to "prop10", set "min10" and "max10" to 10/15 (10-15% chance of open wounds)

  * Coldsteel Eye
    * increased "min4" and "max4" to 113/113 from 50/50 (durability bonus increased to 113 from 50)

  * Hexfire
    * added sock to "prop8", set "par8" to 1 (1 socket)

  * Blade of Ali Baba
    * added dmg-min to "prop7", set "min7" and "max7" to 40/40 (40 minimum damage)

  * Ginther's Rift
    * increased "min4" and "max4" to 90/90 from 40/40 (durability bonus increased to 90 from 40)

  * Plague Bearer
    * increased "max1" to 6 from 4 (Poison Nova on striking level increased to 6 from 4)
    * added pierce-pois to "prop7", set "min7" and "max7" to 6/9 (-6-9% enemy poison resistance)
    * added ease to "prop8", set "min8" and "max8" to -15/-15 (requirements -15%)

  * The Atlantian (The Atlantean)
    * increased "min1" and "max1" to 225/225 from 100/100 (durability bonus increased to 225 from 100)
    * increased "max2" to 100 from 75 (defense increased to 75-100 from 75)

  * Bing Sz Wang
    * increased "min5" and "max5" to 8/7 from 5/3 (Frozen Orb on striking proc chance increased to 8% from 5%, level increased to 7 from 3)
    * added swing2 to "prop7", set "min7" and "max7" to 10/10 (10% increased attack speed)
    * added sock to "prop8", set "par8" to 1 (1 socket)

  * The Vile Husk
    * increased "min1" and "max2" to 11/3 from 6/1 (Amplify Damage on striking proc chance increased to 11% from 6%, level increased to 3 from 1)

  * Cloudcrack
    * increased "min1" and "max1" to 12/10 from 6/7 (Fist of the Heavens on striking proc chance increased to 12% from 6%, level increased to 10 from 7)
    * increased "max2" to 320 from 240 (lightning damage increased to 1-320 from 1-240)
    * changed "prop3" to ac% from ac, changed "min3" and "max3" to 30/40 from 30/30 (30-40% enhanced defense instead of 30 defense)
    * increased "min7" and "max7" to 65/65 from 15/15 (attacker takes lightning damage increased to 65 from 15)
    * added pierce-ltng to "prop10", set "min10" and "max10" to 12/17 (-12-17% enemy lightning resistance)

  * Todesfaelle Flamme
    * increased "min1" and "max1" to 175/225 from 50/200 (fire damage increased to 175-225 from 50-200)
    * increased "min2" and "max2" to 50/50 from 40/40 (fire resist increased to 50% from 40%)
    * increased "min3" and "max3" to 15/15 from 10/10 (fire absorb increased to 15 from 10)
    * increased "min4" and "max4" to 15/11 from 10/6 (Fire Ball on attack proc chance increased to 15% from 10%, level increased to 11 from 6)
    * increased "min5" and "max5" to 190/230 from 120/160 (enhanced damage increased to 190-230% from 120-160%)
    * changed "prop7" to hit-skill from charged, changed "min7" and "max7" to 13/3 from 20/10 (13% chance to cast level 3 Fire Wall on striking instead of 20 level 10 Fire Wall charges)
    * added deadly to "prop8", set "min8" and "max8" to 15/20 (15-20% chance of deadly strike)

  * Swordguard
    * increased "min3" and "max3" to 15/25 from 10/20 (all resistances increased to 15-25% from 10-20%)
    * increased "min4" and "max4" to 250/250 from 100/100 (defense vs missile increased to 250 from 100)
    * increased "min7" and "max7" to 350/350 from 200/200 (defense vs melee increased to 350 from 200)
    * added block2 to "prop10", set "min10" and "max10" to 20/20 (20% faster block rate)
    * added ac% to "prop11", set "min11" and "max11" to 50/70 (50-70% enhanced defense)

  * Heart Carver
    * decreased "min5" and "max5" to 3/3 from 4/4 (Find Potion skill level decreased to 3 from 4)
    * added oskill to "prop8", set "par8" to Find Potion, set "min8" and "max8" to 1/1 (level 1 Find Potion oskill [+3 FP skill level increases it to 4 total])
    * added openwounds to "prop9", set "min9" and "max9" to 60/60 (60% chance of open wounds)

  * Blackbog's Sharp
    * changed "prop3" to dmg% from dmg-norm, changed "min3" and "max3" to 100/100 from 15/45 (100% enhanced damage instead of adds 15-45 damage)
    * added pierce-pois to "prop9", set "min9" and "max9" to 5/10 (-5-10% enemy poison resistance)

  * Stormspike
    * increased "max1" to 200 from 120 (lightning damage increased to 1-200 from 1-120)
    * increased "min2" and "max2" to 50/50 from 20/20 (attacker takes lightning damage increased to 50 from 20)
    * changed "par3" to 49 from 38, increased "max3" to 17 from 3 (Lightning instead of Charged Bolt when struck, level increased to 17 from 3)
    * increased "par5" to 11 from 8 (lightning resist per level increased to 1.375 from 1)
    * added sock to "prop6", set "min6" and "max6" to 1/2 (1-2 sockets)
    * added pierce-ltng to "prop7", set "min7" and "max7" to -8/-11 (-8-11% enemy lightning resistance)

  * The Impaler
    * increased "min2" and "max2" to 200/200 from 150/150 (attack rating increased to 200 from 150)
    * added skilltab to "prop9", set "par9" to 2, set "min9" and "max9" to 2/2 (2 to javelin and spear skills)
    * added indestruct to "prop10", set "min10" and "max10" to 1/1 (indestructible)

  * Kelpie Snare
    * increased "par3" to 12 from 10 (life per level increased to 1.5 from 1.25)
    * increased "max5" to 15 from 10 (strength increased to 10-15 from 10)
    * added move2 to "prop7", set "min7" and "max7" to 20/30 (20-30% faster run/walk)

  * Soulfeast Tine
    * increased "min2" and "max2" to 9/9 from 7/7 (life stolen per hit increased to 9% from 7%)
    * increased "min3" and "max3" to 9/9 from 7/7 (mana stolen per hit increased to 9% from 7%)
    * increased "min6" to 200 from 150 (attack rating increased to 200-250 from 150-250)
    * increased "min7" and "max7" to 34/34 from 15/15 (durability bonus increased to 34 from 15)

  * Hone Sundan
    * increased "par4" to 15 from 10 (repairs 1 durability every 6.66 seconds from 10 seconds)

  * Spire of Honor
    * increased "min1" and "max1" to 50/50 from 25/25 (attack rating increased to 50% from 25%)
    * increased "min3" and "max3" to 30/40 from 20/20 (replenish life increased to 30-40 from 20)
    * increased "min9" and "max9" to 35/50 from 25/25 (enhanced defense increased to 35-50% from 25%)
    * added dmg-und/lvl to "prop10", set "par10" to 6 (0.75% damage to undead per level)

  * Blackleach Blade
    * increased "min2" and "max2" to 18/8 from 5/5 (Weaken on striking proc chance increased to 18% from 5%, level increased to 8 from 5)
    * increased "max4" to 12 from 8 (life stolen per hit increased to 8-12% from 8%)
    * increased "min6" and "max6" to 120/149 from 100/140 (enhanced damage increased to 120-149% from 100-140%)
    * added manasteal to "prop7", set "min7" and "max7" to 1/2 (1-2% mana stolen per hit)

  * Athena's Wrath
    * increased "min1" to 3 from 1 (druid skills increased to 3 from 1-3)
    * increased "max2" to 25 from 15 (dexterity increased to 15-25 from 15)
    * increased "par4" to 12 from 8 (life per level increased to 1.5 from 1)

  * Husoldal Evo
    * increased "min1" and "max1" to 21/27 from 20/20 (replenish life increased to 21-27 from 20)
    * added rep-dur to "prop7", set "par7" to 8 (repairs 1 durability in 12.5 seconds)

  * Grim's Burning Dead
    * increased "min4" and "max4" to 30/40 from 8/8 (attacker takes damage increased to 30-40 from 8)
    * increased "min8" and "max8" to 25/40 from 20/20 (enhanced defense increased to 25-40% from 20%)
    * added fireskill to "prop10", set "min10" and "max10" to 1/1 (1 to fire skills)
    * added pierce-fire to "prop11", set "min11" and "max11" to 13/16 (-13-16% enemy fire resistance)

  * Razorswitch
    * increased "min2" and "max2" to 50/66 from 15/15 (attacker takes damage increased to 50-66 from 15)

  * Ribcracker
    * increased "min9" and "max9" to 225/225 from 100/100 (durability bonus increased to 225 from 100)

  * Chromatic Ire
    * increased "min2" to 25 from 20 (all resistances increased to 25-40% from 20-40%)
    * increased "min4" and "max4" to 69/69 from 20/20 (attacker takes lightning damage increased to 69 from 20, noice)
    * changed "prop6" to extra-fire from skill, changed "par6" to blank from 61, changed "min6" and "max6" to 7/12 from 1/1 (7-12% to fire skill damage instead of level 1 Fire Mastery)
    * changed "prop7" to extra-ltng from skill, changed "par7" to blank from 63, changed "min7" and "max7" to 7/12 from 1/1 (12-15% to lightning skill damage instead of level 1 Lightning Mastery)
    * changed "prop8" to pierce-cold from skill, changed "par8" to blank from 65, changed "min8" and "max8" to 7/12 from 1/1 (-7-12% enemy cold resistance instead of level 1 Cold Mastery)
    * added dmg% to "prop9", set "min9" and "max9" to 100/150 (100-150% enhanced damage)

  * Warpspear
    * changed "prop1" to sock from sorc, changed "max1" to 4 from 3 (3-4 sockets instead of 3 to sorceress skills)
    * changed "prop2" to cast3, changed "min2" and "max2" to 80/80 from 1/1 (80% faster cast rate instead of ignore target's defense)
    * increased "min3" and "max3" to 8/8 from 3/3 (Teleport level increased to 8 from 3)
    * increased "min4" and "max4" to 6/6 from 3/3 (Telekinesis level increased to 6 from 3)
    * increased "min5" and "max5" to 6/6 from 3/3 (Energy Shield level increased to 6 from 3)

  * Skullcollector (Skull Collector)
    * increased "min1" and "max1" to 25/25 from 20/20 (maximum mana increased to 25% from 20%)
    * increased "par4" to 12 from 8 (magic find per level increased to 1.5 from 1)
    * added life-kill to "prop5", set "min5" and "max5" to 5/10 (5-10 to life after each kill)

  * Skystrike
    * increased "min2" and "max2" to 200/200 from 100/100 (attack rating increased to 200 from 100)
    * increased "min3" and "max3" to 15/15 from 10/10 (energy increased to 15 from 10)
    * increased "min6" to 8 from 2 (Meteor on striking proc chance increased to 8% from 2%)
    * added res-fire to "prop8", set "min8" and "max8" to 15/20 (fire resist 15-20%)
    * added res-ltng to "prop9", set "min9" and "max9" to 15/20 (lightning resist 15-20%)

  * Endlesshail
    * increased "max1" to 50 from 35 (cold resist increased to 35-50% from 35%)
    * changed "prop3" to ac from ac-miss (defense instead of defense vs missile)
    * increased "par6" to 100 from 75, increased "min6" and "max6" to 20/50 from 15/30 (cold length increased to 100 frames/4 seconds from 75 frames/3 seconds, cold damage increased to 20-50 from 15-30)
    * added hit-skill to "par7", set "par7" to 59, set "min7" and "max7" to 12/3 (12% chance to cast level 3 Blizzard on striking)

  * Whichwild String (Witchwild String)
    * increased "min1" to 7 from 2 (Amplify Damage on striking proc chance increased to 7% from 2%)

  * Cliffkiller
    * added skill to "prop8", set "par8" to 13, set "min8" and "max8" to 2/3 (2-3 to Dodge)
    * added skill to "prop8", set "par8" to 18, set "min8" and "max8" to 2/3 (2-3 to Avoid)
    * added skill to "prop8", set "par8" to 29, set "min8" and "max8" to 2/3 (2-3 to Evade)

  * Magewrath
    * increased "min3" and "max3" to 5/5 from 3/3 (Guided Arrow level increased to 5 from 3)
    * added dmg-mag to "prop10", set "min10" and "max10" to 35/80 (adds 35-80 magic damage)

  * Godstrike Arch (Goldstrike Arch)
    * increased "min5" to 9 from 5 (Fist of the Heavens on striking proc chance increased to 9% from 5%)
    * increased "min7" and "max7" to 18/18 from 12/12 (replenish life increased to 18 from 12)

  * Langer Briser
    * increased "min3" to 40 from 30 (magic find increased to 40-60% from 30-60%)
    * increased min5" and "max5" to 20/35 from 10/30 (maximum damage increased to 20-35 from 10-30)
    * added sock to "prop8", set "par8" to 1 (1 socket)

  * Pus Spiter (Pus Spitter)
    * decreased "par1" to 25 from 200, increased "min1" and "max1" to 2047 from 192 (poison length decreased to 25 frames/1 second from 200 frames/8 seconds, poison bitrate increased to 2047 from 192 [poison damage increased to 200 over 1 second from 150 over 8 seconds])
    * changed "prop2" to pierce-pois from hit-skill, changed "par2" to blank from 91, increased "min2" and "max2" to 12/15 from 4/1 (-12-15% enemy poison resistance instead of Lower Resist on striking)
    * changed "prop5" to dmg-ac from gethit-skill, changed "par5" to blank from 92, increased "min5" and "max5" to -125/-125 from 9/6 (-125 monster defense per hit instead of Poison Nova when struck)
    * increased "min6" and "max6" to 15/15 from 10/10 (increased attack speed increased to 15% from 10%)
    * changed "prop8" to att%/lvl from att/lvl, decreased "par8" to 3 from 10 (1.5% attack rating per level instead of 5 attack rating per level)
    * added pierce to "prop9", set "min9" and "max9" to 50/50 (+50% piercing attack)

  * Peasent Crown (Peasant Crown)
    * increased "max1" to 25 from 20 (energy increased to 20-25 from 20)
    * increased "max2" to 25 from 20 (vitality increased to 20-25 from 20)
    * increased "min5" and "max5" to 9/14 from 6/12 (replenish life increased to 9-14 from 6-12)

  * Darksight Helm
    * increased "par2" to 20 from 16 (defense per level increased to 2.5 from 2)
    * increased "min5" and "max5" to 13/6 from 6/3 (Dim Vision when struck proc chance increased to 13% from 6%, level increased to 6 from 3)
    * increased "max6" to 8 from 5 (Cloak of Shadows charge level increased to 8 from 5)

  * Valkiry Wing (Valkyrie Wing)
    * added cast1 to "prop6", set "min6" and "max6" to 10/10 (10% faster cast rate)
    * added swing1 to "prop7", set "min7" and "max7" to 10/10 (10% increased attack speed)

  * Blackhorn's Face
    * increased "min1" and "max1" to 63/63 from 25/25 (attacker takes lightning damage increased to 63 from 25)
    * increased "max2" to 25 from 20 (slows target increased to 20-25% from 20%)
    * increased "max5" to 25 from 15 (lightning resist increased to 15-25% from 15%)

  * The Spirit Shroud
    * increased "max3" to 14 from 11 (magic damage reduced increased to 7-14 from 7-11)
    * increased "min4" and "max4" to 13/13 from 10/10 (replenish life increased to 13 from 10)
    * added res-cold to "prop6", set "min6" and "max6" to 15/25 (cold resist 15-25% )
    * added red-dmg% to "prop7", set "min7" and "max7" to 5/5 (5% PDR)

  * Skin of the Flayerd One (Skin of the Flayed One)
    * increased "min2" and "max2" to 20/30 from 15/25 (replenish life increased to 20-30 from 15-25)
    * increased "min6" and "max6" to 40/50 from 15/15 (attacker takes damage increased to 40-50 from 15)

  * Ironpelt (Iron Pelt)
    * increased "min2" and "max2" to 45/45 from 25/25 (life increased to 45 from 25)
    * added move3 to "prop7", set "min7" and "max7" to 25/25 (25% faster run/walk)
    * added oskill to "prop8", set "par8" to Iron Skin, set "min8" and "max8" to 1/1 (level 1 Iron Skin oskill)

  * Spiritforge (Spirit Forge)
    * increased "min3" and "max3" to 55/108 from 20/65 (fire damage increased to 55-108 from 20-65)
    * increased "min4" and "max4" to 15/25 from 5/5 (fire resist increased to 15-25% from 5%)
    * added res-mag to "prop9", set "min9" and "max9" to 10/10 (magic resist 10%)

  * Crow Caw
    * increased "min3" and "max3" to 20/20 from 15/15 (dexterity increased to 20 from 15)
    * enabled "prop6", increased "min6" and "max6" to 60/14 from 3/5 (enabled Raven charges, increased charge count to 60 from 3 and level to 14 from 5)
    * added att to "prop8", set "min8" and "max8" to 125/125 (125 to attack rating)

  * Shaftstop
    * increased "min1" and "max1" to 350/350 from 250/250 (defense vs missile increased to 350 from 250)

  * Toothrow
    * increased "min1" and "max1" to 60/80 from 20/40 (attacker takes damage increased to 60-80 from 20-40)
    * added dmg% to "prop9", set "min9" and "max9" to 20/30 (20-30% enhanced damage)

  * Atma's Wail
    * increased "min2" and "max2" to 26/26 from 10/10 (replenish life increased to 26 from 10)
    * changed "prop3" to mana from mana%, increased "min3" and "max3" to 100/100 from 15/15 (100 mana instead of 15% maximum mana)
    * increased "min8" and "max8" to 30/30 from 20/20 (magic find increased to 30% from 20%)
    * added rip to "prop10", set "min10" and "max10" to 1/1 (slain monsters rest in peace)

  * Black Hades
    * increased "min2" and "max2" to 250/350 from 200/250 (attack rating against demons increased to 250-350 from 200-250)
    * increased "min6" and "max6" to 50/80 from 30/60 (damage to demons increased to 50-80% from 30-60%)
    * added res-pois to "prop8", set "min8" and "max8" to 28/28 (poison resist 28%)

  * Corpsemourn
    * increased "max1" to 12 from 8 (strength increased to 8-12 from 8)
    * increased "max2" to 15 from 10 (vitality increased to 10-15 from 10)
    * increased "min4" and "max4" to 11/11 from 6/2 (Iron Maiden when struck proc chance increased to 11% from 6%, level increased to 11 from 2)
    * increased "min6" and "max6" to 34/97 from 12/36 (fire damage increased to 34-97 from 12-36)
    * increased "min7" to 50 from 40 (Corpse Explosion charge count increased to 50 from 40)

  * Que-Hegan's Wisdon (Que-Hegan's Wisdom)
    * increased "min1" and "max1" to 25/25 from 20/20 (faster cast rate increased to 25% from 20%)
    * increased "min2" and "max2" to 4/6 from 3/3 (mana after each kill increased to 4-6 from 3)
    * increased "min3" and "max3" to 7/11 from 6/10 (magic damage reduced increased to 7-11 from 6-10)
    * increased "min4" and "max4" to 20/25 from 15 (energy increased to 20-25 from 15)
    * added move2 to "prop8", set "min8" and "max8" to 20/20 (20% faster run/walk)

  * Visceratuant
    * increased "min5" and "max5" to 33/33 from 10/10 (attacker takes lightning damage increased to 33 from 10)

  * Stormchaser
    * increased "max1" to 226 from 60 (lightning damage increased to 1-226 from 1-60)
    * changed "prop3" to nofreeze from half-freeze (cannot be frozen instead of half freeze duration)
    * increased "max5" to 200 from 150 (attack rating increased to 150-200 from 150)
    * increased "min7" and "max7" to 40/40 from 10/10 (faster block rate increased to 40% from 10%)
    * increased "min8" and "max8" to 12/10 from 4/6 (Blizzard when struck proc chance increased to 12% from 4%, level increased to 10 from 6)
    * increased "min9" and "max9" to 12/9 from 4/5 (Tornado when struck proc chance increased to 12% from 4%, level increased to 9 from 5)
    * added res-cold to "prop11", set "min11" and "max11" to 14/19 (cold resist 14-19%)

  * Tiamat's Rebuke
    * increased "min6" to 9 from 5 (Frost Nova when struck proc chance increased to 9% from 5%)
    * increased "min7" and "max7" to 13/12 from 5/7 (Nova when struck proc chance increased to 13% from 5%, level increased to 12 from 7)
    * increased "min8" to 11 from 3 (Hydra when struck proc chance increased to 11% from 3%)

  * Kerke's Sanctuary (Gerke's Sanctuary)
    * increased "max3" to 21 from 15 (replenish life increased to 15-21 from 15)

  * Radimant's Sphere (Radament's Sphere)
    * decreased "par1" to 50 from 100, increased "min1" and "max1" to 768/768 from 204/204 (poison length decreased to 50 frames/2 seconds from 200 frames/8 seconds, poison bitrate increased to 768 from 204 [poison damage increased to 150 over 2 seconds from 80 over 4 seconds])
    * increased "min1" and "max1" to 14/11 from 5/5 (Poison Nova when struck proc chance increased to 14% from 5%, level increased to 11 from 5)
    * changed "prop7" to hit-skill, changed "min7" and "max7" to 17/9 from 40/6 (17% chance to cast level 9 Poison Explosion on striking instead of 40 level 6 Poison Explosion charges)
    * added pierce-pois to "prop10", set "min10" and "max10" to 5/7 (-5-7% enemy poison resistance)

  * Lance Guard
    * increased "min4" and "max4" to 93/93 from 47/47 (attacker takes damage increased to 93 from 47)

  * Venom Grip
    * increased "min2" and "max2" to 10/10 from 5/5 (maximum poison resist increased to 10% from 5%)
    * increased "min3" and "max3" to 461/461 from 153/153 (poison bitrate increased to 461 from 153 [poison damage increased to 180 over 4 seconds from 60 over 4 seconds])
    * increased "min4" and "max4" to 10/10 from 5/5 (crushing blow increased to 10% from 5%)

  * Gravepalm
    * increased "max1" to 20 from 10 (energy increased to 10-20 from 10)
    * increased "max2" to 15 from 10 (strength increased to 10-15 from 10)
    * increased "min3" to 130 from 100 (damage to undead increased to 130-200% from 100-200%)
    * increased "min4" and "max4" to 250-350 from 100-200 (attack rating against undead increased to 250-350 from 100-200)
    * added swing1 to "prop6", set "min6" and "max6" to 10/10 (10% increased attack speed)

  * Ghoulhide
    * increased "par2" to 20 from 16 (damage to undead per level increased to 2.5 from 2)

  * Lavagout (Lava Gout)
    * increased "min3" to 4 from 2 (Enchant on striking proc chance increased to 4% from 2%)
    * increased "min6" and "max6" to 26/73 from 13/46 (fire damage increased to 26-73 from 13-46)

  * Hellmouth
    * increased "min1" and "max1" to 92/179 from 15/72 (fire damage increased to 92-179 from 15-72)
    * increased "min5" and "max5" to 7/12 from 2/4 (Meteor on striking proc chance increased to 7% from 2%, level increased to 12 from 4)
    * increased "min6" and "max6" to 8/16 from 4/12 (Firestorm on striking proc chance increased to 8% from 4%, level increased to 16 from 12)
    * added nofreeze to "prop7", set "min1" and "max1" to 1 (cannot be frozen)

  * Infernostride
    * increased "min1" and "max1" to 39/61 from 12/33 (fire damage increased to 39-61 from 12-33)
    * increased "min2" and "max2" to 25/25 from 20/20 (faster run/walk increased to 25% from 20%)
    * increased "min9" to 9 from 5 (Blaze when struck proc chance increased to 9% from 5%)

  * Waterwalk
    * increased "min1" and "max1" to 200/200 from 100/100 (defense vs missile increased to 200 from 100)

  * Silkweave
    * increased "min3" and "max3" to 275/275 from 200/200 (defense vs missile increased to 275 from 200)

  * Wartraveler (War Traveler)
    * increased "min8" and "max8" to 25/40 from 5/10 (attacker takes damage increased to 25-40 from 5-10)

  * Gloomstrap (Gloom's Trap)
    * increased "min3" and "max3" to 8/8 from 5/5 (mana stolen per hit increased to 8% from 5%)
    * increased "max5" to 25 from 15 (vitality increased to 15-25 from 15)
    * increased "min6" and "max6" to 20/25 from 15/15 (regenerate mana increased to 20-25% from 15%)
    * added slow to "prop7", set "min7" and "max7" to 20/20 (slows target by 20%)

  * Snowclash
    * increased "min1" to 10 from 5 (Blizzard when struck proc chance increased to 10% from 5%)
    * increased "par4" to 125 from 75 and "min4" and "max4" to 28/47 from 13/21 (cold length increased to 125 frames/5 seconds from 75 frames/3 seconds, cold damage increased to 28-47 from 13-21)

  * Thudergod's Vigor (Thundergod's Vigor)
    * increased "min1" and "max1" to 8/9 from 5/7 (Fist of the Heavens when struck proc chance increased to 8% from 5%, level increased to 9 from 7)
    * increased "max2" to 188 from 50 (lightning damage increased to 1-188 from 1-50)

  * Veil of Steel
    * added deadly to "prop8", set "min8" and "max8" to 22/25 (22-25% chance of deadly strike)

  * The Gladiator's Bane
    * increased "min4" and "max4" to 70/70 from 20/20 (attacker takes damage increased to 70 from 20)

  * Arkaine's Valor
    * increased "min1" and "max1" to 170/190 from 150/180 (enhanced defense increased to 170-190% from 150-180%)
    * increased "par5" to 10 from 4 (vitality per level increased to 1.25 from 0.5)
    * added hp/lvl to "prop6", set "par6" to 20 (2.5 life per level)

  * Blackoak Shield
    * increased "min4" and "max4" to 14/8 from 4/5 (Weaken when struck proc chance increased to 14% from 4%, level increased to 8 from 5)
    * changed "prop8" to nofreeze from half-freeze (cannot be frozen instead of half freeze duration)
    * added block to "prop9", set "min9" and "max9" to 15/15 (15% increased chance to block)

  * Hellslayer
    * increased "par1" to 6 from 4 (strength per level increased to 0.75 from 0.5)
    * increased "par2" to 8 from 4 (vitality per level increased to 1 from 0.5)
    * increased "min4" and "max4" to 250/300 from 150/250 (fire damage increased to 250-300 from 150-250)
    * increased "max5" to 40 from 25 (life increased to 25-40 from 25)
    * increased "min7" to 13 from 10 (Fire Ball on attack proc chance increased to 13% from 10%)
    * added pierce-fire to "prop8", set "min8" and "max8" to 18/21 (-18-21% enemy fire resistance)
    * added extra-fire to "prop9", set "min9" and "max9" to 7/11 (7-11% to fire skill damage)
    * added reduce-ac to "prop10", set "min10" and "max10" to 66/66 (-66% target defense)
    * added dur to "prop11", set "min11" and "max11" to 60/60 (60 durability bonus)

  * Messerschmidt's Reaver
    * increased "min7" to 171 from 20 (fire damage increased to 171-240 from 20-240)
    * increased "min8" and "max8" to 75/75 from 25/25 (durability bonus increased to 75 from 25)
    * added dmg-ac to "prop10", set "min10" and "max10" to -125/-125 (-125 monster defense per hit)
    * added manasteal to "prop11", set "min11" and "max11" to 14/17 (14-17% mana stolen per hit)
    * added oskill to "prop12", Revive to "par12", set "min12" and "max12" to 5/5 (level 5 Revive oskill)

  * Baranar's Star
    * increased "max7" to 250 from 200 (lightning damage increased to 1-250 from 1-200)
    * increased "max8" to 250 from 200 (fire damage increased to 1-250 from 1-200)
    * increased "max9" to 250 from 200 (cold damage increased to 1-250 from 1-200)

  * Schaefer's Hammer
    * increased "min8" and "max8" to 120/150 from 100/130 (enhanced damage increased to 120-150% from 100-130%)
    * increased "min9" and "max9" to 2/2 from 1/1 (light radius increased to 2 from 1)
    * increased "max10" to 300 from 200 (lightning damage increased to 50-300 from 50-200)

  * The Cranium Basher
    * increased "max6" to 25 from 20 (max damage increased to 25 from 20 [also makes the damage bonus display as "adds 20-25 damage", ingame it would only show +20 minimum damage])
    * increased "min7" and "max7" to 233/266 from 200/240 (enhanced damage increased to 233-266% from 200-240%)
    * increased "min8" and "max8" to 17/5 from 4/1 (Amplify Damage on striking proc chance increased to 17% from 4%, level increased to 5 from 1)

  * Lightsabre
    * increased "min2" to 11 from 5 (Chain Lightning on attack proc chance increased to 11% from 5%)

  * Doombringer
    * increased "min3" and "max3" to 133/166 from 40/40 (attack rating increased to 133-166% from 40%)
    * changed "par6" to 87 from 72, changed "min6" and "max6" to 24/6 from 8/3 (Weaken on striking changed to Decrepify, proc chance increased to 24% from 8%, level changed to 6 from 3)
    * added deadly to "prop8", set "min8" and "max8" to 28/37 (28-37% chance of deadly strike)

  * The Grandfather
    * increased "min5" and "max5" to 125/160 from 50/50 (attack rating increased to 125-160% from 50%)
    * changed "prop8" to dur from indestruct, changed "min8" and "max8" to 105/105 (105 durability bonus instead of indestructible)
    * increased "min9" and "max9" to 270/330 from 150/250 (enhanced damage increased to 270-330% from 150-250%)
    * added addxp to "prop10", set "min10" and "max10" to 7/9 (adds 7-9% to experience gained)

  * Stormspire
    * increased "min2" and "max2" to 10/22 from 5/5 (Chain Lightning when struck proc chance increased to 10% from 5%, level increased to 22 from 5)
    * increased "min3" to 190 from 150 (enhanced damage increased to 190-250% from 150-250%)
    * increased "min4" and "max4" to 15/20 from 10/10 (strength increased to 15-20 from 10)
    * changed "par5" to Blizzard from 38, increased "min5" and "max5" to 8/17 from 2/0 (Charged Bolt when struck changed to Blizzard, proc chance increased to 8% from 2%, level decreased to 17 from 20)
    * increased "max8" to 449 from 237 (lightning damage increased to 1-449 from 1-237)
    * increased "min9" and "max9" to 179/227 from 27/27 (attacker takes lightning damage increased to 179-227 from 27)
    * added res-cold to "prop10", set "min10" and "max10" to 30/30 (cold resist 30%)
    * added pierce-ltng to "prop11", set "min11" and "max11" to 30/40 (-30-40% enemy lightning resistance)
    * added pierce-cold to "prop12", set "min12" and "max12" to 25/35 (-25-35% enemy cold resistance)

  * Eaglehorn
    * changed "prop1" to reduce-ac from ignore-ac, increased "min1" and "max1" to 80/80 from 1/1 (-80% target defense instead of ignore target's defense)
    * increased "min5" and "max5" to 2/3 from 1/1 (amazon skill levels increased to 2-3 from 1)

  * Bul Katho's Wedding Band (Bul-Kathos' Wedding Band)
    * changed "prop1" to hp from hp/lvl, changed "par1" to blank from 4, set "min1" and "max1" to 20/30 (20-30 life instead of 0.5 life per level)
    * increased "diablocloneweight" to 1 from 0 (allows Diablo Clone to be summoned by selling a BK ring to vendors)

  * The Cat's Eye
    * increased "min2" and "max2" to 25/30 from 20/20 (increased attack speed increased to 25-30% from 20%)
    * increased "min3" and "max3" to 150/150 from 100/100 (defense increased to 150 from 100)
    * increased "min4" and "max4" to 250/250 from 100/100 (defense vs missile increased to 250 from 100)

  * The Rising Sun
    * increased "min3" to 11 from 2 (Meteor when struck proc chance increased to 11% from 2%)
    * increased "min4" and "max4" to 94/188 from 24/48 (fire damage increased to 94-188 from 24-48)
    * ~~added pierce-fire to "prop7", set "min7" and "max7" to 10/10 (-10% enemy fire resistance)~~ (see patch 1.03b)

  * Crescent Moon (amulet)
    * added openwounds to "prop7", set "min7" and "max7" to 15/20 (15-20% chance of open wounds)

  * Atma's Scarab
    * increased "min1" and "max1" to 588/588 from 102/102 (poison bitrate increased to 588 from 102 [poison damage increased to 230 over 4 seconds from 40 over 4 seconds])
    * increased "min4" and "max4" to 45/45 from 5/5 (attacker takes damage increased to 45 from 5)
    * increased "min5" and "max5" to 8/3 from 5/2 (Amplify Damage on striking proc chance increased to 8% from 5%, level increased to 3 from 2)
    * added pierce-pois to "prop7", set "min7" and "max7" to 8/11 (-8-11% enemy poison resistance)

  * Highlord's Wrath
    * deleted all stats from "prop2" through "max2" and moved the other stats over (removed lightning damage cause I like the sounds of critical hits and I hate how elemental damage overwrites it even though you'll probably use a Raven Frost anyways :p)
    * increased new "min5" and "max5" to 76/76 from 15/15 (attacker takes lightning damage increased to 76 from 15)

  * Saracen's Chance
    * increased "max2" to 8 from 2 (Iron Maiden when struck level increased to 8 from 2)
    * increased "min3" and "max3" to 14/14 from 12/12 (strength increased to 14 from 12)
    * increased "min4" and "max4" to 14/14 from 12/12 (dexterity increased to 14 from 12)
    * increased "min5" and "max5" to 14/14 from 12/12 (energy increased to 14 from 12)
    * increased "min6" and "max6" to 14/14 from 12/12 (vitality increased to 14 from 12)
    * added gethit-skill to "prop7", set "par7" to 81, set "min7" and "max7" to 7/6 (7% chance to cast level 6 Confuse when struck)
    * added gethit-skill to "prop8", set "par7" to 71, set "min7" and "max7" to 13/9 (13% chance to cast level 9 Dim Vision when struck)

  * The Oculus
    * decreased "min1" and "max1" to 2/2 from 3/3 (sorc skills decreased to 2 from 3)

  * Bloodmoon
    * changed "prop3" to oskill from charged, changed "min3" to 15 from 9 (Blood Golem charges changed to oskill)

  * Djinnslayer (Djinn Slayer)
    * increased "min5" and "max5" to 6/9 from 3/7 (lightning absorb increased to 6-9 from 3-7)

  * Warshrike
    * increased "max6" to 12 from 9 (Nova on striking level increased to 12 from 9)

  * Gutsiphon (Gut Siphon)
    * increased "min1" to 185 from 160 (enhanced damage increased to 185-220% from 160-220%)
    * increased "min3" to 14 from 12 (life stolen increased to 14-18% from 12-18%)
    * increased "min5" and "max5" to 45/45 from 33/33 (open wounds proc chance increased to 45% from 33%)
    * added manasteal to "prop6", set "min6" and "max6" to 3/6 (3-6% mana stolen per hit)

  * Razoredge (Razor's Edge)
    * increased "min3" and "max3" to 40/40 from 33/33 (target defense increased to -40% from -33%)
    * added thorns to "prop6", set "min6" and "max6" to 42/65 (attacker takes 42-65 damage)

  * Demonlimb (Demon Limb)
    * increased "min2" and "max2" to 333/444 from 222/333 (fire damage increased to 333-444 from 222-333)
    * increased "max6" to 246 from 123 (damage to demons increased to 123-246% from 123%)
    * increased "min7" and "max7" to 20/30 from 15/20 (fire resist increased to 20-30% from 15-20%)

  * Steelshade
    * increased "min2" and "max2" to 8/13 from 5/11 (fire absorb increased to 8-13 from 5-11)
    * increased "min4" and "max4" to 16/23 from 10/18 (replenish life increased to 16-23 from 10-18)
    * added red-dmg to "prop5", set "min5" and "max5" to 8/11 (damage reduced by 8-11)
    * added sock to "prop6", set "par6" to 1 (1 socket)

  * Tomb Reaver
    * increased "min3" to 220 from 200 (enhanced damage increased to 220-280% from 200-280%)
    * increased "min6" to 35 from 30 (all resistances increased to 35-50% from 30-50%)
    * increased "min8" and "max8" to 12/12 from 10/10 (reanimated as returned proc chance increased to 12% from 10%)
    * increased "min10" to 2 from 1 (sockets increased to 2-3 from 1-3)

  * Nature's Peace
    * increased "min5" and "max5" to 54/7 from 27/5 (Oak Sage charge count increased to 54 from 27, level increased to 7 from 5)

  * Azurewrath
    * added extra-cold to "prop9", set "min9" and "max9" to 12/16 (12-16% to cold skill damage)

  * Seraph's Hymn
    * increased "min3" and "max3" to 75/100 from 25/50 (damage to demons increased to 75-100% from 25-50%)
    * increased "min4" and "max4" to 75/100 from 25/50 (damage to undead increased to 75-100% from 25-50%)
    * increased "min5" and "max5" to 200/350 from 150/250 (attack rating against demons increased to 200-350 from 150-250)
    * increased "min6" and "max6" to 200/350 from 150/250 (attack rating against undead increased to 200-350 from 150-250)
    * added ac% to "prop8", set "min8" and "max8" to 30/40 (30-40% enhanced defense)

  * Fleshripper
    * increased "min1" to 230 from 200 (enhanced damage increased to 230-300% from 200-300%)

  * Horizon's Tornado
    * increased "max3" to 30 from 20 (slows target increased to 20-30% from 20%)
    * increased "min4" to 33 from 20 (Tornado on striking proc chance increased to 33% from 20%)

  * Stone Crusher
    * increased "min4" and "max4" to 33/33 from 25/25 (target defense increased to -33% from -25%)
    * increased "min6" to 20 from 10 (+damage increased to 20-30 from 10-30)

  * Cerebus (Cerebus' Bite)
    * increased "min1" and "max1" to 170/210 from 130/140 (enhanced defense increased to 170-210% from 130-140%)
    * increased "min2" to 3 from 2 (shape shifting skills increased to 3-4 from 2-4)
    * increased "min4" to 75 from 60 (attack rating increased to 75-120% from 60-120%)
    * increased "min6" and "max6" to 2/3 from 1/2 (feral rage increased to 2-3 from 1-2)
    * added "move2" to "prop7", set "min7" and "max7" to 20/20 (20% faster run/walk)

  * Tyrael's Might
    * increased "min3" and "max3" to 160/180 from 120/150 (enhanced defense increased to 160-180% from 120-150%)
    * changed "prop4" to sock from rip, set "min4" and "max4" to 2/2 (2 sockets instead of slain monsters rest in peace)
    * increased "min5" and "max5" to 200/250 from 50/100 (damage to demons increased to 200-250% from 50-100%)
    * increased "min7" and "max7" to 70/70 from 20/20 (faster run/walk increased to 70% from 20%)
    * changed "prop8" to aura from res-all, set "par8" to Salvation, set "min8" and "max8" to 1/1 (level 1 Salvation when equipped instead of all resistances 20-30%)
    * added item_heavenlyburden to "prop10", set "min10" and "max10" to 1/1 (heavenly burden on mercenaries [Salvation aura only works at 1/6 effectiveness, -75% velocity and attack rate, -100% PDR only when equipped by the mercenary, no penalty for players])
    * added allskills to "prop11", set "min11" and "max11" to 1/1 (1 all skills)
    * added res-poison-len to "prop12", set "min12" and "max12" to 175/175 (175% poison length reduced)

  * Souldrain (Soul Drainer)
    * increased "min4" and "max4" to 11/5 from 8/3 (Weaken on striking proc chance increased to 11% from 8%, level increased to 5 from 3)
    * increased "min5" and "max5" to -75/-75 from -50/-50 (monster defense per hit increased to -75 from -50)

  * Deathcleaver (Death Cleaver)
    * increased "min3" and "max3" to 50/50 from 33/33 (target defense increased to -50% from -33%)

  * Executioner's Justice
    * increased "min3" and "max3" to 70/70 from 33/33 (target defense increased to -70% from -33%)
    * changed "par4" to Amplify Damage from Decrepify, decreased "min4" to 25 from 50, increased "max4" to 8 from 6 (Decrepify when you kill an enemy changed to Amplify Damage, proc chance decreased to 25% from 50%, level increased to 8 from 6)

  * Stoneraven
    * increased "min1" and "max1" to 300/340 from 230/280 (enhanced damage increased to 300-340% from 230-280%)
    * increased "min2" and "max2" to 369/420 from 101/187 (magic damage increased to 369-420 from 101-187)
    * increased "min3" and "max3" to 35/50 from 30/50 (all resistances increased to 35-50% from 30-50%)
    * increased "min5" and "max5" to 3/4 from 1/3 (javelin and spear skills increased to 3-4 from 1-3)
    * added ac% to "prop6", set "min6" and "max6" to 60/80 (60-80% enhanced defense)

  * Wisp (Wisp Projector)
    * increased "min2" and "max2" to 12/21 from 10/16 (Lightning on striking proc chance increased to 12% from 10%, level increased to 21 from 16)
    * increased "min4" to 40 from 20 (Oak Sage charge count increased to 40 from 20)
    * increased "min5" and "max5" to 26/8 from 13/5 (Heart of Wolverine charge count increased to 26 from 13, level increased to 8 from 5)
    * increased "min6" and "max6" to 22/13 from 11/7 (Spirit of Barbs charge count increased to 22 from 11, level increased to 13 from 7)

  * Gargoyle's Bite
    * decreased "par3" to 150 from 250, increased "min3" and "max3" to 1574/1574 from 300/300 (poison length reduced to 150 frames/6 seconds from 250 frames/10 seconds, poison bitrate increased to 1574 from 300 [poison damage increased to 922 over 6 seconds from 293 over 10 seconds])
    * changed "prop5" to oskill from charged, changed "min5" to 8 from 60 (Plague Javelin charges changed to oskill, level decreased to 8-11 from 11)
    * added dmg-ac to "prop6", set "min6" and "max6" to -110/-110 (-110 monster defense per hit)
    * added extra-pois to "prop7", set "min7" and "max7" to 11/15 (11-15% poison skill damage)

  * Lacerator
    * deleted "par6" through "max6" and moved the other stat over (removed hit causes monster to flee 50%)

  * Mang Song's Lesson
    * increased "min2" and "max2" to 13/17 from 7/15 (enemy fire resistance increased to -13-17% from -7-15%)
    * increased "min3" and "max3" to 13/17 from 7/15 (enemy lightning resistance increased to -13-17% from -7-15%)
    * increased "min4" and "max4" to 13/17 from 7/15 (enemy cold resistance increased to -13-17% from -7-15%)
    * increased "min5" and "max5" to 45/45 from 10/10 (regenerate mana increased to 45% from 10%)

  * Viperfork
    * decreased "par2" to 75 from 250, increased "min2" and "max2" to 2047/2047 from 333/333 (poison length decreased to 75 frames/3 seconds from 250 frames/10 seconds, poison bitrate increased to 2047 from 333 [poison damage increased to 600 over 3 seconds from 325 over 10 seconds])
    * increased "min4" and "max4" to 300/350 from 200/250 (attack rating increased to 300-350 from 200-250)
    * increased "max5" to 16 from 9 (Poison Explosion on striking level increased to 16 from 9)
    * increased "min6" and "max6" to 50/70 from 30/50 (poison resist increased to 50-70% from 30-50%)

  * Ethereal Edge
    * increased "min3" and "max3" to 13/17 from 10/12 (fire absorb increased to 13-17 from 10-12)
    * increased "min5" and "max5" to 9/14 from 5/10 (life after each demon kill increased to 9-14 from 5-10)
    * added reduce-ac to "prop9", set "min9" and "max9" to 20/20 (-20% target defense)

  * Demonhorn's Edge
    * increased "min2" and "max2" to 15/15 from 10/10 (increased attack speed increased to 15% from 10%)
    * increased "min3" and "max3" to 5/7 from 3/6 (life stolen increased to 5-7% from 3-6%)
    * increased "min4" and "max4" to 99/121 from 55/77 (attacker takes damage increased to 99-121 from 55-77)
    * added dmg% to "prop8", set "min8" and "max8" to 45/65 (45-65% enhanced damage)

  * Spiritkeeper (Spirit Keeper)
    * added skill to "prop8", set "par8" to Oak Sage, set "min8" and "max8" to 2/3 (2-3 to Oak Sage)
    * added skill to "prop9", set "par9" to Heart of Wolverine, set "min9" and "max9" to 2/3 (2-3 to Heart of Wolverine)
    * added skill to "prop10", set "par10" to Spirit of Barbs, set "min10" and "max10" to 2/3 (2-3 to Spirit of Barbs)

  * Hellrack
    * increased "min2" to 151 from 63 (elemental damage increased to 151-324 from 63-324)
    * changed "prop6" to oskill from charged, changed "min6" and "max6" to 16/19 from 150/18 (Immolation Arrow charges changed to oskill, level changed to 16-19 from 18)

  * Alma Negra
    * increased "min5" and "max5" to 11/14 from 5/9 (magic damage reduced increased to 11-14 from 5-9)
    * changed "prop6" to att from att%, increased "min6" and "max6" to 110/155 from 40/75 (110-155 attack rating instead of 40-75% attack rating)
    * changed "prop7" to dmg-norm from dmg%, decreased "min7" and "max7" to 12/23 from 40/75 (adds 12-23 damage instead of 40-75% enhanced damage)

  * Widowmaker
    * added ease to "prop6", set "min6" and "max6" to -15/-15 (requirements -15%)

  * Bloodraven's Charge (Blood Raven's Charge)
    * increased "min3" and "max3" to 21/21 from 13/13 (fires explosive arrows increased to level 21 from 13)
    * increased "min4" to 3 from 2 (bow and crossbow skills increased to 3-4 from 2-4)
    * increased "min5" and "max5" to 72/9 from 30/5 (Revive charge count increased to 72 from 30, level increased to 9 from 5)
    * added pierce-fire to "prop6", set "min6" and "max6" to 21/24 (-21-24% enemy fire resistance)
    * added dmg-fire to "prop7", set "min7" and "max7" to 142/250 (142-250 fire damage)

  * Ghostflame
    * increased "min3" and "max3" to 238/238 from 108/108 (magic damage increased to 238 from 108)
    * added red-dmg% to "prop8", set "min8" and "max8" to 7/9 (7-9% PDR)

  * Shadowkiller (Shadow Killer)
    * added pierce-cold to "prop8", set "min8" and "max8" to 10/14 (-10-14% enemy cold resistance)

  * Boneflame
    * increased "max2" to 30 from 20 (faster run/walk increased to 20-30% from 20%)
    * increased "min3" and "max3" to 21/5 from 15/3 (Terror when struck proc chance increased to 21% from 15%, level increased to 5 from 3)
    * added pierce-fire to "prop6", set "min6" and "max6" to 9/12 (-9-12% enemy fire resistance)

  * Steelpillar (Steel Pillar)
    * increased "min1" and "max1" to 240/270 from 210/260 (enhanced damage increased to 240-270% from 210-260%)
    * increased "min3" and "max3" to 45/45 from 20/20 (target defense increased to -45% from -20%)
    * increased "min4" and "max4" to 70/95 from 50/80 (enhanced defense increased to 70-95% from 50-80%)

  * Dragonscale
    * increased "min3" and "max3" to 10/10 from 5/5 (maximum fire resist increased to 10% from 5%)
    * increased "min4" and "max4" to 30/40 from 15/25 (strength increased to 30-40 from 15-25)
    * increased "min5" and "max5" to 331/411 from 211/371 (fire damage increased to 331-411 from 211-371)
    * increased "min6" and "max6" to 18/18 from 10/10 (Hydra oskill level increased to 18 from 10)

  * Steel Carapice (Steel Carapace)
    * increased "min3" and "max3" to 26/31 from 9/14 (damage reduced increased to 26-31 from 9-14)
    * increased "min5" and "max5" to 25/35 from 10/15 (regenerate mana increased to 25-35% from 10-15%)
    * increased "min7" and "max7" to 14/17 from 8/6 (Iron Maiden when struck proc chance increased to 14% from 8%, level increased to 17 from 6)

  * Medusa's Gaze
    * increased "max2" to 25 from 20 (slows target increased to 20-25% from 20%)
    * increased "min3" to 17 from 10 (Lower Resist when struck proc chance increased to 17% from 10%)
    * increased "min6" to 55 from 40 (cold resist increased to 55-80% from 40-80%)
    * added ease to "prop8", set "min8" and "max8" to -35/-35 (requirements -35%)

  * Flamebellow
    * increased "min2" to 466 from 233 (fire damage increased to 466-482 from 233-482)
    * increased "min5" and "max5" to 22/25 from 12/16 (Firestorm on striking proc chance increased to 22% from 12%, level increased to 25 from 16)
    * increased "min6" and "max6" to 20/30 from 10/20 (strength increased to 20-30 from 10-20)
    * increased "min7" and "max7" to 12/17 from 5/10 (vitality increased to 12-17 from 5-10)
    * increased "min8" to 15 from 12 (Inferno oskill level increased to 15-18 from 12-18)

  * Spirit Ward
    * increased "min2" and "max2" to 8/14 from 6/11 (cold absorb increased to 8-14 from 6-11)
    * increased "min6" to 10 from 5 (Fade when struck proc chance increased to 10% from 5%)

  * Stormlash
    * increased "min6" and "max6" to 110/110 from 30/30 (attacker takes lightning damage increased to 110 from 30)

  * Halaberd's Reign
    * increased "min2" and "max2" to 2/2 from 1/1 (combat masteries skills increased to 2 from 1)
    * increased "min5" and "max5" to 19/26 from 15/23 (replenish life increased to 19-26 from 15-23)
    * increased "min6" to 2 from 1 (Battle Orders level increased to 2 from 1-2)
    * increased "min7" to 2 from 1 (Battle Command level increased to 2 from 1-2)
    * added hit-skill to "prop8", set "par8" to Shout, set "min8" and "max8" to 12/4 (12% chance to cast level 4 Shout on striking)

  * Spike Thorn
    * increased "par2" to 27 from 11 (attacker takes damage per level increased to 3.375 from 1.375)
    * added gethit-skill to "prop7", set "par7" to Amplify Damage, set "min7" and "max7" to 19/8 (19% chance to cast level 8 Amplify Damage when struck)

  * Frostwind
    * changed "prop3" to nofreeze from half-freeze (cannot be frozen instead of half freeze duration)
    * increased "par4" to 300 from 150 and "min4" to 453 from 237 (cold length increased to 300 frames/12 seconds from 150 frames/6 seconds, cold damage increased to 453-486 from 237-486)
    * increased "min7" and "max7" to 10/16 from 7/14 (Arctic Blast oskill level increased to 10-16 from 7-14)
    * added pierce-cold to "prop8", set "min8" and "max8" to 18/23 (-18-23% enemy cold resistance)

  * Templar's Might
    * increased "min3" and "max3" to 375/450 from 250/300 (defense vs missile increased to 375-450 from 250-300)
    * changed "prop4" to hp from stam, increased "max4" to 60 from 50 (40-60 life instead of 40-50 stamina)
    * increased "min5" and "max5" to 15/25 from 10/15 (strength increased to 15-25 from 10-15)

  * Firelizard's Talons
    * increased "min4" to 419 from 236 (fire damage increased to 419-480 from 236-480)
    * added fireskill to "prop8", set "min8" and "max8" to 2/2 (2 to fire skills)
    * added pierce-fire to "prop9", set "min9" and "max9" to 6/8 (-6-8% enemy fire resistance)

  * Sandstorm Trek
    * increased "par4" to 18 from 8 (stamina per level increased to 2.25 from 1)
    * added res-poison-len to "prop10", set "min10" and "max10" to 50/50 (50% poison length reduced)

  * Marrowwalk
    * increased "min3" to 35 from 13 (Bone Prison charge count increased to 35 from 13)

  * Metalgrid
    * increased "min5" and "max5" to 33/21 from 20/12 (Iron Maiden charge count increased to 33 from 20, level increased to 21 from 12)
    * added oskill to "prop6", set "par6" to Summon Resist, set "min6" and "max6" to 1/1 (level 1 Summon Resist oskill)

  * Carrion Wind
    * increased "min1" and "max1" to 130/190 from 100/160 (defense vs missile increased to 130-190 from 100-160)
    * increased "min2" and "max2" to 11/13 from 10/10 (Poison Nova when struck proc chance increased to 11% from 10%, level increased to 13 from 10)
    * increased "min5" to 41 from 15 (Poison Creeper charge count increased to 41 from 15)
    * increased "min6" and "max6" to 9/16 from 8/13 (Twister on striking proc chance increased to 9% from 8%, level increased to 16 from 13)

  * Annihilus
    * decreased "lvl" to 100 from 110 (item level decreased to 100 from 110)

  * Cranebeak
    * increased "max2" to 391 from 305 (lightning damage increased to 1-391 from 1-305)
    * increased "min3" to 30 from 20 (magic find increased to 30-50% from 20-50%)
    * increased "min6" and "max6" to 75/19 from 15/8 (Raven charge count increased to 75 from 15, level increased to 19 from 8)

  * Nord's Tenderizer
    * changed "prop4" to hit-skill from charged, changed "min4" and "max4" to 14/14 from 12/16 (14% chance to cast level 14 Blizzard on striking instead of 12 level 16 Blizzard charges)
    * increased "min6" and "max6" to 20/25 from 5/15 (cold absorb increased to 20-25% from 5-15%)
    * increased "par7" to 225 from 125 and "min7" to 317 from 205 (cold length increased to 225 frames/9 seconds from 125 frames/5 seconds, cold damage increased to 317-455 from 205-455)

  * Earthshifter (Earth Shifter)
    * changed "prop5" to hit-skill from charged, changed "min5" and "max5" to 11/13 from 30/14 (11% chance to cast level 13 Volcano on striking instead of 30 level 14 Volcano charges)
    * increased "min7" and "max7" to 20/20 from 10/10 (faster cast rate increased to 20% from 10%)
    * added ease to "prop8", set "min8" and "max8" to -15/-15 (-15% requirements)

  * Bonehew
    * increased "min3" to 42 from 30 (Corpse Explosion charge count increased to 42 from 30)

  * Ondal's Wisdom
    * increased "min5" and "max5" to 8/11 from 5/5 (experience gained increased to 8-11% from 5%)

  * Headhunter's Glory (Head Hunter's Glory)
    * increased "min4" to 2 from 1 (sockets increased to 2-3 from 1-3)
    * added mana-kill to "prop7", set "min7" and "max7" to 5/7 (5-7 mana after each kill)

  * Steelrend
    * increased "min3" and "max3" to 45/70 from 30/60 (enhanced damage increased to 45-70% from 30-60%)
    * increased "min4" and "max4" to 15/20 from 10/10 (crushing blow increased to 15-20% from 10%)

  * Hellfire Torch
    * deleted all stats from "prop5" through "max5" and moved the other stats over (removed Firestorm proc)
    * decreased "lvl" to 100 from 110 (item level decreased to 100 from 110)

  * Arpaska's Medallion
    * created new entry for "Arpaska's Medallion" (cloned row 403)
    * set "lvl" to 99
    * set "lvl req" to 40
    * set "code" to cm1
    * set "carry1" to blank
    * set "prop1" to oskill, set "par1" to Teleport, set "min1" and "max1" to 1/1 (level 1 Teleport oskill)
    * set "prop2" to res-all-max, set "min2" and "max2" to -15/-15 (-15% maximum all resists)

#### weapons.txt
  * increased "mindam", "maxdam", "2handmindam", "2handmaxdam", "minmisdam", and "maxmisdam" of all exceptional weapons by 15% (decimals 0.0-0.4 rounded down, 0.5+ rounded up)
  * increased "mindam", "maxdam", "2handmindam", "2handmaxdam", "minmisdam", and "maxmisdam" of all elite weapons by 20% (decimals 0.0-0.4 rounded down, 0.5+ rounded up)
  * increased "rangeadder" of throwing axes/balanced axes (and their exceptional/elite variants) to 1 from 0
  * increased "StrBonus" and "DexBonus" of all axes to 130/30 from 100/0 (axes gain 1.3/0.3% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all wands/orbs to 120/40 from 100/0 (wands/orbs gain 1.2/0.4% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all maces/scepters/staves to 160/0 from 100/0 (flail/knout/scourge changed to 130/40 from 100/0) (maces gain 1.6/0% enhanced damage per strength/dexterity [flail/scourge/knout gain 1.3/0.4% enhanced damage per strength/dexterity])
  * increased "StrBonus" and "DexBonus" of all hammers to 170/0 from 110/0 (hammers gain 1.7/0% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all swords to 110/50 from 100/0 (swords gain 1.1/0.5% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all daggers/throwing knives to 60/100 from 75/75 (daggers/throwing knives gain 0.6/1% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all javelins/throwing axes/katars to 80/80 from 75/75 (javelins/throwing axes/katars gain 0.8/0.8% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all spears to 100/60 from 100/0 (spears gain 1/0.6% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all polearms to 140/20 from 100/0 (polearms gain 1.4/0.2% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all bows/amazon bows to 60/100 from 0/100 (bows/amazon bows gain 0.6/1% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all crossbows to 80/100 from 0/100 (crossbows gain 0.8/1% enhanced damage per strength/dexterity)
  * increased "StrBonus" and "DexBonus" of all amazon spears to 100/80 from 80/50 (amazon spears gain 1/0.8% enhanced damage per strength/dexterity)
  * ~~increased "StrBonus" and "DexBonus" of all amazon javelins to 80/60 from 80/50 (amazon javelins gain 0.8/0.6% enhanced damage per strength/dexterity)~~ (see patch 1.03)
  * increased "durability" of normal/exceptional/elite weapons by 50/125/200% (decimals 0.0-0.4 rounded down, 0.5+ rounded up)
  * ~~set "ShowLevel" to 1 (displays item level)~~ (see patch 1.03)

### data>global>monsters
* z4
  * added new entry for "z4" (cloned from va folder in vanilla data>global>monsters)
  * changed all applicable file prefixes to start with "z4" instead of "va" (fixes Trang vampire appearance in legacy graphics, it was invisible otherwise [currently a bug where the idle animation is faster])

### data>global>animdata.d2
* trangvampire
  * added new entry for "trangvampire" and set it to use necro casting animations (part of a change to allow Trang vampires to use necro casting frames instead of slow vampire casting frames)

### data>hd>character
#### monsters.json
  * trangvampire
    * added new entry for "trangvampire" (part of a change to allow Trang vampires to use necro casting frames instead of slow vampire casting frames)

### data>hd>global>ui>logoanimation
  * added custom logoanimation.sprite with DMMod logo

### data>hd>global>ui>spells>hireables
  * added Double Swing icon to hrskillicon.sprite (adds a Double Swing icon to be used for the Frenzy Act 5 merc skill list)

### data>hd>global>excel
#### desecratedzones.json
  * ~~decreased "terror_duration_min" to 25 from 60 (Terror Zones change every 25 minutes instead of 60 minutes)~~ (see patch 1.03)
  * changed "seed" to 14803616718064904423 from 16664395743969097666 (changes the order in which TZs are selected)
  * removed Blood Moor and Den of Evil
  * merged Stony Field and Tristram
  * added Tamoe Highland to the Pit
  * added Maggot Lair to Far Oasis
  * added Canyon of the Magi to Tal Rasha's Tombs
  * added Arachnid Lair to Spider Forest and Spider Cavern

### data>hd>global>video
  * added blank blizzardlogos.webm and logoanim.webm (skips the D2R intro logos)
  * added custom logoloop.webm with DMMod logo

### data>local>lng>strings
#### item-modifiers.json
  * added new entry for "id" 50000 (ModStrHeavenlyBurden)
  * used Google Translate for non-English languages

#### item-names.json
  * added new entry for "id" 51000 (Arpaska's Medallion)
  * used Google Translate for non-English languages

#### skills.json
  * changed "id" 4415 (Jab tooltip) to add daggers to the list of usable weapon types
  * changed "id" 4431 (Power Strike tooltip) to add daggers to the list of usable weapon types
  * changed "id" 4471 (Charged Strike tooltip) to add daggers to the list of usable weapon types
  * changed "id" 4511 (Lightning Strike tooltip) to add daggers to the list of usable weapon types
  * changed "id" 22052 (Lycanthropy tooltip) to add run/walk speed to the statlist
  * added new entry for "id" 52000 (StrSkillDefenseActive)
  * added new entry for "id" 52001 (StrSkillDefensePassive)
