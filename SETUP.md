# Setup

## Prerequisites
- Git
- Unreal Engine 5 (choose one version and keep the team aligned)
- Visual Studio with the C++ game development workload on Windows
- Enough disk space for the engine, derived data cache, and source assets

## Create the Unreal project
1. Create a **Games → Third Person → C++** project named `MultiverseMod`.
2. Put the `.uproject` at the repository root.
3. Generate IDE project files and compile the Development Editor target.
4. Enable Enhanced Input. Add other plugins only when required.
5. Commit source files and configuration; normally exclude `Binaries/`, `Intermediate/`, `Saved/`, and `DerivedDataCache/`.

## Validate a mod package
1. Keep the mod inside `Mods/<ModName>/`.
2. Add a `mod.json` manifest and data files.
3. Validate JSON syntax and schema before loading.
4. Reject unknown schema versions, unsafe paths, oversized files, and unsupported asset types.
5. Test the package in a disposable development build.

## Platform plan
Develop and profile on Windows PC first. Android requires mobile-friendly rendering, memory budgets, and touch controls. Console releases require platform-holder approval and platform-specific packaging; unrestricted file-based mod loading may not be permitted.
