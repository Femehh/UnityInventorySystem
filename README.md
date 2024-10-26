# UnityInventorySystem
Step 1: Create a New Unity Project
Open Unity Hub and create a 3D project.
Name it something like ModularInventorySystem.
Step 2: Set Up the Scripts
In the Project window, right-click and create a new folder named Scripts.
Inside the Scripts folder, create a C# script named InventorySystem.cs by right-clicking and selecting Create > C# Script.
Repeat the process to create a second script called ItemPickup.cs.
Step 3: Add the Script Code
Open InventorySystem.cs and ItemPickup.cs and replace any existing code with the code provided in the previous answer.
Save both scripts (Ctrl+S or Cmd+S).
Step 4: Set Up Inventory UI Elements
Create a Canvas for the inventory UI:
Right-click in the Hierarchy and select UI > Canvas.
Rename it to InventoryCanvas.
Create an Inventory UI Panel:
Inside InventoryCanvas, right-click and select UI > Panel.
Rename it to InventoryUI.
Adjust the size and position to fit your screen layout.
Add a Grid Layout Group component to InventoryUI to help organize items.
Create Item Slot Prefabs:
Right-click inside the Project window and create a Prefab folder.
Inside Prefab, create an empty UI > Image (call it ItemSlot) and make it a prefab by dragging it into the Prefab folder. This will represent an item slot.
Step 5: Configure the Inventory System
Attach the InventorySystem Script:
Create an empty GameObject in the Hierarchy, name it InventoryManager, and attach the InventorySystem.cs script to it.
Set Inspector Values:
With InventoryManager selected, look at the InventorySystem component in the Inspector.
Set Max Inventory Size to the desired number of slots (e.g., 20).
Assign InventoryUI to the Inventory UI field.
Drag the ItemSlot prefab to the Item Slot Prefab field.
Step 6: Setting Up an Item Pickup
Create Item Prefabs:
Create a 3D object (e.g., a cube or sphere) in the scene to act as a pickup item.
Attach the ItemPickup script to this object.
In the Inspector, configure the InventoryItem properties (like name, quantity, and whether it’s stackable).
Set Up Item Prefab:
Assign an icon and set other attributes, like stackability.
Save the item as a prefab by dragging it to the Prefabs folder.
Step 7: Test the System in Play Mode
Press Play in the Unity editor.
Move your player near the item and press E to pick it up.
Press I to open or close the inventory and see the items you’ve collected.
Step 8: Customize and Expand
To add more functionality:

Customize the InventoryItem properties to include attributes like weight, rarity, or effects.
Configure Unity Events:
Under Inventory Events in InventorySystem, add functions (e.g., sound effects, animations) to run when items are picked up or dropped.
Recap
InventorySystem manages the inventory, handles item pickup/drop, and toggles inventory display.
ItemPickup holds individual item data.
Inventory Canvas shows items in UI, and each item is represented by an ItemSlot prefab.
