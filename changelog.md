Invasion from the Unknown - Changelog
=====================================

Version 2.1.3+dev:
------------------
* General:
  * Replaced deprecated Lua API calls.


Version 2.1.3:
--------------
* General:
  * Update to Naia 20200625.
  * Fixed OOS errors caused by Naia's cutscene skip functionality, first
    introduced in version 2.1.1.

* Scenarios:
  * Added a hint to all scenarios about browsing through unit AMLAs. This is
    only displayed once per save and it is triggered by Anlindë reaching level
    4 for the first time, or by Elynia existing on the game map.


Version 2.1.2:
--------------
* General:
  * Update to Naia 20200621.
  * Updated art licenses for CC BY-NC-ND 4.0, CC BY-SA 4.0 and CC0 content.

* Graphics:
  * New or updated unit graphics: Anlindë Elvish Avatar.

* Language and i18n:
  * Updated translations: French (Naia only), Russian (complete).

* Music:
  * Added Telaron's Climactic Contemplation and Western_Theme2 to IftU Music
    0.3.2.

* Scenarios:
  * S2 - A Real Confrontation:
    * Don't scroll back to Lédinor when he remarks on the newly recruited demon
      (fixes #64)
  * S7 - Goliath:
    * Made it more practical to find and obtain the Void Armor item.
  * S10 - The Source of Light:
    * Fixed Berserker Potion increasing the unit's HP pool without increasing
      its current HP as well.
  * S16 - Dawn of War
    * Properly displayed gold carryover bonus in the objectives after defeating
      enemies (fixes #50).
  * S19 - Under the Sands
    * Clarified objectives (fixes #52).

* Units:
  * Chaos Cardinal migrated to Naia and expanded with a new baseframe by VYNLT
    and slightly different stats over the mainline Ancient Lich.
  * Use 1.14 rodent fangs icon for the Rabbit's incisors attack.
  * Chaos Hound line is now considered part of the wolves race and receives
    names and traits accordingly.
  * Implemented a more elegant way to disable Enchantress advancement to Sylph
    (fixes #38).
  * Terror ability no longer affects same-level units.


Version 2.1.1:
--------------
* General:
  * Update to Naia 20180722.

* Units:
  * Revised Elvish Avatar (Anlindë)'s AMLA tree:
    * XP increase for all AMLAs is 15%.
  * Revised Lady of Light (Elynia)'s AMLA tree:
    * XP increase for all AMLAs is 15%.
    * Base XP decreased from 90 XP to 70 XP.
    * Strength I: HP +4, melee dmg +1.
    * Strength II: HP +4, melee str +1.
    * Strength III: HP +5.
    * Strength IV: HP +5, melee dmg +1.
    * Strength V: HP +7.
    * Focus I: faerie fire dmg +1, requires Strength I.
    * Focus II: faerie fire str +1, requires Strength III.
    * Focus III: ensnare str +1, requires Strength IV.
    * Shielding I: arcane res +10%, requires Focus I.
    * Shielding II: arcane res +10%, impact res +10%, requires Focus II.
    * Shielding III: arcane res +10%, cold res +10%, requires Strength IV.
    * Thorns I: new attack - ranged pierce magical+drain 10-2.
    * Thorns II: thorns str +1.
    * Thorns III: thorns dmg +2.


Version 2.1.0:
--------------
* General:
  * Wesnoth 1.14 support implememented, raising the minimum version requirement
    to Wesnoth 1.13.12 (Wesnoth 1.15.x is *not* supported yet). Some large
    chunks of code (in particular FOREACH loops) were rewritten in the
    process.
  * Shared units, assets, code, and translations are now part of the Naia
    library, also used by AtS version 0.10.0 and later.

* Language and i18n:
  * Removed empty Dutch translation.

* Music:
  * Added Aleksi's gameplay06.ogg to IftU Music 0.3.1.

* Scenarios:
  * General:
    * Revised a few maps to use 1.14 terrains.
    * The old IftU/AtS gates have been replaced with the new mainline gates.
      Special event gates are now recolored mainline rusty gates. While the
      open version does exist, it's not currently used since event gates are
      handled as barriers that get completely removed by scenarios.
    * Added wall moss overlays from Naia/AtS to hive maps.
    * Unit loyalty in boss/finale scenarios is now controlled using temporary
      or permanent [object] modifications instead of direct attribute
      manipulation, as the latter causes issues in 1.14. The same applies to
      the hidden loyal trait for special characters such as Mal Keshar,
      Anlindë, and Elynia (issue #27).
  * S2 - A Real Confrontation:
    * Lédinor's supporter now starts with 0 moves and outside his castle (see
      issue #29).
  * S7 - Goliath:
    * Removed demon embedded in a wall (issue #36).
    * Kill all Automaton-line units at the same time at the end (issue #36).
  * S10 - The Source of Light:
    * Disallow IftU's special brand of Elvish Enchantress from using the
      Berserker Potion, for what little good it does.
  * S13 - Face Your Fate:
    * Dwarvish Ulfserkers can no longer be recruited once the Warlord arrives
      (issue #44).
  * S20 - The Heart:
    * Unhide side 6 as its leader arrives to the battlefield after turn 1
      (issue #54).
  * S23A - Into the Lair:
    * Now using Aleksi's gameplay06.ogg as the initial track.
  * S23B - Until Death:
    * Using mainline's frantic.ogg during the last part of stage 1.
    * Fixed issues with team color ellipses when Galas gets possessed during
      stage 1 (issue #60).
  * S24 - Epilogue:
    * Minor music and UI tweaks.

* Units:
  * Balancing:
    * Elynia's Thorns I base damage increased by 1 (9-3), Thorns II increase by
      2 instead of 1 (fully upgraded total is now 11-3).
  * Synced descriptions with AtS for a few units that were somehow not already
    synced between IftU 2.0.1 and AtS 0.9.17+.
  * Fixed female Elvish Civilian making male sounds when hit (not killed).
  * Staff-wielding units use the new staff sounds in 1.14.


Version 2.0.1:
--------------
* Graphics:
  * New or updated unit graphics: Faerie Forest Spirit, Elvish Ascetic, Elvish
    Mystic.

* Scenarios:
  * S3 - Memories from the Depths:
    * Keep Mal Keshar's current facing when transferring him at the end of the
      scenario.
  * S5b - Cursed Plateau:
    * Increased turn limit.
    * Remove gold piles when acquired.
  * S14 - Bye and Behold:
    * Increased enemy gold.
  * S21 - Innuendo:
    * Increased turn limit.
  * S22B - The Dark Hive:
    * Replaced the beginning of a pivotal line by Elynia with a rephrased
      version provided by vultraz.
  * S23A - Into the Lair:
    * Increased turn limit.
  * S23B - Until Death:
    * Decreased base HP for the boss from 217 to 208.
    * Shifted boss guards around to delay them engaging in combat with player
      units.
    * The boss can now only recruit up to one Goliath on Hard instead of two.
    * Possessed units regenerate less health.
    * Reduced frequency of Psy Crawler spawns.
    * The boss can only spawn Shaxthal Worms when hit during the last stage on
      Easy difficulty. Also reduced the chance for spawns on all difficulties.
    * The boss can no longer remove negative effects (which is to say, the
      slowed effect) while absorbing damage during the second stage of the
      boss fight. The justification is that this boss does not have the same
      physical prowess as the Chaos Warlord.

* Units:
  * Reworked description and WML for the Intimidates ability granted by the
    special Shardia's Meteor item from S5b.
  * Elvish Avatar (Anlindë) now has AMLAs:
    * Add drains special to melee attack (+25% XP)
    * Increase gossamer strikes by 1 (+25% XP)
  * Redone Lady of Light (Elynia) AMLA tree:
    * Strength I: +5 HP (+25% XP)
      * Thorns I: 8-3 ranged pierce, magical (+25% XP)
    * Strength II: melee damage +1 (+25% XP)
      * Focus I: faerie fire damage +1 (+35% XP)
      * Thorns II: thorns damage +1, drains (+35% XP)
    * Strength III: melee strikes +1 (+25% XP)
      * Focus II: faerie fire strikes +1 (+40% XP)
    * Strength IV: +10 HP, melee damage +1 (+30% XP)
      * Focus III: ensnare strikes +1 (+40% XP)
    * Shielding I: +10% arcane resistance (+30% XP), requires both Focus I and
      Strength III
    * Shielding II: +20% arcane resistance (+50% XP), requires Focus II
  * Removed Thorns attack from the unit type used for Elynia after S23B.
  * Increased base Shaxthal resistances to arcane from -20% to -10%.
  * Increased Chaos Warlord's resistances to arcane from -10% to 0%.
  * Shadow Spawn resistances changed and HP reduced from 29 to 26:
    * Blade/pierce/impact 50% -> 20%
    * Fire 10% -> -20%
    * Cold 70% -> 50%
  * Fixed a cutscene unit type used for Anlindë being always visible in the
    help browser and unit tree.
  * New unit type descriptions: Chaos Cataphract, Hound of Chaos, Demonic
    Hound, Hellhound.
  * Made it so the full list of advancements for the Elvish Civilian display
    in the help browser/unit tree instead of only the male advancements.
  * Rabbits can no longer move into village tiles.


Version 2.0.0:
--------------
* Scenarios:
  * S21 - Innuendo:
    * Minor balancing changes.
  * 22A - Face of the Enemy:
    * Lift shroud prior to highlighting the exit gate during the boss fight.

* Units:
  * New unit type descriptions
    * Shaxthal Assault Drone, Minor Imp, Imp, Blood Imp, Gutwrencher Imp,
      Armageddon Imp, Skeleton Rider (taken from Liberty), Bone Knight.


Version 1.99.8 (codename Reconstruction RC 9):
----------------------------------------------
* Scenarios:
  * Rolled back change from versions 1.99.3 and 1.99.5 that causes auto-recalls
    to become loyal for the remainder of the campaign due to an engine bug in
    the implementation of [object] duration=scenario with certain effects. This
    causes auto-recalls to cost upkeep again in scenarios 2, 3, 4, 5a, 5b, 6,
    8, and 10.
  * S21 - Innuendo:
    * Cleaner (but functionally-equivalent) fix for the SLF issue fixed
      in RC 8.


Version 1.99.7 (codename Reconstruction RC 8):
----------------------------------------------
* Scenarios:
  * S14 - Bye and Behold:
    * Fixed incorrect secondary damage amount in the Explosive Runic Arrows'
      description (50% instead of the actual 80%).
  * S15 - Shadows of Time:
    * Fixed typo in prose.
  * S21 - Innuendo:
    * Make sure the Shaxthal Sentry Drone miniboss doesn't run off to the
      nearest keep.
    * Fix an inexplicable issue where a radial SLF gets doubled when [or]'d,
      resulting in the first chamber near the starting area being matched by
      a late event trigger filter.

* Units:
  * New unit type descriptions:
    * Shaxthal Sentry Drone.
  * Fixed typo in the Chaos Invoker's description.


Version 1.99.6 (codename Reconstruction RC 7):
----------------------------------------------
* Scenarios:
  * S22A - Face of the Enemy:
    * Fixed boss escape countdown in Objectives not updating at the start of
      every turn.
  * S23C - Broken Heart:
    * Added a "Checkpont cleared" alert when clearing checkpoints.

* Units:
  * Balancing:
    * Increased base Union damage from 28-3 to 29-3.
  * New unit type descriptions:
    * Faerie Sprite, Fire Faerie, Faerie Dryad, Faerie Forest Spirit,
      Shaxthal Rayblade.
    * Merged Orcish Nightblade unit description from mainline Wesnoth 1.13.2.
  * Minor tweaks to unit type descriptions:
    * Shaxthal Drone.


Version 1.99.5 (codename Reconstruction RC 6):
----------------------------------------------
* Graphics:
  * New or improved unit animations: Elynia (ranged attack, defense).

* Scenarios:
  * S2 - A Real Confrontation:
    * Forbid Lédinor from abandoning his keep to do something stupid.
  * S7 - Goliath:
    * Force the enemy boss to engage the player by enabling the
      leader_ignores_keep aspect.
  * S9 - The Library:
    * Minor map layout tweaks.
  * S10 - The Source of Light:
    * Auto-recalled units no longer require upkeep for this scenario.
    * Minor map layout tweaks.
  * S13 - Face your Fate:
    * Minor gold tweaks.
  * S14 - Bye and Behold:
    * Mudcrawlers and Water Serpents are not supposed to speak when encountered
      by the player.
  * S19 - Under the Sands:
    * Minor prose tweaks.
  * S20 - The Heart:
    * Minor prose tweaks.
  * S21 - Innuendo:
    * Minor prose tweaks.
  * S22A - Face of the Enemy:
    * Minor prose tweaks.
  * S22B - Dark Hive:
    * Minor prose tweaks.
  * S23A - Into the Lair:
    * Minor prose tweaks.
  * S23B - Until Death:
    * Minor prose tweaks.
  * S23Bx/S23By - Do Us Part:
    * Major prose changes by vultraz.

* Units:
  * New unit type descriptions:
    * Chaos Emperor, Chaos Warlord, Chaos Hound, Demonic Hound, Hellhound,
      Chaos Longbowman, Chaos Heavy Longbowman, Chaos Cavalier, Chaos
      Cataphract, Shadow Minion, Fungoid, Rabbit.
  * Removed E2 Shaxthal Drone variation formerly used in S7 and S9 in versions
    prior to Reconstruction RC 1.


Version 1.99.4 (codename Reconstruction RC 5):
----------------------------------------------
* Graphics:
  * New or updated unit graphics: Chaos Headhunter, Chaos Marauder, Chaos
    Soulhunter.

* Scenarios:
  * S2 - A Real Confrontation:
    * Negligible dialogue tweaks.
  * S8 - Errand of Hope:
    * Clear Althurin's statuses at the end if necessary, so that he does not
      reappear poisoned or slowed in the subsequent cutscene scenario.
  * S23B - Until Death:
    * Make the final boss able to spawn units when damaged during stage 3
      (accidentally disabled in RC 1).
    * Decreased amount of damage regenerated by the final boss when killed by
      the wrong unit during stage 3.
    * Fix Mal Keshar potentially appearing embedded in a wall in stage 3.

* Units:
  * New unit type descriptions:
    * Chaos Arbalestier, Chaos Crossbowman, Chaos Invader, Chaos Bowman, Chaos
      Raider, Chaos Headhunter, Chaos Doom Guard, Chaos Hell Guardian, Chaos
      Dark Knight, Chaos Razerman, Chaos Overlord, Shaxthal Drone, Lady of
      Light, Chaos Invoker, Chaos Magus, Sylvan Warden, Chaos Lorekeeper, Chaos
      Marauder, Chaos Soulhunter.


Version 1.99.3 (codename Reconstruction RC 4):
----------------------------------------------
* Scenarios:
  * Fixed a few typos reported on the forum thread.
  * Auto-recalled speaking units in scenarios 2, 3, 4, 5a/5b, 6 and 8 no longer
    require upkeep for the duration of the scenario in which they were
    auto-recalled.
  * S1 - Border Patrol:
    * Fixed late objectives claiming there is no early finish bonus.
  * S4 - Over the Sands:
    * Re-enabled option to advance to S5b.
  * S5b - Cursed Plateau:
    * Revised scenario.
  * S6 - The Moon Valley:
    * Disabled two unnecessary mid-battle dialogue events.
  * S7 - Goliath:
    * Very minor balancing changes to the boss fight.
  * S10 - The Source of Light:
    * Fixed objectives claiming there is an early finish bonus.
  * S11 - Strike on Herthgar:
    * Removed gold carryover and bonus carryover for this scenario, and changed
      the bonus objective to be a bonusless alternative instead.
  * S12 - The Escape:
    * Adjusted initial settings to permit the most inefficient recruitment
      pattern even without gold carryover from S11.
  * S13 - Face your Fate:
    * Ensured there isn't any gold carried over to S14.
  * S23B - Until Death:
    * Balancing changes to make the fight slightly less of an uphill battle.

* Units:
  * New unit type descriptions:
    * Chaos Arbalestier, Chaos Crossbowman, Chaos Invader.


Version 1.99.2 (codename Reconstruction RC 3):
----------------------------------------------
* Scenarios:
  * Fixed boss AI engine breaking when AtS is not installed.
  * Changed the savegame prefix for both episodes to "IftU", dropping the
    episode number since it's effectively meaningless in practice.
  * S7 - Goliath:
    * Removed all healing glyphs.
  * S14 - Bye and Behold:
    * Added a bare-bones attack animation to the Explosive Arrows item
      (issue #17).


Version 1.99.1 (codename Reconstruction RC 2):
----------------------------------------------
* Scenarios:
  * Removed redundant "(Bonus)" annotation for some objectives in S9, S11, and
    S16.
  * S2 - A Real Confrontation:
    * Fixed pre-captured elven villages not being counted for the scenario
      defeat condition.
  * S3 - Memories from the Depths:
    * Fixed Mal Keshar not speaking one of his lines.
  * S20 - The Heart:
    * Fixed alternate victory by defeating all enemy leaders never triggering
      without using cheats.
  * S21 - Innuendo:
    * Increased turn limit.
  * S23A - Into the Lair:
    * Added a somewhat more elaborate initial sound transition.
  * S23B - Until Death:
    * Fixed an oversight so that player recruits no longer require upkeep.

* Terrains:
  * Ported gate fix from AtS 0.9.1 meant to solve clipping issues for gates
    adjacent to (convex) stone wall corners.

* Units:
  * Door units now clear terrain beneath them on 'last breath' rather than
    'die' events, in order to ensure shroud is correctly cleared before
    scenario-specific event handlers are run.
  * Replaced Chaos Crossbowman and Arbalestier's sword attack with an axe to
    match the sprites.


Version 1.99.0 (codename Reconstruction RC 1):
----------------------------------------------
* General:
  * Raised minimum Wesnoth version requirement from 1.9.10 to 1.12.0.
  * Removed remaining code implementing/referencing the glamour ability.
  * Removed code for story maps that's gone unused for who knows how many years
    due to the campaign's chronic lack of proper story map artwork.
  * Many changes are missing in this changelog, either because they were
    forgotten or because they constitute spoilers.

* Graphics:
  * New or updated terrain graphics: Dark Hive, Dark Hive Surface, Dark Hive
    Depths.
  * New or improved unit animations: Elynia (melee).
  * New or updated unit graphics: Anlindë, Chaos Arbalestier, Chaos Warlord,
    Demon, Demon Zephyr, Demon Grunt, Demon Warrior, Sprite, Fire Faerie,
    Forest Spirit, Dryad, Rabbit, Chaos Emperor.

* Music:
  * All music tracks have been moved to a separate add-on, named "IftU Music".
    This add-on is now an optional dependency for those who can't afford
    downloading it or don't play with music enabled. When absent, the IftU
    campaign menu entries for each episode will include a notice stating so.

* Scenarios:
  * Rewritten or revised all scenarios, including maps. As a result, there are
    too many changes that will not be listed here.
  * Fixed several instances of sighted events taking place prematurely on
    Wesnoth 1.11.x.
  * S2 - A Real Confrontation:
    * Removed Sprites from the player's recruit list.
  * S3 - Memories from the Depths:
    * The Ring of Swiftness now increases movement points by one instead of two.
  * S4 - Over the Sands:
    * Removed Ghouls and Elvish Warrior Spirits from the player's recruit list.
  * S14 - Bye and Behold:
    * Sprites are now added to the player's recruit list here instead of S2.

* Units:
  * Walking Corpses no longer can advance to Ghouls.
  * Elynia's alternate AMLAs heal her.
  * Imps are now immune to the plague weapon special.
  * Removed units:
    * Tiger
    * Verlissh Prong Bug
    * Verlissh Spearbearer line
    * Steppe Orcs faction
    * Aragwaith Peasant
    * Dwarvish Gyrocopter and Dwarvish Steamcopter
  * Renamed Chaos Advanced Crossbowman to Chaos Arbalestier.
  * Renamed Errant Spirit to Errant Soul.
  * Balancing:
    * The Protection ability affects own units of any lower level again instead
      of only level 0 and 1.
    * Granted the new 'precision' weapon special to the Greatbow's ranged
      attack.
    * Increased Psy Mindraider's HP from 58 to 59.
    * Gave feeding ability to Psy Mindraider.
    * Decreased Demon Zephyr's movement cost on deep water terrains from 2 to 1.
    * Decreased Demon Zephyr's movement cost on unwalkable terrains from 3 to 1.
    * Increased arcane damage resistance for most Shaxthal units from -50% to
      -20%.
    * Decreased Shaxthal elusivefoot defense on Deep Water from 20% to 10%
      (Shaxthal Rayblade, Shaxthal Stormblade, Elyssa).
    * Increased Errant Soul's ranged attack strength from 2-1 to 2-2.
    * Changed Leech's alignment from 'lawful' to 'neutral'.
    * Decreased Leech's HP from 62 to 42.
    * Decreased Leech's melee damage from 11-2 to 9-2.
    * Decreased Leech's unit level from 3 to 1.
    * Disabled Elvish Sylph advancement from Elvish Enchantress.
    * Elvish Trapper has skirmisher instead of ambush again.
    * Increased arcane resistance for mechanical units (Worker Droid,
      Automaton, Iron Golem, Goliath) from 30% to 50%.
    * Increased Elynia's resistance to impact damage from -10% to 0%.
    * Decreased the Chaos Emperor's max moves from 6 to 5.
    * Removed skirmisher ability from the Chaos Emperor.
  * Applied changes from bumbadadabum's "The Aragwaithi" add-on, versions 1.0.6
    through 1.0.9, and "Era of Chaos" version 1.3.1+dev up to commit
    9dedeba7cddc2a027745c9994a917fdcb78ed341:
    * Archer HP increased from 26 to 28.
    * Granted the new 'precision' weapon special to the Greatbow's ranged
      attack.
    * Increased Guard's blade resistance from 10% to 20%.
    * Increased Guard's XP from 64 to 74.
    * Decreased Guard's cost from 28 to 27.
    * Decreased Pikeman's cost from 38 to 28.
    * Increased Shield Guard's cost from 37 to 45.
    * Increased Shield Guard's blade and pierce resistances from 10% to 20%.
    * Granted the 'marksman' weapon special to the Swordsmaster.
    * Renamed the Aragwaith Witch's image files.
  * Fixed Chaos Arbalestier ranged attack animation failing to trigger.
  * Fixed unit types with missing faction prefixes in their names:
    * Arbalestier -> Chaos Arbalestier
    * Cataphract -> Chaos Cataphract
    * Crossbowman -> Chaos Crossbowman
    * Heavy Longbowman -> Chaos Heavy Longbowman
  * Fixed multiple "Descriptions should no longer include the name as the first
    line" warnings on 1.11.1 and later.
  * Fixed "Terrain '**' has evaluated to 100 (cost) [...]" warnings on Wesnoth
    1.11.x caused by Aragwaith units.
  * Replaced old bird NPC behavior code with the newer Lua-based implementation
    from AtS.
  * Removed help markup from the Sylvan Essence ability special notes to avoid
    issues in Pango contexts (e.g. sidebar tooltips).
  * Removed references to nonexistent image files in the defense animations for
    female Elvish Trapper and Elvish Prowler units.
  * Fixed recruited elvish units from scenario 4 onwards belonging to hidden
    unit types.
  * New unit type descriptions:
    * Demon, Demon Zephyr, Demon Grunt, Demon Warrior
    * Elvish Civilian
    * Elvish Hunter, Elvish Trapper, Elvish Prowler
    * Sylvan Warden
  * Fixed a minor inaccuracy at the beginning of the Terror ability
    description.
  * New or improved unit animations: multiple Aragwaith units.

* User interface:
  * Made sure cutscene theme with menu bar works on Wesnoth 1.11.5 and later
    (affecting S8x, S14xA, S14xB, S16x, S20x, S23By).
  * Cutscene themes now use the 1.11.10 [theme] id attribute on 1.11.10 and
    later.


Version 1.90.7:
---------------

- Increased minimum Wesnoth version requirement from 1.9.6 to 1.9.10; dropped
  support for 1.9.9 and earlier.

- Various internal code improvements and clean-up.

- Graphics:
    - New or updated unit graphics: most Aragwaith units (wayfarer), Sprite,
      Fire Faerie, Forest Spirit, Dryad, Shaxthal Assault Drone, Shaxthal
      Protector Drone, Shaxthal Runner Drone, Shaxthal Rayblade, Abomination.

- Language and i18n:
    - Various fixes.
    - Updated translations from WesCamp-i18n: fr, it, ru

- Scenarios:
    - Minor cosmetic changes on various maps.
    - Replaced character descriptions prompt on startup with a custom GUI2
      dialog.
    - Updated maps for compatibility with Wesnoth 1.11.x.
    - Various grammar, style, and punctuation fixes or changes.
    - 4
        - Allowed units to be hydrated on water terrains with overlays.
    - 5A
        - More terrain variety.
    - 10
        - Removed deprecated Ggf terrain (changed to Gg^Efm).
    - 13
        - Minor dialog changes.
    - 14
        - Fixed the dwarven chainmail armor resistances so it has the advertised
          effect.
        - Made it so that when Galas gets the dwarven chainmail armor, he also
          gets a special trait to remind the player of the resistance bonuses
          the armor gives.
    - 15
        - More terrain variety.
    - 16
        - More terrain variety.
    - 18
        - More terrain variety.
    - 19
        - More terrain variety.
    - 22A
        - The Amulet of the Arcane Flows should now actually boost its owner's
          arcane resistance.
    - 22B
        - Minor dialog changes.
    - 22C
        - Minor dialog changes.
    - 23B
        - Made it so that Rurhló and Garg are recalled in the second part.

- Units:
    - Balancing:
      - Farmland no longer applies for the effects of the Sylvan Spark and
        Sylvan Essence abilities.
      - Increased Sprite's impact resistance from -20% to 0%.
      - Increased Fire Faerie's impact resistance from -20% to 0%.
      - Increased Dryad's impact resistance from -10% to 0%.
    - Fixed AMLA XP requirement for the Psy Crawler and Shadow Courier unit
      types.
    - Fixed flickering during Elynia's ranged pierce attack animation caused by
      references to removed images.
    - Fixed flickering during Anlindë's defense animation caused by references
      to non-existent images.
    - Made it so that the Aragwaithi Captain line's protection ability doesn't
      interfere with resistances higher than 50%.
    - Ported some animation code, description, and stat changes from AtS.
    - Replaced Shaxthal Wyrm unit type with AtS's Shaxthal Worm.
    - Made it so that the Runner Drone can advance to the Rayblade instead of
      the Assault Drone.
    - Rewrote several unit descriptions.
    - Updated Aragwaith units to match the faction from bumbadadabum's
      "The Aragwaithi" add-on. This has resulted in the following changes:
      - Protection only affects allied L1 and L0 units instead of any allied
        lower level unit
      - Ancient Banner abilities: +leadership, -protection, -steadfast
      - Ancient banner resistances: impact 10% -> 20%
      - Ancient banner stats: HP 55 -> 58, MP 4 -> 5
      - Ancient banner attacks: sword renamed to scythe
      - Archer attacks: melee 6-3 -> 4-3
      - Captain abilities: +leadership, -protection, -steadfast
      - Captain resistances: blade 20% -> 10%, fire 10% -> 0%, cold 10% -> 0%,
        pierce 20% -> 10%
      - Captain stats: HP 43 -> 55, MP 4 -> 5
      - Captain attacks: spear renamed to glaive, 17-2 -> 18-2; sword renamed to
        glaive, 9-4 -> 10-4
      - Eagle Master stats: HP 48 -> 45, MP 7 -> 9
      - Eagle Master attacks: blade 9-3 -> 10-3, impact 15-2 -> 16-2
      - Eagle Rider defense: mountain 60% -> 50%
      - Eagle Rider stats: HP 36 -> 34, MP 7 -> 9, cost 21 -> 23
      - Eagle Rider attacks: impact 10-2 -> 12-2
      - Flagbearer abilities: +leadership, -protection, -steadfast
      - Flagbearer resistances: blade 20% -> 10%, fire 10% -> 0%, cold 10% ->
        0%, pierce 20% -> 0%, impact 10% -> 0%
      - Flagbearer stats: HP 34 -> 45, MP 4 -> 5
      - Flagbearer attacks: spear renamed to glaive, sword renamed to glaive
      - Greatbow stats: HP 43 -> 46, MP 5 -> 6
      - Greatbow attacks: melee 13-3 -> 10-3
      - Guard abilities: +steadfast
      - Guard resistances: pierce 20% -> 10%, impact 20% -> 10%, blade 30% ->
        10%
      - Guard stats: HP 40 -> 54, XP 78 -> 64, cost 27 -> 28
      - Guard attacks: melee 12-3 -> 11-3
      - Guardian resistances: fire 10% -> 0%, cold 10% -> 0%
      - Guardian stats: HP 51 -> 62
      - Lancer now has a female variation
      - Lancer stats: HP 40 -> 48, cost 38 -> 34
      - Longswordsman stats: HP 38 -> 46, MP 5 -> 6, XP 78 -> 88, cost 24 -> 27
      - Pikeman resistances: blade 20% -> 10%, impact 10% -> 0%, fire 10% -> 0%,
        cold 10% -> 0%
      - Pikeman stats: HP 44 -> 50, XP 94 -> 70
      - Pikeman attacks: melee 17-2 -> 16-2
      - Scout now has a female variation
      - Scout stats: HP 31 -> 36, XP 36 -> 40
      - Scout attacks: melee 10-2 -> 11-2
      - Shield Guard abilities: +protection, +steadfast
      - Shield Guard resistances: pierce 30% -> 10%, impact 30% -> 10%, blade
        40% -> 10%
      - Shield Guard stats: HP 54 -> 66
      - Shield Guard attacks: melee 16-3 -> 15-3
      - Silver Shield now has a female variation
      - Silver Shield stats: HP 54 -> 62, MP 8 -> 9, cost 38 -> 48
      - Silver Shield attacks: melee 13-4 -> 12-4
      - Slayer stats: HP 45 -> 53, MP 5 -> 6, cost 46 -> 62
      - Slayer attacks: melee 12-4 -> 11-4
      - Sorcerer renamed to Sorceress, no longer has a male variation
      - Spearman resistances: blade 20% -> 0%, pierce 20% -> 10%, impact 10% ->
        0%, fire 10% -> 0%, cold 10% -> 0%
      - Spearman stats: HP 30 -> 34, XP 38 -> 43
      - Spearman attacks: 11-2 -> 12-2
      - Strongbow stats: HP 35 -> 38, MP 5 -> 6, XP 80 -> 85, cost 31 -> 38
      - Strongbow attacks: melee 9-3 -> 7-3, ranged 8-4 -> 9-4
      - Swordsmaster id changed, breaking old saved games with the unit
      - Swordsmaster stats: MP 5 -> 6
      - Swordsman resistances: blade 10% -> 0%
      - Swordsman stats: HP 28 -> 32, XP 32 -> 39, cost 13 -> 14
      - Warlock renamed to Witch, no longer has a male variation
      - Witch stats: XP 44 -> 54, cost 18 -> 22
      - Witch attacks: staff renamed to kick, 6-2 -> 7-1
      - Wizard no longer has a male variation
      - Wizard attacks: melee 10-2 -> 7-2, ranged 11-3 -> 10-3


Version 1.90.6:
---------------

- Language and i18n:
    - Various fixes.

- Scenarios:
    - 23B
         - Worked around an engine bug to ensure that the Shadow Master
           appearance event and the aggressive shaxthal respawn event trigger.
    - 23Cx
         - Fixed syntax errors in a [color_adjust] block.
    - 24
         - Fixed syntax errors in a [color_adjust] block.

- Units:
    - Sprite tree, Lady of Light, and Sylvan Warden: made it so that the ring
      haloes in the mystic fire animation do not get vertically flipped
      when attacking in the southern directions.


Version 1.90.5:
---------------

- Units:
    - Updated AMLA XP requirements to match mainline on 1.9.10 and later.


Version 1.90.4:
---------------

- Scenarios
    - 23C
         - Made it so that Rurhló and Garg aren't recalled.


Version 1.90.3:
---------------

- Graphics:
    - Introduced Elynia's sprite from After the Storm.

- Scenarios:
    - Recall Rurhló and Garg in non-cutscene scenarios after Innuendo.

- Units
    - Brought back the old Falcon unit since it will no longer be in mainline
      starting with 1.9.10.
    - Made use of image_icon= in the Verlissh Matrix Core and the Verlissh
      Matrix Flow System units to enhance experience in 1.9.10 and beyond.


Version 1.90.2:
---------------

- Graphics:
    - New or updated unit graphics: Shaxthal Drone, Shaxthal Runner Drone,
      Shaxthal Sentry Drone.
    - Removed the old Elvish Fighter and female Elvish Archer portraits;
      wired the new ones into the Elvish Civilian.

- Scenarios:
    - Added bonus/gold carryover notes
    - 8
        - Anlindë and Mal Keshar are now properly recalled at the start of the
          scenario

- Terrains:
    - Improved wasteland-water transitions

- User interface:
    - Fixed glitches at the start of scenario 14, Bye and Behold, when starting
      Episode II from the campaigns menu.
    - Removed map borders overlay from fullscreen cutscene UI.

- Units:
    - The following units are no longer affected by plague: Spearbearer,
      Light Assault Tropper, Heavy Assault Trooper.


Version 1.90.1:
---------------

- User interface:
    - Improved custom themes for use in cutscenes, from AtS.


Version 1.90.0:
---------------

- Ported to Wesnoth 1.9.2+.

- i18n and l10n:
    - New translations from WesCamp-i18n: ja

- Graphics:
    - New unit portraits: L1 Demon (male), L1 Demon (female).

- Units:
    - Balancing:
        - Removed Skirmisher from Elynia.
        - Removed Glamour
    - New NPC bird behavior code.


Version 1.70.2:
---------------

- i18n and l10n:
    - Updated translations from WesCamp-i18n: es, fr, hu, it, nl, ru, tr

- Units:
    - Balancing:
        - Decreased Shaxthal Razordbird's HP from 32 to 26
        - Decreased Shaxthal Thunderbird's HP from 44 to 39


Version 1.70.1:
---------------

- Scenarios:
    - 7 (The Elf and Goliath):
        - Fix extremely coward boss AI.
    - 8 (Errand of Hope):
        - Got rid of the nagas.
        - Made several changes in the initial dialog sequence.
    - 10 (Source of Light):
        - Set a sensible minimum amount of gold for the player.
    - 11 (Strike on New Knalga):
        - Set a sensible minimum amount of gold for the player.

- Units:
    - Balancing:
        - Increased imps' resistances to arcane damage from -50% to -10%
        - Increased Armageddon Imp's resistance to impact damage from 10% to 20%
        - Increased Minor Imp's resistance to impact damage from -50% to -20%
        - Reset Regular Imp's resistances to the base values for the impfoot
          movetype
        - Changed Demon Zephyr's resistances as follows:
            - Blade: 20% -> 0%
            - Impact: 10% -> 0%
            - Arcane: -50% -> -10%
            - Cold: -10% -> 0%
        - Changed Demon unit tree resistances as follows:
            - Blade:
                - Base: 20% -> 0%
                - Grunt: 40% -> 20%
                - Warrior: 50% -> 20%
            - Pierce:
                - Grunt: 20% -> base
                - Warrior: 40% -> 10%
            - Impact:
                - Base: 10% -> 0%
                - Grunt: 20% -> 10%
                - Warrior: 30% -> 20%
            - Arcane: -50% -> -10%
            - Cold:
                - Base: -10% -> 0%
                - Grunt, Warrior: base -> 10%
        - Changed Shaxthal Warlord's resistances as follows:
            - Blade: 30% -> 20%
            - Fire: base -> 30%
            - Arcane: -50% -> -10%
        - Increased Shaxthal Warlord's hitpoints from 190 to 196
        - Changed Master of Darkness' resistances as follows:
            - Impact: 20% -> 30%
            - Pierce: 40% -> 30%
            - Arcane: 20% -> -10%
        - Increased Mechanical Goliath's base hitpoints from 58 to 61
        - Increased Automaton's hitpoints from 36 to 38
        - Increased Worker Droid's hitpoints from 17 to 20
    - Removed units: Sand Troll line
    - The following units are no longer affected by plague: Fungoid, Giant Ant,
      Lesser Giant Spider, Leech, Giant Leech, Brain Drainer Leech, Crow,
      Falcon, Rabbit, Eyestalk.


Version 1.70.0:
---------------

- Administration and maintenance:
    - Minimum Wesnoth version requirement is 1.7.6

- Graphics:
    - New or updated unit graphics: Demon, Demon Zephyr, Elvish Ascetic, Elvish
      Mystic, Shaxthal Sentry Drone, Shaxthal Warlord, Shaxthal Protector Drone,
      Shaxthal Runner Drone, Shaxthal Master Drone, Elvish Avatar, Demon
      Grunt, Demon Warrior, Skeleton Rider
    - New portraits: Shadow Master

- Language and i18n:
    - Applied SouthernOracle's revisions of all scenarios and both episodes'
      story text.

- Plot, storyline and background:
    - Renamed Yanqui to Zhangor (reflects mainline change).

- Scenarios:
    - 4 (Over the Sands):
        - Apply dehydration/hydration over the human player's units only.
        - Completely rewrote this scenario.
    - 6 (The Moon Valley):
        - Made some changes in the scenario design for balancing
        - Fix long delay when loading saved games of a different scenario or
          start menu when music is enabled.
    - 12 (The Escape):
        - Fixed objectives reset code not being executed again after the first
          enemy leader is defeated.
    - 22B (Face of the Enemy):
        - Renamed (was "Gauntlet").
    - 23C (Broken Heart):
        - Fixed a WML/Formula syntax problem that made an essential event not
          trigger until the end of the scenario.
          (http://www.wesnoth.org/forum/viewtopic.php?p=363314#p363314)

- Terrains:
    - Fixed more transition issues with gates and walls of any kind.
    - Fixed base terrain issues with the campfire overlay.

- Units:
    - Balancing:
        - Reduced Sylvan Warden's melee attack strength from 6-5 to 6-3.
        - Reduced Lady of Light/Sylvan Warden's movement points from 7 to 6.
        - Reduced Lady of Light/Sylvan Warden's movement cost over deep water
          from 5 to 4.
    - Fix animation filter issues with Chaos Longbowmen.
    - Removed units:
        - Caravan


Version 1.12.0:
---------------

- Administration and maintenance:
    - Minimum Wesnoth version requirement is 1.5.14 (1.6 RC3).

- Scenarios:
    - 03 (Memories from the Depths):
        - Do not offer loyal undead on any difficulty level.
    - 22B (The Gauntlet):
        - Made it possible for matrix components to attack the player.
    - Alien units are not available until scenario 19.

- Terrains:
    - Fixed awkward lack of Dirt <-> dark-tile Road transitions.
    - Fixed some transition issues with gates and brick walls.

- Units:
    - Balancing:
        - The player cannot recruit Ghouls anymore - however, they are still
          available as an alternate advancement for Walking Corpses.


Version 1.11.1.1:
-----------------

- Scenarios:
    - Applied some more text revisions from Solsword.
    - Revised some maps.

- Terrains:
    - Fixed awkward lack of Dirt <-> Hive transitions.


Version 1.11.1:
---------------

- Administration and maintenance:
    - Bumped minimum Wesnoth version requirement to 1.5.10, and dropped
      compatibility with IftU 1.10.3 and earlier, and Wesnoth 1.5.9 and earlier.

- Graphics:
    - Removed portraits: Murlin.
    - Updated baseframes: Water Serpent.

- Scenarios:
    - Fixed some plot holes.
    - Revised some maps.
    - Applied a user-contributed patch to the English text (from Solsword).
    - The Ring of Regeneration may not be used by faeries, units of the Elvish
      Shaman line, or Anlindë.
    - The Berserk Potion may not be used by faeries, units of the Elvish Shaman
      line, Anlindë, Mal Keshar, or units of the Walking Corpse or Ghoul lines.
    - Re-enabled custom AI formulas for dark hive guardians in final scenarios.
    - 24 (Epilogue):
        - Fixed a map size issue that caused Wesnoth 1.5.11+ to abort.

- Units:
    - Balancing:
        - Force Cockatrices to use only their ranged attack on offensive
          strikes.
        - Reduced Elvish Prowler's HP from 62 to 54.
        - Replaced Elvish Trapper's skirmishing ability with ambush.


Version 1.11.0:
---------------

- Graphics:
    - Updated baseframes: Shaxthal Rayblade, Shaxthal Master Drone (masked and
                          unmasked), Shaxthal Warlord (masked and unmasked),
                          Water Serpent.
    - Updated portraits: Elyssa (masked and unmasked) [D].

- Scenarios:
    - New scenarios:
        - 22C (The Dark Hive)
        - 23A (Frozen Hell)
    - Removed scenarios:
        - 23A (Interim)
    - Scenario 14 (Bye and Behold):
        - Fixed King Asthorgar not getting his portrait when starting
          Episode II from scratch.

- Units:
    - Balancing:
        - Gave real shaxthal stats to Elyssa.
            - Replaced "infernal chill" (cold, ranged, magical 15-2) with the
              more powerful "burning inferno" (fire, ranged, magical 14-3).
            - Gave her the Submerges ability.
            - Reduced her "sword" attack strength (melee, blade, drains 12-4) to
              11-4.
        - Made the Water Serpent a level 2 unit. 'nuff said.
    - Merged Elynia's union attack animation into her unit.
    - Removed Elvish Horseman unit due to artwork requirements and balancing.


Version 1.10.5:
---------------

- Administration and maintenance:
    - Began to use inline formulas in WML to decrease code complexity. This
      means that this campaign will not work properly in Wesnoth 1.5.6 or
      earlier.
    - Saved games of the last boss fight and afterwards may no longer work.

- Graphics:
    - Updated baseframes: Elynia, Master of Darkness, Elvish Mystic,
                          Elvish Avatar, Shaxthal Protector Drone.
    - Updated portraits: Lédinor [D], King Asthorgar [D].

- Scenarios:
    - 8 (Errand of Hope):
        - Slight improvements to the initial custscene.
    - 8 - final cutscene (A Royal Meeting):
        - Fixed probably the most half-assed dialog sequence in this campaign's
          history. Damnit, there were even a few plot contradictions in it.
    - 10 (The Source of Light):
        - Removed the possibility of giving the draining potion to faerie
          beings and undead spirits (reported by TheJM).
    - 22A, 22B, 23A, 23B:
        - Fixed WML that invoked undefined behavior from the vconfig engine.
          This change means you've got to restart "Innuendo" or the last turn
          of The Heart to update your saves, since otherwise the recall list
          for the last scenarios will be unusable.
        - Prohibited plagued units (Walking Corpses, Soullesses, Ghouls) from
          being carried over to next scenarios.
    - 22A (Innuendo):
        - Removed one recall/recruitment hex for the player.
    - 22B (Gauntlet):
        - Major map revisions.

- Units:
    - Balancing:
        - Increased Aragwaith Sorcerer's total movement from 5 to 6.
        - Increased Chaos Hound's HP from 21 to 22.
        - Increased Hellhound's HP from 44 to 47.
    - Fixed glitchy animations:
        - Bone Knight
    - Removed unused units:
        - Bear
        - Giant Boar
    - Renamed units:
        - Sylvan Faerie -> Sylvan Warden


Version 1.10.4:
---------------

- Graphics:
    - Updated portraits: Igor [D], Galas [D], Mal Keshar [D], Anlindë [D],
                         Elynia [D], Lédinor [P], Mal Hekuba [P].

- Language and i18n:
    - Cleaned up usage of textdomains.
    - Brought back translations from WesCamp-i18n into the official
      distribution: French, Italian, Spanish, Turkish.

- Music and sound effects:
    - Removed battle6.ogg since it's been included in the official Wesnoth
      mainline distribution as suspense.ogg since 1.5.7.

- Scenarios:
    - Fixed a few typos or removed inexisting words.
    - 1 (Border Patrol):
        - Fixed a text overflow issue in the story screens.
    - 5 (Crossfire, Cursed Plateau):
        - Gave a more visible indication that Dark Adepts are recruitable in
          these scenarios.
    - 22A (Innuendo):
        - Removed a coffin that was floating over abyss.
        - Some "minor" revisions.
    - 23C (Broken Heart):
        - Some "minor" revisions.

- Units:
    - Balancing, including changes after mainline revision 32126:
        - Reduced Shaxthal Rayblade's movement costs:
            - Deep water: 4 -> 3
            - Shallow water: 3 -> 2
            - Swamp water: 3 -> 2
        - Increased Shaxthal Rayblade's defense on deep water from 10% to 20%.
        - Reduced Shaxthal Rayblade's defense on reef terrain from 40% to 30%.
        - Reduced Shaxthal Runner and Protector's defense on reef terrain from
          40% to 30%.
        - Reduced 'aragwaithfoot' movetype defense on reef and swamp
          water terrains from 40% to 30%.
        - Reduced 'aragwaithmounted' movetype defense on reef terrain from 40%
          to 30%.
        - Reduced Doom Guard's line defense on reef terrain from 30% to 20%.
        - Reduced 'impfoot' movetype defense on reef terrain from 50% to 40%.
        - Reduced 'impfoot' movetype defense on shallow water from 40% to 30%.
        - Reduced 'impfoot' movetype defense on swamp water from 60% to 40%.
        - Reduced 'demon' movetype defense on reef terrain from 50% to 40%.
        - Reduced 'demon' movetype defense on shallow water from 40% to 30%.
        - Reduced 'demon' movetype defense on swamp water from 60% to 50%.
        - Reduced 'undeadmountedfoot' movetype defense on reef terrain from 40%
          to 30%.
        - Reduced 'steppebasic' movetype defense on reef terrain from 40% to
          30%.
        - Reduced 'steppelusive' movetype defense on reef terrain from 50% to
          40%.
        - Reduced 'steppescout' movetype defense on reef terrain from 40% to
          30%.
        - Reduced 'mutantfoot' movetype defense on reef terrain from 50% to 40%.
        - Removed unused movetype, 'crawlerfoot'.
        - Reduced Steppe Savage's defense on reef terrain from 50% to 40%.
        - Reduced Elynia's defense on reef terrain from 50% to 40%.
    - Gave the Dwarvish Runesmith proper attack icons.


Version 1.10.3:
---------------

- EXPERIMENTAL [U]:
    - Make Galas, Mal Keshar, Erathan Althurin and Igor use kitty's transparent
      portraits in 1.5.7.

- Administration and maintenance:
    - Removed unused, deprecated and/or unmaintained files:
        - SPOILERS
        - TEXT_SOURCES

- Graphics:
    - New portraits: Mal Keshar [D]

- Scenarios:
    - 3 (Memories from the Depths):
        - Faerie spirits aren't supposed to be able to take the Ring of
          Switftness.
    - 4 (Over the Sands):
        - Merged from upstream (/trunk/data/campaigns/Under_the_Burning_Suns):
            - revision 31828 <zookeeper> Added a little overlay icon to
              dehydrated units.
              (Tue Dec 30 21:38:13 2008 +0000)
            - revision 31840 <zookeeper> Allowed villages to rehydrate units.
              (Wed Dec 31 17:55:05 2008 +0000)
            - revision 31841 <zookeeper> Fixed rehydration screwing up attack
              stats of units that leveled up after getting dehydrated.
              (Wed Dec 31 18:16:45 2008 +0000)
    - 5a (Crossfire), 5b (Cursed Plateau):
        - Faerie spirits aren't supposed to be able to take the Ring of
          Regeneration.
    - 9 (The Library):
        - Fixed enemy respawn points.
    - 10 (The Source of Light):
        - Faerie and elvish spirits aren't supposed to be able to take the
          Draining potion.
        - Text revisions, including a few English variant fixes (e.g. UK
          English in middle of US English). Also gave Igor more stuff to say.
    - 14 (Bye and Behold):
        - Make Igor available when starting episode II on HARD.
    - 21 (The Heart):
        - Fix graphic glitches.
        - Fix an "invalid WML" warning.
    - 22A (Innuendo):
        - Blocked entrance to secret scenario.
        - Fixed spelling mistakes.
        - Made the filters for objects that may be applied only to living
          beings exclude Faerie Spirits as well.
        - Revised dialog and objectives text.
    - 22B (The Gauntlet):
        - Revised dialog text.
    - 22C (The Backyard):
        - Removed unbalanced and unmaintained scenario, "The Backyard".

- Units:
    - Made Anlindë's unit line visible in the help engine again.
    - Removed units: Captain, Commander, Dark General, Swordsman (mainline
                     override), Man at Arms, Champion, Crossbowman, High Guard,
                     Deathguard.


Version 1.10.2:
---------------

- Maintenance toolchain:
    - Made build-external-archive.sh use uname instead of GNU distribution-
      specific environment variables. Also, fill the PUBLISH tag with a bit more
      of information. In the future I'll probably use GnuPG to sign packages.
    - Updated the WMLDIRS and IMPORTDIRS tags.

- Scenarios:
    - 3 (Memories from the Depths):
        - Cosmetic and consistency fixes on the map.
        - Erase a duplicated 'not' in the initial dialogue.
    - 4 (Over the Sands):
        - http://www.wesnoth.org/forum/viewtopic.php?p=328014#p328014:
            - Force dehydration/hydration to operate only on units located
              on the gamemap.
            - Removed an accidentally copy & pasted unit filter that
              hydrated on victory only those units that would have been
              hydrated on the next turn (stepping on water hexes, blah blah).

- Units:
    - Fix a small mistake in Galas' character description text.


Version 1.10.1a:
----------------

- Graphics:
    - New portraits: Althurin [D]

- Scenarios:
    - 12 (The Escape):
        - Balancing changes.
    - 21 (The Heart):
        - Balancing changes.
        - Fixed an "invalid WML" warning

- Units:
    - Fixed all instances of UNREACHABLE with the macro of the same name.
    - Refactoring of Elynia's unit code.
    - Removed units: City Guard.


Version 1.10.1:
---------------

- Graphics:
    - New portraits: Igor [D]
    - Updated unit graphics: Elynia, Elvish Mystic, Elvish Avatar, Blood Imp,
                             Demon, Demon Zephyr

- Scenarios:
    - Subtle storyline changes since 1.10.0 (applies HISTORY and CHARACTERS,
      which are not distributed officially yet)
    - 8 (Errand of Hope):
        - Balancing changes.
        - Fixed some invalid WML warnings
    - 10 (The Source of Light):
        - Balancing changes.
        - Dialog revisions.
    - 11 (Strike on New Knalga):
        - Balancing changes.
        - Dialog revisions.
        - Fixed an Unknown-Unit-Type schroedinbug (i.e. improbably triggered in
          practice - which is still a Bad Thing since it was part of an
          enemy's recruit list).
    - 12 (The Escape):
        - Balancing changes.
    - 14 (Bye and Behold):
        - Balancing changes.
    - 15 (Shadows of Time):
        - Cosmetic/balancing changes: the enemy recruits random Walking Corpse
          variations from a set that seems to fit the map.
    - 16 (Arrival of the Battalion):
        - Balancing changes.
    - 17 (Dawn of the Great War):
        - Removed reference to Wose recruitment in a dialog (a left-over from
          ancient releases).
    - 19 (Legend of Wesmere):
        - Fixed a typo in one of Erathan's lines.
    - 20.5 (The Plot):
        - Althurin no longer "kills" King Asthorgar.
    - 21 (The Heart):
        - Make Althurin's first-time description available when starting
          straight from episode II.

- Units:
    - Balancing:
        - Player's Dark Adepts can advance to Liches.
          THIS CHANGE BREAKS OLD SAVED GAMES.
    - Fixed Elvish Avatar's ranged arcane attack animation.
    - Removed Elvish Protector for not fitting the quality requirement for this
      series.


Version 1.10.0 (interim release):
---------------------------------

- Ported from 1.4 branch to trunk. Cycholka/Mist ran wmllint on it for
  making it compatible with Wesnoth 1.5.1 and later.
- Prevented past-the-end WML array access using new macros,
  VARIABLE_RANDOM_SUBSCRIPT and RANDOM_SUBSCRIPT.
  All WML found with the regular expression /\.\.\$[a-zA-Z0-9_]*\.length/
  was fixed to use this method.
- Removed many unused macros.
    - Ditch IS_ON_MAP in favor of mainline NOT_ON_RECALL_LIST.
- Switched back from ~ preprocessor includes to @, which allows IftU to be
  loaded from a mainline datadir if present. This is completely absurd IMO, but
  users of our SVN trunk have the weird habit of making the checkout in such
  exotic locations...

- Graphics:
    - Added baseframes: Elvish Civilian (bow attack), Elvish Avatar,
                        Elvish Ascetic
    - Added portraits: Elvish Civilian male [P] and female [P]
    - Gave Elynia a separate standing animation when she's over water,
      impassable or unwalkable terrains - she also uses this animation while
      moving.
    - New original portraits by Kitty: Galas [D], Anlindë [D], Elynia [D],
                                       Erathan [D]
    - Removed now unnecessary generic portraits: Lich, Dark Adept,
      female Dark Adept
    - Updated baseframes: Elynia, Elvish Civilian, Blood Imp, Shaxthal Drone,
                          Shaxthal Assault Drone, Shaxthal Wyrm, Elvish Prowler,
                          Elvish Trapper
    - Updated portraits: Dryad [P]

- Language and i18n:
    - Changed unit race text for female Demons from "race+female^Demon"
      to "race+female^Demoness".
    - Changed female unit_type names for the Demon tree to be of the
      "Demoness" form rather than "Demon".

- Music and sound effects:
    - Added battle7.ogg, a work-in-progress music piece by Rain that I liked. :)
    - Removed West's "sad.ogg" since its mainline original, "nr-sad.ogg" is
      being moved to a public location reachable by this campaign.

- Scenarios:
    - Added first-time description for Elynia, Erathan and Althurin.
    - Character first-time descriptions and the option to skip them are enabled
      when starting straight from episode II.
    - Changed all instances of "alright" to more formal expressions as
      suggested by Espreon.
    - Player can choose Galas initial unit type when starting straight from
      episode II.
    - Revised glamour ability WML and enabled HP changes (still quirky due to
      engine bugs on arithmetic with WML variables containing real numbers)
    - Sanitized many event unit filters.
    - Some dialogs were improved (Shadow Master alone, with nobody's help!
                                  mwahahahahahhaaa!!!)
    - Turned Anlindë from Elvish Sorceress into Elvish Ascetic.
    - 1 (Border Patrol):
        - Map balancing.
    - 2 (A Real Confrontation):
        - A few dialogue improvements at the start - they also involve changes
          on the free recall mechanics.
        - Add an explanation for the Elvish civilians.
        - Other balancing changes.
    - 4 (Over the Sands):
        - New dehydration logic from Under the Burning Suns.
    - 5a (Crossfire):
        - Added more gold income to some enemy sides.
        - Status balancing.
        - Map balancing.
        - Units can no longer move to the "green side" of the map.
    - 6 (The Moon Valley):
        - Yeti is not a blocker for victory.
    - 7 (The Elf versus Goliath):
        - Added Fog of War.
        - Increased overall difficulty.
        - Increased level of demon enemies.
        - Strength potion's filter is more strict regarding non-living beings.
    - 9 (The Library):
        - Galas movement costs in cave terrains don't get reduced on hardest
          difficulty.
    - 10 (The Source of Light):
        - Made berserk potion have effect only until the end of this scenario.
        - Mal Keshar explains why Elynia hid herself in this cave.
        - Fixed some awkward grammar
          (http://www.wesnoth.org/forum/viewtopic.php?p=305960#p305960)
    - 16 (Arrival of the Battalion):
        - Fixed a bug which made Quogar Ratham always speak a line that Erathan
          is supposed to speak otherwise.
    - 17 (Dawn of the Great War):
        - Fixed insane music fade-out delay after the initial character dialog.
    - 22B (Gauntlet):
        - Did significant clean-ups, removing most variables and all macros
          that were used before.
        - Drones now use Formula AI rules.
    - 22C (The Backyard):
        - This scenario is no longer enabled. The code will be left around for
          two more releases, but it will be disabled unless the WML preprocessor
          symbol HAVE_BACKYARD is defined.
    - 23A (Interim):
        - Clean-ups.
        - Reduced turn limit.
    - 23B (Welcome to the Lair of the Shadow Master):
        - Boss can now recruit units.
        - Changed controller for side of door units from 'ai'
          to 'null'.
        - Increased turn limit by 100; scenario starts at the
          turn that "Interim" was finished plus one
        - Made many changes to this scenario, making the boss fight
          far harder, fixing old bugs, and changing the former balance.

- Terrains:
    - Made Dark Road terrain play better with castle/keep terrain types
      (C*, K*).
    - Renamed many terrain types, rendering some old saved games unusable.
    - Revised most of the terrain graphics layout code to be 1.5.x-compatible.

- Units:
    - Added units: Chaos Raider, Chaos Cavalier, Chaos Cataphract,
                   Chaos Bowman, Chaos Longbowman, Chaos Crossbowman,
                   Chaos Heavy Longbowman, Chaos Advanced Crossbowman,
                   Elvish Ascetic (character), Elvish Mystic (character),
                   Elvish Avatar (character).
    - Balancing:
        - Added farmland to vegetated terrains list
        - Elynia's AMLAs:
            - AMLA 0 (unbound): new attack (thorns, ranged, pierce,
              magic) -> (removed)
            - AMLA 1: melee +1D, HP +5 <FH> , XP +20% -> HP +5, XP +30%
            - AMLA 2: melee +1S, HP <FH>, XP +30% -> melee +1D, XP +45%
            - AMLA 3: melee +1D, HP <FH>, XP +40% -> melee +1S, XP +60%
            - AMLA 4: melee +1S, HP <FH>, XP +50% -> ranged +
              thorns <ranged, pierce> [magic] 7-3, XP +75%.
        - Gave most units adequate movement costs and defense
          on Reef terrain.
        - Imps may receive the traits Weak, Slow or Dim.
        - Increased Shaxthal Razorbird's resistance to damage as follows:
            - Blade: 0% -> 10% <base>
            - Pierce: 0% -> 10%
        - Increased Shaxthal Thunderbird's resistance to damage as follows:
            - Blade: 0% -> 10% <base>
            - Pierce: 0% -> 20%
        - Increased Worker Droid's movement costs as follows:
            - Shallow Water: 3 -> 4
            - Swamp Water: 3 -> 4
        - Reduced Chaos Hound line's movement cost on swamp from 3 to 2.
        - Reduced Chaos Razerman's axe attack strength from 25-2 (!) to 18-2.
        - Reduced Dark Knight's axe attack strength from 17-2 to 14-2.
        - Reduced Dark Knight's cost from 36g to 32g.
        - Reduced Doom Guard's cost from 40g to 35g.
        - Reduced Elvish Hunter's HP from 30 to 29.
        - Reduced Elvish Protector's pierce resistance from 60% to 30%.
        - Reduced Elvish Prowler's HP from 66 to 62.
        - Reduced Elvish Trapper's HP from 44 to 43.
        - Reduced Elvish Warrior Spirit's HP from 18 to 16.
        - Reduced Hell Overlord's axe attack strength from 31-2 (!) to 20-2.
        - Increased Lady of Light's XP from 65 to 90.
        - Reduced Sylvan Faerie's HP from 68 to 61.
        - Increased Sylvan Faerie's melee attack strength from 8-3 to 6-5.
        - Reduced Sylvan Faerie's ensnare attack strength from 7-4 to 6-3.
        - Reduced Sylvan Faerie's thorns attack strength from 9-3 to 7-3.
        - Reduced Sylvan Faerie's mystic fire attack strength from 8-6 to 5-5.
        - Removed 'magical' weapon special from Elynia's staff.
    - Fixed a bug which caused Anlindë to lose her portrait after advancing to
      level 4.
    - Fixed cockatrice and chimera not being immune to plaguing
    - Fixed references to inexistent images (actually typos) in Dwarvish
      Runesmith's attack animation.
    - Fixed WEAPON_SPECIAL_DRAINS -> WEAPON_SPECIAL_DRAIN typo on Giant Leech.
    - Removed an extra, obsolete defense animation from Elvish Hunter.
    - Removed inclusion of inexistent macro BIRD_NAMES.
    - Removed some engine bug workarounds that we don't need on 1.5.x.
    - Removed units: Wose Shaman, Dread Bat [mainlined]
    - Simplified rules for vegetated terrain recognition on unit specials
    - Simplified Shaxthal's unit_type variation WML


; kate: indent-mode normal; encoding utf-8; space-indent on; word-wrap on;
; kate: indent-width 2;