# Modding guide (starter)

A mod is a directory with a manifest and supported data files. This initial scaffold describes the intended format; a runtime loader still needs to be implemented.

Example:
```json
{
  "schemaVersion": 1,
  "id": "example.original_warrior",
  "name": "Original Warrior Example",
  "version": "0.1.0",
  "author": "Your Name",
  "description": "A sample original character package.",
  "content": {
    "characters": ["characters/original_warrior.json"],
    "abilities": ["abilities/energy_burst.json"],
    "worlds": ["worlds/crystal_frontier.json"]
  }
}
```

Only use supported fields. Keep asset paths relative to the mod folder. Do not include copyrighted material unless you have permission.
