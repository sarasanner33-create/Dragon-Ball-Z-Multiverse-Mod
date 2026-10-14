# Full project structure

```text
Dragon-Ball-Z-Multiverse-Mod/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   └── workflows/
│       └── validate-mod-data.yml
├── Config/
│   └── ModSchema/
│       ├── character.schema.json
│       ├── ability.schema.json
│       └── world.schema.json
├── Content/
│   ├── Characters/
│   ├── Worlds/
│   ├── Arenas/
│   ├── Abilities/
│   ├── VFX/
│   ├── Audio/
│   ├── UI/
│   └── Data/
├── Docs/
│   ├── ARCHITECTURE.md
│   ├── MODDING_GUIDE.md
│   ├── ROADMAP.md
│   └── SECURITY.md
├── Mods/
│   └── ExampleOriginalWarrior/
│       ├── mod.json
│       ├── characters/
│       │   └── original_warrior.json
│       ├── abilities/
│       │   └── energy_burst.json
│       └── worlds/
│           └── crystal_frontier.json
├── Plugins/
│   └── MultiverseModKit/
│       ├── MultiverseModKit.uplugin
│       ├── Source/
│       │   ├── MultiverseModKit/
│       │   └── MultiverseModKitEditor/
│       └── Resources/
├── Source/
│   └── MultiverseMod/
│       ├── MultiverseMod.Build.cs
│       ├── Public/
│       │   ├── Characters/
│       │   ├── Combat/
│       │   ├── Abilities/
│       │   ├── Worlds/
│       │   ├── Mods/
│       │   ├── Progression/
│       │   ├── Save/
│       │   └── UI/
│       └── Private/
│           ├── Characters/
│           ├── Combat/
│           ├── Abilities/
│           ├── Worlds/
│           ├── Mods/
│           ├── Progression/
│           ├── Save/
│           └── UI/
├── Tests/
│   ├── Unit/
│   ├── Integration/
│   └── TestMods/
├── Tools/
│   ├── mod_validator/
│   └── asset_manifest/
├── .editorconfig
├── .gitattributes
├── .gitignore
├── LICENSE
└── README.md
```

## Responsibilities
- `Source/`: trusted gameplay code and runtime systems.
- `Plugins/MultiverseModKit/`: optional mod browser, validator, and authoring tools.
- `Mods/`: user-created packages; never assume their files are safe.
- `Config/ModSchema/`: JSON schemas for validating mod data.
- `Content/`: original project assets and data assets.
- `Tests/`: unit, integration, and compatibility tests.
- `Tools/`: command-line validation and build helpers.
- `.github/workflows/`: automated checks on pull requests.
