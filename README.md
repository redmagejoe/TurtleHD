# TurtleHD
Turtle WoW HD patch MPQ repo

I (Astricon) am also active on the Turtle WoW Discord Channel in my own subchannel #hd-patch. However, I will refer you to this GitHub for known issues and FAQs sometimes, or someone else will.

## Contents

This mod updates many things at once in your client to appear more modern. This is the most frequently-updated part of the HD Mod (patch-A). 
patch-A includes the following:
- Player Character Models and Textures
- NPC humanoid and non-humanoid models and textures
- Spell sounds and visuals
- Equipment models and textures
- Music

patch-B: https://drive.google.com/file/d/1GQ932XSzsFMKozhGd-a8HPetQI79xcXb/view?usp=share_link
- World and environment visual upgrade

patch-C: https://drive.google.com/file/d/1LAldcTI2CFliAvMTYVbURDngHyqVTzCH/view
- Autoattack weapon sound update

## Installation

As with any MPQ-based Classic WoW mod, simply get the MPQ by downloading it from the "Releases" link on the main github page, then put the MPQ file in your TWoW/data folder with all the other MPQs. If you have other MPQs in this folder from other mods, their name will matter as MPQs load in order alphabetically. If you only use the HD mod, this will not affect you.

## Reporting a Bug or Submitting a Request
You can report bugs and submit requests through the Issues tab in Github. Please check the Frequently-Asked Questions and Known Issues section of this README as well as existing issues before posting a new issue. Also, make sure you have observed the issue exists with the HD Patch and NOT without it, and that you have freshly deleted your WDB folder and that the issue isn't due to interactions with other addons and mods you maay have.

## Frequently-Asked Questions
### Can you make a version of this without X change? I like Y but I don't like X.
No, but you can! Download Ladik's MPQ Editor (https://www.hiveworkshop.com/threads/ladiks-mpq-editor.249562/) and get to work. It's not that hard. Once you have it, all you need to do is go into patch-A with it and delete files you don't like. Finding which files are the correct ones to delete can be challenging, but it can also be pretty obvious. Here's some common use cases:
#### I want the player character models and textures but I don't want the new spell effects and sounds
Delete the following:
- In the folder DBFilesClient: Spell.dbc, SpellVisual.dbc, SpellVisualKit.dbc, SpellVisualEffectName.dbc, and SoundEntries.dbc
- The whole folder on the top level called "Spells"
- The whole Sounds/Spells folder (not the whole Sounds folder, just the Spells one inside it)
- This might mess up your dungeon entrance texture, but someone might figure out a solution to this soon
- You CANNOT have the spell sounds update without the spell visuals update or vice versa. They are unfortunately tied together, so don't ask for this.
  
#### I want a certain race to be modern, but not others
Sorry, this is way harder to do than you think. You'll have to edit DBCs for this one.
#### I don't want the equipment visual changes
- Delete the "Item" folder in patch-A
- In the DBFilesClient folder, delete ItemDisplayInfo.dbc
  
#### The music isn't right in some areas. I'd prefer the vanilla versions
- In the Sound folder, delete the Music folder

### Will this be updated in time for the next Turtle WoW patch?
Probably. I (Astricon) am on the TWoW team, so I have access to their client changes which I can work on before launch. The current patch is updated for the Gilneas patch.

### Can I Contribute?
I think so. Try making your own branch and see if it works. Otherwise, contact me on Discord. I use the same name there (Astricon)

## Known Issues
- Sheath animation is broken for most race/sex models. This is difficult to fix and may never be, so I suggest you unbind your sheath/unsheath keybind and live with it.
- Many TWoW custom mounts have messed up textures
- Infernal, Deer, Sea Giant, Hydra, and Pterodactyl models are giant. This is difficult to fix currently but I am always exploring what can be done about this.
- Wyverns are missing the death animation and Gryphons are missing the attack animation. Gryphons can be fixed soon, but Wyverns might have to be reverted to their old model.
- High Elf eye glow is weak, doesn't react to blinking very well, and remains blue for the premium Blood Elf and Dark Ranger skins. This may not be fixable, so I may just remove the glow altogether or there may be a workaround in the future.
- Rain of Fire is a very temperamental spell, and my efforts to change its fire to green like all other Warlock Fire Spells have failed thus far. You will notice a single green fireball falling every wave. Yeah.
- Moonfire's visual effect is very oversized. Not sure how to fix this yet but it's probably doable eventually.
- All ogres are currently 1-Headed. Not ideal. Trying to downport a two-headed model but no success yet.

## TO-DO List
Including the Known Issues, here are some updates you might see in the future
- New models for Boar, Quillboar, Gnoll, Kobold, Nightsaber, Unicorn, Level 40 Paladin Class Mount, Totem, Rams
- More spell effect and sounds updates, as usual.
