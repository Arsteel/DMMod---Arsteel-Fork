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

See DMMod's changelog for those changes. This will only list changes made by Arsteel.

**Arsteel Patch 0.03 Changelog**

https://docs.google.com/document/d/1yyHu9l2f-mYBThKDynIl6eygLm0oFDuT2gAnQ38nGWU/edit?tab=t.0

**Arsteel Patch 0.02 Changelog**

https://docs.google.com/document/d/1aS1XIRuz68l4xgt-agBf_TQC6kYNilECrpxRbQOA8tA/edit?tab=t.0

**Arsteel Patch 0.01c Changelog**

Added missing json files to data/local/lng/strings

**Arsteel Patch 0.01b Changelog**

Replaced the main directory folder with the correct version for the patch notes. Oops. 

**Arsteel Patch 0.01 Changelog**

https://docs.google.com/document/d/1oFkBNy5SQwizKXKrtklme89k9g5hvqqpdJv_08bKXeA/edit?tab=t.0

**Arsteel Patch 0.00 Changelog**

https://docs.google.com/document/d/1ttZ2f1edTHdIQxnJkoucYgROWXUlH8IR0C8QW2WsU00/edit?tab=t.0
