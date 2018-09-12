<!-- TITLE: Modify Menu -->
<!-- SUBTITLE: Description of menus and how to change them for OvRride.com -->

# Menus
![Menu](/uploads/menu.png "Menu")

The menu bar at the top of the site is actually two menus. There's the logo and booking link on the left and the links on the right which collapse on small screens.

# Accessing Menus
## Log into admin dashboard
[https://ovrride.com/wp-admin](https://ovrride.com/wp-admin)

## Select **Menus** from the **Appearance** heading
![Apearance Menu](/uploads/apearance-menu.png "Apearance Menu")

Menus can be found from the **Appearance** heading in the admin dashboard



# Modifying a menu
## Current menus
* Logo and Booking
	*  OvRride Logo and link to shop, sits on left side of screen
	*  Will very rarely need to be edited
*  Main Menu
	*  Winter menu
*  Main Menu Summer
	*  Summer menu

## Select menu to edit
![Select Menu](/uploads/select-menu.png "Select Menu")

Select menu to edit from drop down. Most likely Main menu or Main Menu Summer. If you see brackets with text like ```(Main Menu Collapse)``` it means the menu is assigned to an area to be displayed.

click the **Select** button to continue.


## Menu view
![Menus](/uploads/menus.png "Menus")

Menu items are displayed in boxes. Existing items can be moved around by dragging.

### Menu items can be dragged into order
![Menu Drag](/uploads/menu-drag.png "Menu Drag")

### Menu items on the same level
![Menu Drag 3](/uploads/menu-drag-3.png "Menu Drag 3")

### Menu item nested under one level
![Menu Drag](/uploads/menu-drag.png "Menu Drag")

Watch the dotted outline to determine which level you're dropping the menu item into.
**Our current theme DOES NOT SUPPORT menu items nested 2 or more layers deep**

### Menu item reveal
![Menu Item](/uploads/menu-item.png "Menu Item")

clicking the disclosure triangle in the upper right hand corner of a menu item allows you to edit additional fields.
* Navigation label
	* Text that shows up in the menu for this item
	* By default WordPress uses the title of the item you add
* Title attribute
	* this is ignored by our theme, can be left blank
* Move
	* with the links here you can move the item by clicking links to move:
		* Up one  
		* Down one  
		* Out from under .....
* Remove
	*  removes menu item
* Cancel
	* closes menu item

## Removing an item
![Menu Item](/uploads/menu-item.png "Menu Item")

* Click the disclosure triangle in the upper right hand corner of the item
* Click the **Remove** link
* Click **Save Menu** button in the upper right hand corner of the window

## Adding an item
![Menu Categories](/uploads/menu-categories.png "Menu Categories")

There are quite a few options here. Typically our menu is made up of only **Pages, Products and Custom Links**. Some of the other categories may not give you the output you're expecting.

![Menu Pages](/uploads/menu-pages.png "Menu Pages")

Each category will look like this. Pages will be the most common as it makes up all the **Destination** and **Bus Stop** pages/menu items.
Here you can search for **Pages** by name and you also get a list of recently made **Pages**
Select the checkbox for the item you wish to add and them clickthe **add to menu** button in the bottom right corner of the box.

### New items will be added to the bottom of the menu
[Moving menu items](#menu-items-can-be-dragged-into-place)

Be sure to save your changes when done.
	

  ## Considerations
	* Types of items good for the menu
		* Pages
			* Things like Destinations, Bus Stops
		* Products
			* Could put a link in the menu to a certain product in the shop
		* Custom Links
			* enter a custom url to any site
		* Other types
			* Make sure you know what you're doing here, other types are often custom post types added by plugins and might give you weird results
			* Shortcodes
				* Almost definetly going to cause issues, best to stear clear of these

	### Menu can only be two levels deep
	This is a limit imposed by part of our theme but it's good practice. The reason it's good to keep the menu nesting down is because deep menus are bad on mobile.
	