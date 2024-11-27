
# AS7 Radio Script

## Description
AS7 Radio is a customizable and feature-rich radio script designed for FiveM servers. It allows players to join radio channels, interact with others, and manage their communication seamlessly.

---

## Installation Guide

### Step 1: Download and Extract
1. Download the AS7 Radio script (this folder).
2. Extract the folder and ensure it's named `as7_radio`.

### Step 2: Add to Your Server
1. Place the `as7_radio` folder into your server's `resources` directory.
2. Add the following line to your server.cfg:
   ```
   ensure as7_radio
   ```

### Step 3: Configure (Optional)
1. Open `config.lua` to customize the settings (e.g., default radio channels, volume, etc.).

---

## How to install

### Step 1: Add items in Shared
1. Add a new item in your `qb-core/shared/items.lua` file:
   ```lua
    radio_blue                   = { name = 'radio_blue', label = 'Radio Blue', weight = 2000, type = 'item', image = 'radio_blue.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_brown                  = { name = 'radio_brown', label = 'Radio Brown', weight = 2000, type = 'item', image = 'radio_brown.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_cherry                 = { name = 'radio_cherry', label = 'Radio Cherry', weight = 2000, type = 'item', image = 'radio_cherry.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_green                  = { name = 'radio_green', label = 'Radio Green', weight = 2000, type = 'item', image = 'radio_green.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_mint                   = { name = 'radio_mint', label = 'Radio Mint', weight = 2000, type = 'item', image = 'radio_mint.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_orange                 = { name = 'radio_orange', label = 'Radio Orange', weight = 2000, type = 'item', image = 'radio_orange.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_pink                   = { name = 'radio_pink', label = 'Radio Pink', weight = 2000, type = 'item', image = 'radio_pink.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_purple                 = { name = 'radio_purple', label = 'Radio Purple', weight = 2000, type = 'item', image = 'radio_purple.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_red                    = { name = 'radio_red', label = 'Radio Red', weight = 2000, type = 'item', image = 'radio_red.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_yellow                 = { name = 'radio_yellow', label = 'Radio Yellow', weight = 2000, type = 'item', image = 'radio_yellow.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
    radio_white                  = { name = 'radio_white', label = 'Radio White', weight = 2000, type = 'item', image = 'radio_white.png', unique = true, useable = true, shouldClose = true, combinable = nil, description = 'You can communicate with this through a signal' },
   ```

### Step 2: Add the Item Images In Your Inventory
1. Copy the item images in Folder `icons` Place in the inventory scripts image folder (e.g., `qb-inventory/html/images/` or similar).

---

## Notes
- This script uses **pma-voice** for voice functionality. Ensure `pma-voice` is installed and configured correctly.
- For support, refer to the `guide.png` image in the script folder.

---

## Commands
- `/radio [channel]`: Join a specific radio channel.
- `/radiooff`: Turn off the radio.
- `/radiolist`: View all available channels.

---

## Credits
Developed by abusou7 from AS7 Team.
