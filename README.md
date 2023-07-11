# Gambeson
`fabric-api`, patched to run on Forge using Steelwool

## Setup
1. `mkdir gambeson` if it doesn't exist
2. `./gradlew updateSubmodules`
3. `./gradlew applyPatches`

After modifying the commits in `gambeson`, run `./gradlew makePatches` to regenerate the patches.

## Updating

(TODO is this information correct?)

1. Rebase onto a new parent commit in `gambeson`
2. Checkout the same parent commit in `fabric`
3. Commit the change to `fabric` (or staging it might be sufficient? unknown)
4. Run `./gradlew makePatches`; patches will be generated based on the new parent commit.
