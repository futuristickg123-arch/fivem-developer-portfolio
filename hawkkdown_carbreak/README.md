# Hawkk Car Break

A dynamic vehicle break-in script that utilizes QTE minigames, particle effects, and car alarm triggers to simulate street thefts.

## Dependencies
- `es_extended`
- `ox_lib`
- `ox_target`
- `ox_inventory`

## Features
- Integrates ox_target vehicle window breaking options
- Requires lockpick items to begin minigames
- Triggers a top-down focus camera of the vehicle window during breaking sequences
- Spawns realistic glass smashing sound effects and window smoke particles
- Chance of setting off the car alarm and alerting police dispatch

## Required Items
- `lockpick`

## Commands
- **/testcarbreak**: Forcibly triggers window break sequence on nearest vehicle (Debug)

## Configuration Sample
```lua
Config.Minigame = {
    Difficulty = 'medium',
    TimeLimit = 10,
    Keys = {'w', 'a', 's', 'd'}
}
```

## Installation
1. Ensure all dependencies listed above are started in your `server.cfg`.
2. Copy this folder into your resources directory under `[Hawkk]`.
3. Add `ensure hawkkdown_carbreak` to your `server.cfg`.
