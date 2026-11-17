# Changelog

## 1.0.0 – 2026-11-17

First release of SignIt Modern for Minecraft 26.3 (Fabric and NeoForge).

Based on the gameplay concept of *Signit – A mod to sign anything!* by gearsgodmaster. Independently reimplemented
for Minecraft 26.3 Fabric and NeoForge. Not affiliated with or endorsed by the original creator.

- Sign any item: item in the main hand, emerald in the off hand, right-click (air, block or entity).
- Signature with signer UUID and name, UTC timestamp, unique signature id, rarity and schema version, stored in
  vanilla item data; lore lines appended, everything else on the item kept.
- Five cosmetic rarity tiers (Common 60 %, Uncommon 25 %, Rare 10 %, Epic 4 %, Legendary 1 %), configurable.
- Exactly one item per signature: stacks are split safely, full inventories abort without changes.
- Already signed items are refused without cost; duplicate packets of one click sign once.
- Server-side ledger in SQLite (bundled driver, per world, background thread), JSONL fallback.
- Commands `/signit info | history | reload | config`.
- Configuration file with validation; English and German texts; works with clients without the mod
  (English fallback texts).
