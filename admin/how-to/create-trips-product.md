<!-- TITLE: Create Trips Product -->
<!-- SUBTITLE: How to create a day trip product with one package field -->

# Log into admin dashboard
[Visit https://ovrride.com/wp-admin](https://ovrride.com/wp-admin)

Your account will need to have either "Administrator","Shop manager" or "OvR Staff" roles assigned to create products. Contact [devops@ovrride.com](mailto:devops@ovrride.com) if you need to have your existing account upgraded.

# Product Menu
Find the product menu on the left hand side of the dashboard
![Product Menu](/uploads/product-menu.png "Product Menu")

click "Add New" from the products sub menu. You can also click on the "products" heading and it will take you to all products, from there the hovering menu is displayed under the products heading.

# Add New Product
![Add New Product](/uploads/add-new-product.png "Add New Product")

You are now creating a new product. You can save at any time by hitting the "Save Draft" button on the top right, this will keep the product hidden from the store until it's completed and ready to go.

In order to reduce the places around the site we need to edit text all products should use [shortcodes](#) to display as much information as possible. 
For this example you will create a Killington Snow Fiend Trip for November 17th, 2018.

This product will feature the following packages and prices:

| Package | Price |
| --- | --- |
| All Area Lift & Bus | 119.95 |
| All Area Lift, Bus & Board Rental | 149.95 |
| All Area Lift, Bus & Ski Rental | 149.95 |
| Bus & Board Rental | 109.95 |
| Bus & Ski Rental | 109.95 |
| Bus Only | 79.95 |

This product will use the following pickups or bus stops:
| Name | Time |
| --- | --- |
| Skate Brooklyn | 03:30am |
| Cobble Hill, BK | 03:45am |
| Union Square (NW of UNSQ Park) | 04:00am |
| The North Face UWS | 04:30am |

# Set the title
Titles should follow a standard format. The format is {**DESTINATION NAME**} {**TRIP TYPE**} . Dates should be avoided in product titles, all trip products have a date field and the date should be displayed in appropriate places around the shop/site. If you spot a location where the date is missing or looks wrong contact [devops@ovrride.com](mailto:devops@ovrride.com).

For this trip the title would be "Killington Snow Fiend" .
Enter the title in the title box at the top of the page and click "Save Draft".

# Change product type
Find the "Product Data" section on the form and select "Trips Product" from the dropdown. 
Make sure the "Virtual" checkbox is checked.
Save draft.

# Set SKU and Permalink
SKU is a unique identifer for this product. SKUs should follow the format **DESTINATION CODE**-**2 digit month**-**2 digit day**-**2 digit year** .

![Sku](/uploads/sku.png "Sku")
Insert the SKU for this example under the "General" tab using the SKU field add the value **K-11-17-18**

The permalink is the address where the product will be available. By default WooCommerce uses a version of the title but that can be long and ugly. The permalink should be a unique value. Since the permalink should be short **and** unique the SKU should be used in this field too.

![Permalink](/uploads/permalink.png "Permalink")
Set the permalink by hitting the "edit" button next to the permalink under the title at the top of the page. 
Use the SKU value **K-11-17-18** for the permalink value.
Click "ok" to save the permalink.

# General tab
![General Tab](/uploads/general-tab.png "General Tab")
Settings and explanation
* Manage Product Stock: Yes
	* Yes = Manage Stock on this product
	* No = No stock management, could be used if there was stock management on packages
* Stock Status: Instock
	* Instock: product is in stock and purchasable
	* Out of stock: product is not purchasable, could still be visible
* Stock: 50
	* 52 passengers per bus - Trip Leader - Second
* Base Price: 0
	* Field could be used to set a price and have packages add onto that base.
* Destination: Killington
	* If this is the first trip to a destination you might need [HOWTO: Setup a destination](#)
	* This setting helps populate:
		* lists mountain contact info
		* trail map on the products
		* mountain specific lesson age restrictions
* Trip type: Bus
	* Bus: Day/Multi-day trips with packages
	* Beach Bus: Day trips with multiple packages and 2 bus routes
	* Flight domestic/international: Trips with flights, forms are different for domestic/international
* Age Check: 18
	* limits the age for people signing up for the trip
	* values: 18, 18+, 21, 21+
	* values with + have a hard limit on age
	* values without + allow underage and display ovrride age policy on the form
* Start Date: November 17, 2018
	* Clicking this field should bring up a date picker
	* Setting this field helps the trip show up on the calendar and events fields properly
* End Date: November 17, 2018
	* Clicking this field should bring up a date picker
	* Setting this field helps the trip show up on the calendar and events fields properly