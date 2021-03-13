# Fusion Furnace

Class Path: `mods.morerefinedstorage.FusionFurnace`

## Use

To use, import the class with `import mods.morerefinedstorage.FusionFurnace;` at the beginning of your script

## Adding a Recipe

### With standard experience

`FusionFurnace.addRecipe(output, itemLeft, itemRight, catalyst)`

- `output` <[IItemStack](https://docs.blamejared.com/1.12/en/Vanilla/Items/IItemStack/)>
- `itemLeft` <[IIngredient](https://docs.blamejared.com/1.12/en/Vanilla/Variable_Types/IIngredient/)>
- `itemRight` <[IIngredient](https://docs.blamejared.com/1.12/en/Vanilla/Variable_Types/IIngredient/)>
- `catalyst` <[IIngredient](https://docs.blamejared.com/1.12/en/Vanilla/Variable_Types/IIngredient/)>

**Example:**
```zenscript
import mods.morerefinedstorage.FusionFurnace;

FusionFurnace.addRecipe(<minecraft:diamond>, <minecraft:coal_block>, <minecraft:redstone>, <minecraft:apple>);
```

### With custom experience

`FusionFurnace.addRecipe(output, itemLeft, itemRight, catalyst, experience)`

- `output` <[IItemStack](https://docs.blamejared.com/1.12/en/Vanilla/Items/IItemStack/)>
- `itemLeft` <[IIngredient](https://docs.blamejared.com/1.12/en/Vanilla/Variable_Types/IIngredient/)>
- `itemRight` <[IIngredient](https://docs.blamejared.com/1.12/en/Vanilla/Variable_Types/IIngredient/)>
- `catalyst` <[IIngredient](https://docs.blamejared.com/1.12/en/Vanilla/Variable_Types/IIngredient/)>
- `experience` float

**Example:**
```zenscript
import mods.morerefinedstorage.FusionFurnace;

FusionFurnace.addRecipe(<minecraft:diamond>, <minecraft:coal_block>, <minecraft:redstone>, <minecraft:apple>, 2.0);
```

## Removing a Recipe

`FusionFurnace.removeRecipe(output)`

- `output` <[IItemStack](https://docs.blamejared.com/1.12/en/Vanilla/Items/IItemStack/)>

**Example:**
```zenscript
import mods.morerefinedstorage.FusionFurnace;

FusionFurnace.removeRecipe(<minecraft:diamond>);
```

## Existing Recipes

### Fusion Recipes

- `<morerefinedstorage:crystalized_ingot>`