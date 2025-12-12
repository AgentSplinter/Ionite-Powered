# Quick Guide how to utilize exposed features of this Mod

## **Materials and Components**

The primary purpose of this mod is to provide a [set of commonly needed items](https://imgs.xkcd.com/comics/standards_2x.png). 
This helps prevent situations where multiple mods add the same items repeatedly.

If you don’t want to be “the millionth mod” adding steel, copper, or similar materials, you can simply **add a dependency on this mod** and let it handle those items for you.

> **Note:**
> All items and blocks are tagged using the **common tag namespace**, so you don’t need to reference them directly. Simply use the appropriate tag instead.

## **Element / Periodic Table Key System** (Version 1.1.9c)

This mod includes a system that displays the **element symbol** in certain item descriptions. You can extend this system for your own items by following these steps:

> **Note:** Only one loaded mod needs to provide a translation key for a given item. If multiple mods provide keys for the same item, the **last loaded mod’s key will take priority**.

#### **How to Add Support for Your Items**

1. **Tag Your Item**
   One of the following tags is needed for the provided item
   * `c:ingots`
   * `c:raw_materials`
   * `c:dusts`
   * `c:gems`
   * `c:chemicals`

2. **Add a Localization Key for the provided item**
   ```
   element.bwc.%item_registry_name%
   ```

   **Example:**

   ```properties
   element.bwc.iron_ingot=Fe
   element.bwc.steel_ingot=St
   ```

3. **Done!**
   Once your item is tagged and the translation key exists, the tooltip will automatically display the element symbol.




## **Cell system**
WIP

## More to come once 1.2 is out
