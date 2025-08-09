## Fell Seal Expansion PaC (Portraits and Classes)

### Preamble
What I enjoy most about Fell Seal is the creative ways in which the many different abilities of different classes can be combined in fun, powerful, and unexpected ways. Having played quite a bit and tried many of these combinations, I sought to add more options to the theory crafting pool of Fell Seal's numerous abilities without power-creeping existing classes into irrelevance. As such, nearly all active abilities are completely new abilities that I have made from the soup of accessible and alterable ability properties found in game; the goal being to create classes with new niches, playstyles, and combinations, without merely creating a selection of super classes. Additionally, nearly all passive and counter abilities are either newly created or abilities that were previously only accessible to monster/non-generic classes. I've also thrown in a few new weapons for a bit of fun, all of which are obtainable through new hunts or dispatch missions. 
In further seeking to expand replayability, I have also created a number of new character portraits for all manner of characters to increase the existing selection. Nearly all portraits were made based off of in-game aesthetic options so there won't be weird portrait and character mismatch. Additionally, I have tried to incorporate elements in the portraits of lesser-used items/equipment/aesthetics to make picking those options more viable when selecting a portrait. This is my first mod - I hope you enjoy!

### What the mod adds
* 12 new fully custom classes with diverse, and (hopefully) balanced abilities 
    * 8 generic classes, 1 badge class, 3 story classes (one for Kyrie, Anadine, & Reiner) 
    * Classes should be encounterable as enemies as you progress, diversifying random encounters
* 20 new equippable items to add some spice and alternate tactical options
    * 9 weapons, 7 weapons of a new type, 3 armors, 1 accessory
* 9 new dispath missions and 3 new hunts to acquire new items
    * Battle against new classes using new items to reap the rewards
* New portraits created based on the aesthetic options available in character creation in order to make visual matching a reality. 
    * 30 female portraits, 32 male portraits, 4 unisex portraits
    * More portraits of people with darker skin tones, class helmets, accessories, and gear color combinations
    * No longer choose between using the same old portraits or portraits that clash with your characters' sprites

### Installation
**This mod uses abilities from the DLC (Missions and Monsters) and it is required for the mod to work**
* If using a mod manager, simply download and install according to your mod manager's instructions.
* If installing manually, most files will be copied into your customdata folder found at "C:\Users\username\Documents\Fell Seal\customdata", that includes all files except for the portraits and "abilities.txt", "ingredients.txt", and "weapons.txt". The latter three go in "C:\Users\username\Documents\Fell Seal\customdata\languages\en". If you have never modded Fell Seal before, you may need to create the "languages" and "en" folders.
* Portrait installation is the same for any other custom portrait you would upload, inside of "C:\Users\username\Documents\Fell Seal\customdata\portraits" there are folders for "female", "male", and "unisex" in which you should place the relevant portraits. 

### Known Issues
The only **Real** issue is if you intend to mod my work - see #2 below.
<details>
    <summary>Click to Reveal Known Issues</summary>

    - Classes specific to story characters still appear in other characters' class wheels. They are still inaccessible to everyone else, so it's just a visual thing, but one for which I don't know a good fix. 
    - The Martial Artist class pushes the boundaries of what can be done with modded classes, using certain abilities in ways that they weren't designed to be used. This can affect you in two ways:
        1. For normal players: the class' abilities use Beastmaster abilities under the hood. If you combine those abilities in game, you may get some weirdness. As far as I am aware, this means:
            * Qi charges and pets can be used interchangeably. Serenity will also work with Qi charges. 
            * If you summon pets and use a Finisher, pets will visually remain behind despite being dismissed.
        2. For people who want to mess with this code themselves: There is something going on behind the scenes related to the weird way I am using these abilities which has a very strange effect. It makes it so that after the code for the Martial Artist is in your project, abilities created will not work properly (the visual component of the EffectHash will not trigger, and new abilities will default to the generic swing animation). Note that it has to do with when you create abilities, not where they are placed in relation to the Martial Artist code. So weird, and took quite a while to discover.
        Because the class otherwise functions as intended (and does some pretty cool stuff) I decided to keep it. However, given the constraint above, I obviously could not make any more custom classes after making the Martial Artist. As a result, I saved all of the related info for it elsewhere, and (because it all still works) I just added it back in after I was done making my other classes. However, it was a crazy headache to discover this glitch as I initially thought there were certain EffectHash animations which just didn't work properly when modded. So, if you intend to mod/mess with any class-related stuff from this mod, I recommend you remove the Martial Artist (commenting it out did not work for me, I had to remove it and then run the game once) before messing with the code. Make a simple ability with a visual effect you are familair with, and verify that it is working as intended. Hopefully this will spare a would-be tinkerer from suffering as I have. If anyone finds/knows more specifics on what is going on, please reach out. 
</details>

<h1 style="text-align: center;">SPOILERS BELOW</h1>

### Complete Class List
* **Monster Hunter** - Mobile hunters who use specialized grappling hooks to maneuver over difficult terrain as well as displace and dispatch prey. They also employ an array of traps meant for all manner of creatures. 
* **Dancer** - Dancers flow gracefully across the battlefield, evading harm, beguiling their enemies, and captivating all who come near. 
* **Martial Artist** - These skillfull warriors unleash devastating combos by using a series setup techniques to charge their qi before delivering a finishing strike. Qi charges cap at 3. Each setup move can only be used once before a finisher is used. 
* **Demonologist** - These fanatics' lust for power is unbridled - willingly giving their blood to obtain the power and servitude of demons.
* **Geomancer** - Deeply in tune with their environemnt, these casters adapt to their surroundings as their powers wax and wane with the seasons.
* **Infected** - The tainted blood of these once proud knights is a carrier for all types of diseases which they freely employ to bring low any who would stand before them. 
* **Exorcist** - These spiritual specialists have learned how to attack the corporeal essence of maladies, literally beating away ailments and pain. Of course, that doesn't stop them from bashing their enemies on the physical plane as well.
* **Gladiator** - Once legionnaires, these battle-tested warriors know the strategies and formations of war as well as the tactics and grit of those fighting to survive in the colesseum. 
* **Time Traveler** - Having been to the distant future, these unusual combatants are gifted at affecting the flow of time and using futuristic X-weapons. 
* **Fell Arbiter** - Only a powerful marked can channel the dark energies of the Maw to become a Fell Arbiter, but while doing so grants great power, the Maw's infuence corrupts those who would channel its power - tempting them to sacrifice all that they hold dear for greater boons. 
* **Scout** - Speedy and mobile, scouts specialize at weakening and disabling enemies from afar with guns and hazardous canisters. Though the range of their canister launcher is impressive, it can only shoot in straight lines.
* **Inner Demon** - Accepting the Maw's dark energy into them, these daring warriors move further along the path to demonhood, gaining abilities to affect and destroy the mind. They also become much more dangerous to attack. 

### Complete Equipment List
* **X-Targeting Taser** (GUN) - Advanced shocking technology, unlikely to miss (+15 accuracy). 
* **X-Bomber** (GUN) - Causes a point-blank dangerous yet inaccurate explosion (-10 accuracy).
* **X-Piercer** (GUN) - A straight-shooting contraption designed to pierce multiple targets.
* **X-Afflicter** (GUN) - Shoots darts designed to weaken a target's immune system. Debuffs have 10% increased chance to apply.
* **X-Time Displacer** (GUN) - Temporal distortion shots from this weapon delay enemy turns. 
* **X-Amplifier** (GUN) - This magical conduit channels electricity and greatly increases the magical reach of its user. 
* **X-Ambusher** (GUN) - Deals 50% more damage to enemies with full {hp}.
* **Eviscerator** (SWORD) - An unwieldy but lethal blade (-5 accuracy, grants {addpositive} when using a Regular Attack).
* **Wind Dancer** (Dagger) - The wind spirit inside makes you feel lighter than air (grants {addpositive} when using a regular attack from the sides or back).
* **Shaper's Finger** (STAFF) - Concentrates magical power to nearby attacks (Decreases the range of Ranged Spells by 1).
* **Valuter** (SPEAR) - The weapon's flexible shaft helps the user to vault great heights.
* **Insight** (MACE) - Magical knowledge swirls within (grants +2MP per turn).
* **Illusory Rod** (ROD) - Makes its bearer appear insubstantial (grants {addpositive} when HP is Critical at the start of a turn).
* **Harmony** (MAUL) - A weapon which calms the heart and aids the righteous, said to bolster one's Holy affinity.
* **Maw's Tooth** (RAPIER) - A true weapon of evil which shuns the light (+5 accuracy), said to bolster one's Dark affinity.
* **Throwing Axe** (AXE) - An axe that magically returns after being thrown, but leaves the user exposed.
* **Kraken Shell** (SHIELD) - Few weapons can pierce the shell of the mighty Kraken, though it's unmatched defense makes movement difficult.
* **Mind Cage** (HELMET) - A helm of great protection, but tight like a vise (-2MP per turn).
* **Believer's Blindfold** (HELMET) - Strike without fear against that which can't be seen (-15 accuracy).
* **Trapped Soul** (ACCESSORY) - Tapping into the power of a soul brings both great cost and great reward (grants +6MP per turn).