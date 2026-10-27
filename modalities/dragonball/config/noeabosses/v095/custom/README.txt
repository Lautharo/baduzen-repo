Dragon Block Noea v0.95 custom definitions

Put one schemaVersion 1 JSON object in forms/ or planets/. Disabled definitions
may set "enabled": false. Run /noea v095 validate after editing and read
config/noeabosses/v095/reports/custom-definitions-latest.json.

Form example:
{"schemaVersion":1,"id":"solar_ascendant","displayName":"Solar Ascendant",
 "races":["saiyan","sphinxian"],"unlockOnSkillLevel":1,
 "prerequisite":"","strengthMultiplier":2.0,"defenseMultiplier":1.75,
 "powerMultiplier":2.0,"speedMultiplier":1.1,"auraColor":"#75E6FF"}

Planet example (coordinates must remain outside the canonical system reserve):
{"schemaVersion":1,"id":"kai_world","displayName":"Kai World",
 "x":12000,"y":150,"z":12000,"tier":8,"palette":2,
 "bodyKind":"terrestrial","requiredPowerMultiplier":1.25}

Supported races: saiyan, human, namekian, frostdemon, majin, bioandroid,
demon, sphinxian. Supported body kinds: moon, terrestrial, ringed,
gas_giant, star. IDs must stay stable after players begin using a definition.
Noea only writes/removes dragonminez race files carrying its exact managedBy marker.
