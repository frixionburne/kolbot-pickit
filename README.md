# kolbot-pickit
Diablo II Kolbot pickits

# Usage Example
In your config file (ex. Paladin.MCHammerdin.js)

```
// Pickit config. Default folder is kolbot/pickit.
Config.PickitFiles.push("frixionburne/frix_temp.nip");
//Config.PickitFiles.push("frixionburne/frix_early_ladder.nip");
//Config.PickitFiles.push("frixionburne/frix_mid_ladder.nip");
Config.PickitFiles.push("frixionburne/frix_bases.nip");
Config.PickitFiles.push("frixionburne/frix_godly.nip");
Config.PickitFiles.push("frixionburne/frix_sets.nip");

// Config.PickitFiles.push("kolton.nip");
Config.PickitFiles.push("LLD.nip");
Config.PickRange = 40; // Pick radius
Config.FastPick = false; // Check and pick items between attacks
```

# Useful Character Config Crafting Lines
## Insight
```
Config.Runewords.push([Runeword.Insight, "Thresher", Roll.Eth]); // Make ethereal Insight Thresher
Config.Runewords.push([Runeword.Insight, "Cryptic Axe", Roll.Eth]); // Make ethereal Insight Cryptic Axe
Config.Runewords.push([Runeword.Insight, "Colossus Voulge", Roll.Eth]); // Make ethereal Insight Colossus Voulge
Config.Runewords.push([Runeword.Insight, "Great Poleaxe", Roll.Eth]); // Make ethereal Insight Great Poleaxe
Config.Runewords.push([Runeword.Insight, "Giant Thresher", Roll.Eth]); // Make ethereal Insight Giant Thresher

Config.KeepRunewords.push("[type] == polearm # [meditationaura] >= 17");
Config.KeepRunewords.push("[type] == polearm # [meditationaura] >= 17 && [enhanceddamage] >= 260 && [attackrate] >= 250 && [plusskillcriticalstrike] >= 6");
```
## Spirit
```
Config.Runewords.push([Runeword.Spirit, "Monarch", Roll.NonEth]); // Make Spirit Monarch
Config.Runewords.push([Runeword.Spirit, "Sacred Targe", Roll.NonEth]); // Make Spirit Sacred Targe
Config.Runewords.push([Runeword.Spirit, "Sacred Rondache", Roll.NonEth]); // Make Spirit Sacred Rondache
Config.Runewords.push([Runeword.Spirit, "Royal Shield", Roll.NonEth]); // Make Spirit Royal Shield
Config.Runewords.push([Runeword.Spirit, "Crown Shield", Roll.NonEth]); // Make Spirit Crown Shield
Config.Runewords.push([Runeword.Spirit, "Crystal Sword", Roll.NonEth]); // Make Spirit Crystal Sword
Config.Runewords.push([Runeword.Spirit, "Long Sword", Roll.NonEth]); // Make Spirit Long Sword
Config.Runewords.push([Runeword.Spirit, "Broad Sword", Roll.NonEth]); // Make Spirit Broad Sword

Config.KeepRunewords.push("([type] == sword || [type] == shield || [type] == auricshields) # [fcr] == 35");
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