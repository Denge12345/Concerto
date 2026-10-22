# Concerto 26.3 — Unofficial Fork Notes

This repository is an unofficial fork of
[GregTaoo/Concerto](https://github.com/GregTaoo/Concerto), maintained by
Denge12345. It is not affiliated with, endorsed by, or sponsored by the
upstream author.

## Provenance

- Upstream: `GregTaoo/Concerto`, branch `dev`
- Minecraft 26.3 port: [PR #122](https://github.com/GregTaoo/Concerto/pull/122)
  (`SWUST-Minecraft-Club/Concerto`, branch `mc26.3`, commit `353bad7`),
  authored by Nainingsama and contributors
- This fork keeps that commit history. The only source change made here is
  the Fabric Loader version described below.

## Changes in this fork

- `gradle.properties`: `fabric_loader_version` changed from `0.20.0` to
  `0.19.5`. The built jar therefore declares `fabricloader >=0.19.5` and can
  run on the 0.19.5 client/server this build targets. Fabric API
  `0.163.0+26.3` only requires loader `>=0.19.3`.
- Added this note.

No game code, assets, or license texts were changed.

## Build

Requires JDK 25 (the Gradle toolchain can provision it) and network access.

```bash
./gradlew buildAll
```

Outputs:

- `build/libs/Concerto-mc26.3-fabric-2.1.0.jar`
- `build/libs/Concerto-mc26.3-paper-2.1.0.jar`

## License

Concerto is distributed under the GNU General Public License v3.0; see
[`LICENSE`](LICENSE). Upstream copyright notices and all commit authorship
are preserved.

The upstream `LICENSE` also contains a preface about official distribution
channels. This fork is a free, non-commercial source build and does not
claim to be an official release. Official downloads remain the Modrinth,
CurseForge, and MCMod pages linked by upstream.

## Disclaimer

This is an unofficial build provided as-is, without warranty. The upstream
author is not responsible for this fork or for binaries published here.
