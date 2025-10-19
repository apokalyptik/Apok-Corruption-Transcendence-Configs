Generating the base configs
---------------------------
* Base config template: Cloned from GameServerApp.com's "Default settings" template for ASA
* DynamicConfig - empty
* chain - empty
* end - -mods=945677,949623,945883,940975,953154,941697,942024,959740 -DoCustomCosmeticValidation

Sources for configuration and mod values
----------------------------------------
* Mod list and tweaks came from: https://discord.com/channels/694491278729019423/1325487529746632838/1325490513436217405
* Config settings came from: https://discord.com/channels/694491278729019423/1325487529746632838/1361689572538322994
* NPC Overrides came from: https://discord.com/channels/694491278729019423/1178270462900441118/1220447625661124699

Changes to GameUserSettings.ini
-------------------------------
    ; Balanced around 150
    DifficultyOffset=1.000000

    ; not running a Pvp Server
    ServerPVE=True

    ; hopefully prevent losing dino balls randomly sometimes?
    [DinoDepot]
    DinoballAutoStackMode=3

Changes to Game.ini
-------------------
    ; remove these two engrams per https://discord.com/channels/694491278729019423/1325487529746632838/1325490513436217405
    OverrideNamedEngramEntries=(EngramClassName="EngramEntry_Propagator_CS_C",EngramHidden=true)
    OverrideNamedEngramEntries=(EngramClassName="EngramEntry_Mutator_CS_C",EngramHidden=true)

    ; NPC Overrides Copy and Pasted from https://discord.com/channels/694491278729019423/1178270462900441118/1220447625661124699
