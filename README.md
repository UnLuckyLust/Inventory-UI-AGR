# Inventory UI (AGR) 
## User Interface for 'AGR PRO' inventory items

This is the alpha step of the asset to show the concept. All the code is still under development and bugs may occurred.
You can add code or edit it at any time.

### [Tutorial and Demo](https://www.youtube.com/watch?v=7rLUUwoELsc)

### How to use the system with your own project:

1. First of all install the AGR PRO plugin from EPIC Store it does not cost money and it is a useful plugin for many things beyond inventory.

2. Add "AGR_InventoryManager" to your CharacterBP.

3. Create an empty 'Player State' and register it in the game mode.

4. Close your project with AGR installed. copy "InventoryUI" folder to your project "Content" folder.

5. Edit the blueprints:
  
 * a. Add "InventoryUI_BPC" to your character BP.
  
 * b. Create input for opening the inventory UI in project settings, on character BP pull from "InventoryUI_BPC" and connect the command that says "show/hide inventory",
  connect 'close key' pin to the input key.
  
 * c. Create input for highlight items in project settings, on characterBP pull from "InventoryUI_BPC" and connect the command that says "Highlight Items (on)" for       
  pressed,   and "Highlight Items (off)" for Released. (You can add a delay before canceling
  For a slightly more appealing effect).

 * d. add begin play event and pull from "inventoryUI_BPC" the command "Create inventory ui Widget", add remove from parent after and connet to the command Output.

6. Navigate to the 'InventoryUI/Base' folder. You will find actor named "Item_Demo", 
This will be the actor that you can change and edit, to add more item just duplicate this actor and change the 'default class' information in the inventory ui category.

That's all, now everything should work.
the inventory currently supports up to 40 places and you can always add more.

enjoy.

### -UnLuckyLust Bluprint-
