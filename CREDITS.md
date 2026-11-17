# Credits

## Based on / Inspiration

> Based on the gameplay concept of **Signit – A mod to sign anything!** by **gearsgodmaster**.
> Independently reimplemented for Minecraft 26.3 Fabric and NeoForge.
> Not affiliated with or endorsed by the original creator.

| | |
|---|---|
| Original project | Signit – A mod to sign anything! (Modrinth title: "Signit- A mod to sign anything!") |
| Original author | **gearsgodmaster** (owner of the Modrinth project; source repository under the GitHub organisation House-Kitty-Mew) |
| Original project page | https://modrinth.com/mod/signit-a-mod-to-sign-anything%21 |
| Original platform | Minecraft Java Edition 1.21.1, Fabric, server-side |
| Original license | All Rights Reserved (as stated on Modrinth) |
| Verified | 2026-11-17 via the Modrinth project page and the public Modrinth API (project `wK0QFOOR`, team member with role "Owner") |

### What inspired SignIt Modern

The original project publicly describes this gameplay, which SignIt Modern follows:

- hold the item to sign in the main hand and an emerald in the off hand, then right-click;
- the item receives the signer's name and a date-time stamp in its lore;
- a rarity rating is generated for the signed item;
- signatures are logged on the server (the original mentions an SQLite database);
- signed items work as collectibles; the original states that this is for fun, not for anything secure;
- server-side installation, no client mod needed.

### Independent reimplementation

SignIt Modern is a new, independent project. It was written from scratch against the Minecraft 26.3, Fabric and
NeoForge APIs, using only the publicly described features listed above:

- no source code, build files, textures, models, icons, texts or branding of the original were used or looked at;
- the original jars are not redistributed, patched or repackaged;
- all assets (seal texture, stamp model, icon, logo, banner) were created for this project in Blockbench
  (`art/blockbench/`) and with `tools/brand.py`;
- rarity tiers and probabilities are this project's own design (the original page documents no tiers or
  probabilities).

SignIt Modern is **not** an official port, continuation or successor of the original mod, and there is no
connection to, cooperation with or endorsement by gearsgodmaster. If you like the idea, please also visit and
support the original project.

## Libraries

| Library | Use | License |
|---|---|---|
| [SQLite JDBC](https://github.com/xerial/sqlite-jdbc) (org.xerial:sqlite-jdbc 3.54.1.0) | server-side signature ledger; bundled unmodified as jar-in-jar | Apache License 2.0 (SQLite itself: public domain) |
| Fabric Loader, Fabric API / NeoForge | mod loaders (not bundled) | Apache 2.0 / LGPL 2.1 |

## Author

SignIt Modern: cptgummiball.
