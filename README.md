# Spectre Rodeo
Northstar mod that ports Spectre rodeo behavior from Titanfall 1 Frontier Defense gamemode with some additions for usage in other gamemodes.
__Required to be installed on both server and client.__

__Compability issues:__ This mod replaces spectre model (robots/spectre/imc_spectre.mdl) with one that has more animations included. 
If you use other mod that replaces it, you'll get script error about missing animations. You can either change load order of this mod, or modify mdl by adding 2 `$includemodel` lines in QC and re-compile it. 
```
$includemodel "humans/pete/pete_scripted_r1.mdl"
$includemodel "humans/pete/pilot_shared.mdl"
```

When Titan faces Spectre in close range, it will jump on titan and steal battery or throw grenade into hatch if it has one.
Spectres with battery will try to bring it to friendly random Titan. Hacked Spectres prioritize Titan of player who hacked them.

### Server ConVars
```
sv_spectre_rodeo_reset (Default value: 1) - Allow Spectres to try rodeoing Titans again after successful attempt.
sv_spectre_rodeo_reset_time (Default value: 10) - Time in seconds before Spectre starts trying to rodeo Titans again after successful attempt.
sv_spectre_rodeo_allow_friendly (Default value: 1) - Allow Spectres with battery to rodeo friendly Titans.
sv_spectre_rodeo_nuke_grenade (Default value: 0) - Spectres will use Core Overload grenades when rodeoing (Nuke Rodeo from Frontier Defense).
sv_spectre_rodeo_classic (Default value: 0) - Force Spectres to use classic rodeo, unless they're using Core Overload grenades.
```

### To-Do List
- Non-frontal rodeo.
- Animation fixes and code refactoring.