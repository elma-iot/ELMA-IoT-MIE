# Versioned local releases

Final release folders are deliberately flat:

```text
release-assets/
  1.19.16/
    MIE Portable 1.19.16.exe
    ELMA-IoT-MIE_1.19.16.0_x64.msix
    Release notes 1.19.16.txt
    ELMA-IoT-MIE.mielicense       (only when compatible)
```

Owner tools are maintained only in the project-root `Owner Tools/` folder. The current Keygen is `Owner Tools/ELMA-IoT MIE Keygen.exe`; previous owner utilities are preserved under `Owner Tools/Archive/`.

No compiler output, owner tools, test artifacts, work backups or content caches are staged inside a release. The application generates its normal working folders beside the local EXE when run. Existing work files and prior full snapshots remain in `build/`, `.audit/` and the layout migration backup recorded under `.audit/ReleaseLayoutBackup/`. Optional offline packs remain available in the matching `.audit/Release-<version>/Content/` folder for Browse pack installation if their download is not yet published.

A final folder is created only when the matching portable executable and MSIX are available. The package manifest version is checked. Incomplete/historical builds without a matching MSIX stay in the work archive. Stage a completed pair with:

```powershell
python tools/Stage-PortableRelease.py --version 1.19.16 --source .audit/Release-1.19.16 --inherit-state
```

The retained `--inherit-state` option carries only a compatible license. The target application verifies its signature, Windows installation and supported license protocol; expired or not-yet-active licenses are excluded. A role license additionally needs its existing matching, accessible account authorization key; when compatible, that required `authorization-key.dat` companion is copied too. The application still performs its normal trusted-time verification at startup. No owner signing key or cached activation state is included in the release.

Each version has exactly one folder named `<version>`. Rebuilding that version updates its EXE, MSIX and notes in place; identical files are left untouched. Existing runtime folders, settings, work files and local licenses are preserved. A compatible license and authorization key can be carried forward from the current or previous release. Older, different version folders remain unchanged. Release files are prepared before replacement, and a failed replacement rolls back files already changed. Close the testing application before replacing its EXE. `release-assets/latest.json` identifies the current release. Before recompiling, generated work is preserved separately under `.audit/ReleaseWorkHistory/`.

The release folder can contain a personal license and stays excluded from Git. Distributable packages in `dist/` are still built from explicit application files and never include local licenses or owner keys. Copying a license does not remove its Windows/account binding.
