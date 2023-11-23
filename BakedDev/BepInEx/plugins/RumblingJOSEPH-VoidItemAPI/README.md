# Void Item API

So I figured why not make this API because a lot of people ask how to create a void item, and this keeps the process really simple for people.

You can also now modify existing transformations using this, so thats pretty cool.

You will need to add the DLL as a reference for your project, which you can acquire by downloading off the thunderstore or from the "Current DLL" folder in the github repo.

I made a wiki for how to create void items manually on r2wiki, in case you may not want to depend on this API.

# Guide

Requirements:
- You must set this project as a dependency in your main cs file. It will break if it loads after your mod, obviously. Don't forget.
- If you are using an ItemDef from the vanilla game to reference in a transformation, you must call the method AFTER ItemCatalog initializes. Otherwise, you can use the string method at any point in time as long as the void item is valid.
- VoidItemAPI must be set as a dependency in your manifest.json when uploading.

Now that those are out of the way time for a mini-guide on how to use the API. It is pretty simple actually.

There are 4 different CreateTransformation methods you can choose from in the VoidTransformation class:

`CreateTransformation(ItemDef VoidItem, ItemDef TransformedItem)` <br />
`CreateTransformation(ItemDef VoidItem, ItemDef[] TransformedItems)` <br />
You can supply ItemDefs for these two to create your transformations, however remember that the ItemCatalog must be initialized before calling these.

`CreateTransformation(ItemDef VoidItem, string TransformedItem)` <br />
`CreateTransformation(ItemDef VoidItem, string[] TransformedItems)` <br />
You can use a string for these two if you want to call this before the catalog initializes. The string would simply be the name of the item you would use for the ItemDef. <br />
For example: Red Whip = RoR2Content.Items.SprintOutOfCombat, which would mean the string would be "SprintOutOfCombat"

There are also 2 different methods for modifying existing transformations in the table. <br />
The same rules apply to these methods about timing on using ItemDefs vs. Strings.

```c#
ModifyTransformation(ItemDef VoidItem, ItemDef CurrentTransformation, ItemDef NewTransformation, VoidItemModification.ModificationType type)
ModifyTransformation(string VoidItemName, string CurrentTransformationName, string NewTransformationName, VoidItemModification.ModificationType type)
```

With these two methods, you can modify or remove existing transformations by supplying the Defs or Names into these methods. If you are removing a transformation, just set the third parameter to null, and ensure that the fourth parameter is set to `VoidItemModification.ModificationType.Remove`, and the API will handle it for you. <br />
Examples: <br />
```c#
ModifyTransformation(DLC1Content.Items.CritGlassesVoid, RoR2Content.Items.CritGlasses, RoR2Content.Items.SprintOutOfCombat, VoidItemModification.ModificationType.Modify);  //This changes the transformation for lost seer lenses from the crit glasses to red whip
ModifyTransformation("CritGlassesVoid", "CritGlasses", null, VoidItemModification.ModificationType.Remove);  //This will remove the CritGlasses transformation on lost seer lenses
```

That's about it for the guide. You can declare the dependency at the top of your main class by typing: <br />
`[BepInDependency(VoidItemAPI.VoidItemAPI.MODGUID)]`

If you need any help with anything just ping me or shoot me a dm on the modding discord: @joseph#6783

Thanks to bubbet for showing me his method of using strings to get the ItemDef.
