# Inventory UI (AGR) 
User Interface for 'AGR' inventory items

This is the alpha step of the plugin to show the concept. All the code is still under development and bugs may occurred.
You can add code or edit it at any time.

How to use the system with your own project:

1. First of all install the AGR PRO plugin from EPIC Store it does not cost money and it is a useful plugin for many things beyond inventory.

2. Add "AGR_InventoryManager" to your CharacterBP.

3. Create an empty 'Player State' and register it in the game mode.

4. Close your project with AGR installed. Migrate or copy the "InventoryUi" folder to your project 'content' folder.

5. Edit the blueprints:
  a. Character BP: Add "Inventory_BPC" to your character.
  
  b. Create input for opening the inventory UI in project settings,on characterBP pull from "Inventory_BPC" and connect the command that says "show/hide inventory",       connect 'close key' pin to the input key.
  
  c. Create input for highlight items in project settings, on characterBP pull from "Inventory_BPC" and connect the command that says "Highlight Items (on)" for pressed,   and "Highlight Items (off)" for Released. (You can add a delay before canceling
  For a slightly more appealing effect).

  d. add begin play event and pull from "inventoryBPC" the command "create inventory ui Widget", add remove from parent after and connet to the command Output.

That's all, now everything should work.
You can add objects at any stage, the tutorial will go up later. the inventory currently supports up to 40 places and you can always add more, the demo project includes some objects that demonstrate that everything can be done,
enjoy.

-UnLuckyLust Bluprint-
