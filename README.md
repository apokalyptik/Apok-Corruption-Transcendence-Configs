Generating the base configs
---------------------------
* Base config template: Cloned from GameServerApp.com's "Default settings" template for ASA
* DynamicConfig - empty
* chain - empty
* end - `-mods=945677,949623,945883,940975,953154,941697,942024,959740 -DoCustomCosmeticValidation`
  * 945677 [Ark: Corruption Transcendence](https://www.curseforge.com/ark-survival-ascended/mods/act)
  * 949623 [Nanoh's Spyglass](https://www.curseforge.com/ark-survival-ascended/mods/nanohs-spyglass)
  * 945883 [Omega Teleporters](https://www.curseforge.com/ark-survival-ascended/mods/omega-teleporters)
  * 940975 [Cybers Structures QoL+ (Crossplay)](https://www.curseforge.com/ark-survival-ascended/mods/cybers-structures)
  * 953154 [Auto Engrams!](https://www.curseforge.com/ark-survival-ascended/mods/auto-engrams)
  * 941697 [Better Breeding](https://www.curseforge.com/ark-survival-ascended/mods/better-breeding)
  * 942024 [Dino Depot](https://www.curseforge.com/ark-survival-ascended/mods/dino-depot)
  * 959740 [GameServerApp.com Integration (Crossplay)](https://www.curseforge.com/ark-survival-ascended/mods/gsa-integration-no-shop)

Sources for configuration and mod values
----------------------------------------
* [Mod list and tweaks post](https://discord.com/channels/694491278729019423/1325487529746632838/1325490513436217405)
* [Config settings post](https://discord.com/channels/694491278729019423/1325487529746632838/1361689572538322994)
* [NPC Overrides post](https://discord.com/channels/694491278729019423/1178270462900441118/1220447625661124699)

Changes to GameUserSettings.ini
-------------------------------
* Balanced around level 150 dinos:
```
DifficultyOffset=1.000000
```
* I don't want no PVP Server:
```
ServerPVE=True
```
* Hopefully a workaround for a bug causing odccasional dino losses
```
  [DinoDepot]
  DinoballAutoStackMode=3
```
* MOTD
```
[MessageOfTheDay]
Message=Welcome to Ark: Corruption Transcendence
```

Changes to Game.ini
-------------------
* add all the NPC Overrides copy and pasted from the linked file in the [NPC Overrides post](https://discord.com/channels/694491278729019423/1178270462900441118/1220447625661124699)
* Remove two engrams per the [Mod list and tweaks post](https://discord.com/channels/694491278729019423/1325487529746632838/1325490513436217405)
```
    ; remove these two engrams per https://discord.com/channels/694491278729019423/1325487529746632838/1325490513436217405
    OverrideNamedEngramEntries=(EngramClassName="EngramEntry_Propagator_CS_C",EngramHidden=true)
    OverrideNamedEngramEntries=(EngramClassName="EngramEntry_Mutator_CS_C",EngramHidden=true)
```
