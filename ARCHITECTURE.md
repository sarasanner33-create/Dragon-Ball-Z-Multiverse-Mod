# Architecture

## Runtime layers
1. Input and camera
2. Character movement and targeting
3. Combat state machine (neutral, attacking, guarding, dodging, stunned, defeated)
4. Ability execution and cooldown/resource costs
5. Character progression and transformation states
6. World/arena streaming and environment settings
7. Save/profile layer
8. Mod manifest discovery, validation, and content registration

## Mod safety rules
- Mods are data-first; never execute arbitrary scripts from a downloaded package.
- Validate every manifest against a versioned schema.
- Normalize paths and prevent traversal outside the mod root.
- Set file-size and count limits; handle malformed JSON gracefully.
- Use an explicit allowlist of asset types and gameplay properties.
- Do not allow mods to overwrite core files or load native binaries.
- Keep online competitive play server-authoritative and define a separate approved mod policy.

## Suggested implementation order
Movement → camera → target lock → light/heavy attacks → health/stamina → one ability → one test arena → save/load → mod manifest loader → character customization → more worlds and quests.
