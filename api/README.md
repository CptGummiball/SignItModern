# SignIt Modern for mod developers

API version **1** · package `dev.cptgummiball.signitmodern.api` · mod id `signit_modern`

SignIt Modern 1.0 has **no Java API surface** besides the version constant (`SignItModernApi.API_VERSION`). You do
not need a dependency to work with signed items: signatures are stored in **vanilla item components**, so any mod
can read them from an `ItemStack` without compiling against SignIt Modern.

## Reading a signature

`minecraft:custom_data` of the stack contains:

```
signit_modern: {
  signature: {
    v: "1",                        schema version
    id: "<uuid>",                  unique signature id
    signer: "<uuid>",              signer UUID
    name: "Alex",                  signer name at signing time
    at: "1794924180000",           UTC epoch milliseconds
    rarity: "rare",                common | uncommon | rare | epic | legendary
    server: "...", world: "..."    optional
  }
}
```

All values are strings. Treat unknown keys as forward-compatible additions and newer `v` values as readable as long
as the version-1 keys exist. The lore lines are display only (translatable components `signit_modern.lore.*`).

Please do **not** write or change these keys from another mod: signatures are created only by the server running
SignIt Modern. A signature is a collector feature, not a proof of authenticity.

## Getting the API jar

`signit_modern-api-1.jar` and the javadoc jar are attached to the GitHub releases; they only contain the version
constant. The license (section 5) allows compiling against the API and publishing mods that use it.
