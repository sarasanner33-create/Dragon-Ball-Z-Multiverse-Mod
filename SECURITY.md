# Security and trust boundaries

Mod packages are untrusted. Do not run arbitrary code from mods. Validate schemas, limit file sizes, canonicalize paths, reject path traversal, constrain asset references, and provide a way to disable a failing mod. Keep multiplayer authoritative and do not let client mods grant competitive advantages. Scan dependencies and pin tool versions in CI.
