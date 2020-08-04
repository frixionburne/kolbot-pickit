# kolbot-pickit
Diablo II Kolbot pickits

# Usage Example
In your config file (ex. Paladin.MCHammerdin.js), be sure to add the new pickit configs and comment out the kolton.nip include

```
// Pickit config. Default folder is kolbot/pickit.
//Config.PickitFiles.push("frixionburne/frix_early_ladder.nip");
//Config.PickitFiles.push("frixionburne/frix_mid_ladder.nip");
Config.PickitFiles.push("frixionburne/frix_bases.nip");
Config.PickitFiles.push("frixionburne/frix_godly.nip");

// Config.PickitFiles.push("kolton.nip");
Config.PickitFiles.push("LLD.nip");
```

Additionally, a good idea for your own changes is to create a copy of the frix_temp.nip file and make customizations there.
For example, for a customized copy of frix_temp.nip named `frix_temp_custom.nip`

```
// Pickit config. Default folder is kolbot/pickit.
Config.PickitFiles.push("frixionburne/frix_temp_custom.nip");
//Config.PickitFiles.push("frixionburne/frix_early_ladder.nip");
//Config.PickitFiles.push("frixionburne/frix_mid_ladder.nip");
Config.PickitFiles.push("frixionburne/frix_bases.nip");
Config.PickitFiles.push("frixionburne/frix_godly.nip");

// Config.PickitFiles.push("kolton.nip");
Config.PickitFiles.push("LLD.nip");
```

# Useful Character Config Gambling Lines
## Claws
```
Config.GambleItems.push("Katar");
Config.GambleItems.push("Wrist Blade");
Config.GambleItems.push("Claws");
Config.GambleItems.push("Blade Talons");
```

# Useful Character Config Crafting Lines
## Socketing
```
// Polearms
Config.Recipes.push([Recipe.Socket.Weapon, "Colossus Voulge", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Weapon, "Thresher", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Weapon, "Cryptic Axe", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Weapon, "Great Poleaxe", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Weapon, "Giant Thresher", Roll.Eth]);

// Eth bugged armors
Config.Recipes.push([Recipe.Socket.Armor, "Dusk Shroud", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Wyrmhide", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Scarab Husk", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Wire Fleece", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Diamond Mail", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Loricated Mail", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Great Hauberk", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Boneweave", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Balrog Skin", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Archon Plate", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Kraken Shell", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Hellforge Plate", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Lacquered Plate", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Shadow Plate", Roll.Eth]);
Config.Recipes.push([Recipe.Socket.Armor, "Sacred Armor", Roll.Eth]);
```

## Insight
```
Config.Runewords.push([Runeword.Insight, "Colossus Voulge", Roll.Eth]);
Config.Runewords.push([Runeword.Insight, "Thresher", Roll.Eth]);
Config.Runewords.push([Runeword.Insight, "Cryptic Axe", Roll.Eth]);
Config.Runewords.push([Runeword.Insight, "Great Poleaxe", Roll.Eth]);
Config.Runewords.push([Runeword.Insight, "Giant Thresher", Roll.Eth]);

Config.KeepRunewords.push("[type] == polearm # [meditationaura] >= 17");
Config.KeepRunewords.push("[type] == polearm # [meditationaura] >= 17 && [enhanceddamage] >= 260 && [attackrate] >= 250 && [plusskillcriticalstrike] >= 6");
```
## Spirit
```
Config.Runewords.push([Runeword.Spirit, "Monarch", Roll.NonEth])

Config.Runewords.push([Runeword.Spirit, "Crystal Sword", Roll.NonEth])
Config.Runewords.push([Runeword.Spirit, "Long Sword", Roll.NonEth])
Config.Runewords.push([Runeword.Spirit, "Broad Sword", Roll.NonEth])

Config.Runewords.push([Runeword.Spirit, "Targe", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Rondache", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Heraldic Shield", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Aerin Shield", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Crown Shield", Roll.NonEth]);

Config.Runewords.push([Runeword.Spirit, "Akaran Targe", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Akaran Rondache", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Protector Shield", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Gilded Shield", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Royal Shield", Roll.NonEth]);

Config.Runewords.push([Runeword.Spirit, "Sacred Targe", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Sacred Rondache", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Kurast Shield", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Zakarum Shield", Roll.NonEth]);
Config.Runewords.push([Runeword.Spirit, "Vortex Shield", Roll.NonEth]);

Config.KeepRunewords.push("([type] == sword || [type] == shield || [type] == auricshields) # [fcr] == 35");
Config.KeepRunewords.push("([type] == sword || [type] == shield || [type] == auricshields) # [fcr] == 35 && [maxmana] >= 112");
Config.KeepRunewords.push("([type] == sword || [type] == shield || [type] == auricshields) # [fcr] == 35 && [maxmana] >= 112 && [itemabsorbmagic] >= 8");
```
## Heart Of The Oak
```
Config.Runewords.push([Runeword.HeartoftheOak, "Flail", Roll.NonEth]); // Make HotO Flail
Config.KeepRunewords.push("[type] == mace # [fireresist] == 40");
```
## Call To Arms
```
Config.Runewords.push([Runeword.CallToArms, "Flail", Roll.NonEth]); // Make CTA Flail
Config.Runewords.push([Runeword.CallToArms, "Crystal Sword", Roll.NonEth]); // Make CTA Crystal Sword
Config.KeepRunewords.push("([name] == crystalsword || [name] == flail) # [plusskillbattlecommand] >= 6 && [plusskillbattleorders] >=6 && [plusskillbattlecry] >= 4");
```

## Prudence
```
Config.Runewords.push([Runeword.Prudence, "Balrog Skin", Roll.Eth]);
Config.KeepRunewords.push("([type] == armor) # [enhanceddefense] == 170 && [fireresist] >= 30");
```