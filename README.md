# UEFortniteLocker

### Basic recreation of the Fortnite locker that uses CID's and Character Parts to display an Outfit and its info in a scene similar to the Fortmite in gmae locker.
### Made in Unreal Engine 5
### Go to Content/Locker/Locker.umap to see everything in action

# Explanation of What Everything Is

## Data Assets

*Note: Some Data Assets include extra variables that go unused, if a variable is not mentioned here assume you can leave it blank*

AthenaCharacterItemDefinition (CID_000) - Stores Character Parts, Name, Description, ShortDescription (Cosmetic type), Rarity, GameplayTags, and FortHeroType

FortHeroType (HID_000) - Stores Anim Override (changes pose used in the lcoker) and Item Images (only large is used)

CustomCharacterPart (CP_000) - Stores Gender (used for idle animation if not set to a custom one) Character Part Type, Master Skel Mesh (used only by the body), and Skel Mesh

## Data Tables

AthenaOutfitsData - Adding a CID here will add it to the Locker. Row name does not matter.

RarityData - Stores colors for each rarity.

CosmeticSetData - Stores Gameplay Tags and Name of each set. Row name must match the Gameplay Tag.

SeasonTagData - Stores Gameplay Tags and Name of each season. Row name must match the Gameplay Tag.

UserFacingFlags - Stores Gameplay Tags and Name of each UserFacingTag (Ex. Unlockable Styles). Row name must match the Gameplay Tag.

## Blueprints

LockerActor - Contains a camera, slot for each Skeletal Mesh provided by Character Parts, and blueprints that change the Outfit in the viewport using Character Parts.

## Widgets

TestHUD - Contains the Locker pannel and Selected Item Info. (Ignore the fact it has Test in the name, I never changed it.)

Locker Item Card - Old version of the Locker item Card i used when first making this (forgot to remove)

Locker Item Card New - The actual Item Card used by the Locker widget
