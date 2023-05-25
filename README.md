# Spectre Rodeo
Northstar mod that ports Spectre rodeo behavior from Titanfall 1 Frontier Defense gamemode with some additions for usage in other gamemodes.
__Required to be installed on both server and client.__

When Titan faces Spectre in close range, it will jump on titan and steal battery or throw grenade into hatch if it has one.
Spectres with battery will try to bring it to friendly random Titan. Hacked Spectres prioritize Titan of player who hacked them.

### Server ConVars
```
sv_spectre_rodeo_reset (Default value: 1) - Allow Spectres to try rodeoing Titans again after successful attempt.
sv_spectre_rodeo_reset_time (Default value: 10) - Time in seconds before Spectre start trying to rodeo Titans again after successful attempt.
sv_spectre_rodeo_allow_friendly (Default value: 1) - Allow Spectres with battery to rodeo friendly Titans.
sv_spectre_rodeo_nuke_grenade (Default value: 0) - Spectres will use Core Overload grenades when rodeoing (Nuke Rodeo from Frontier Defense).
```

### TODO List
- Classic rodeo support.
- Non-frontal rodeo.
- Animation fixes and code refactoring.