<!-- TITLE: Create Bus Stop Page -->
<!-- SUBTITLE: Generate the public page for a bus stop -->

#### Page vs Pickup location
Pickup locations are custom post types used by the trips plugin to store information about bus stops. This information is used by the plugin to display names and stop times on the booking forms and also used by the lists to find information about the stops.

A bus stop page is a page that is generated by hand using a template. When we add a bus stop to a product we also add a category to the product with the same name. 

# Log into Admin Dashboard
Visit [https://ovrride.com/wp-admin](https://ovrride.com/wp-admin) and log in.

If you do not see the admin dashboard or toolbar after logging in contact [devops@ovrride.com](mailto:devops@ovrride.com) and we will get your account privileges sorted out.

# Add Page
![Page Add New](/uploads/page-add-new.png "Page Add New")

From the **Page** heading in the admin menu on the left side of the page click **Add New**

# Add Page View
![Page Add View](/uploads/page-add-view.png "Page Add View")

# Set Page Title
![Add New Page](/uploads/add-new-page.png "Add New Page")

This field will be displayed as the title on the bus stop page. It's best to use the same name as the pickup location for which you're making the page.
The title field is at the top of the page.
Click **save draft** when done.

# Set Page Attributes
![Page Attributes](/uploads/page-attributes.png "Page Attributes")

Setting the correct **Parent** here helps with organization. Setting the correct **Page Template** will let the site process the information here to display as a bus stop template.
Values:
* Parent: Bus Stops
* Template: Bus Stop
* Order: 0

Click **Save draft**

# Set WooCommerce Product shortcode
In the body of the **Page** you need to add a **shortcode** which will display a category of products from the shop.
You are going to need to know the **slug** for the category in this short code. The **slug** is a version of the **product category name** in which the name is lower case and the spaces are replaced with dashes.
Ex: 
Category: My Category Slug: my-category

You can search for categories by visiting [Products > Categories](https://ovrride.com/wp-admin/edit-tags.php?taxonomy=product_cat&post_type=product)
<!-- COME BACK AND MAKE THIS: If this is a new stop and not on any products yet then you may need to [HOW TO: Create a new product category](#) -->

![Page Body](/uploads/page-body.png "Page Body")
In the body of the page enter the following shortcode with your product category slug added
``` 
  [product_category category="slug-here" per_page="40" columns="4" orderby="date" order="desc"]
```
Click **Save draft**

# Set Custom Fields
![Page Custom Fields](/uploads/page-custom-fields.png "Page Custom Fields")
The rest of the information for this template will be pulled from custom fields. You will be exclusively using the **Enter New** section of this form to add pairs of  **Name** and **Value** fields.

Two things are retrieved from the custom fields for this template.
1. Google Map information
	* **NAME:** bus_stop
	*  **VALUE:** Google Map Place Name
		*  If the location has a name when you search for it on google maps, like [The IFC Center](https://www.google.com/maps/place/IFC+Center/@40.731225,-74.001423,19z/data=!4m5!3m4!1s0x0:0xdae73e0f53cd2d4d!8m2!3d40.7312056!4d-74.0016722?hl=en-US) you can use the name instead of the address
		*  The IFC Center has the address: 323 6th Ave, New York, NY 10014
			*  you could use either one in the **bus_stop** field
2. Tab information
	* 2 fields are required to make a tab
		* **NAME:** tabs **VALUE: tab_name**
			*  you can have multiple fields with the same name, the tabs setup relies on this
		*  **NAME:** tab_tab_name **VALUE:** [shortcode_for_tab_content]
			*  use a short code here to display content
			<!--*  COME BACK AND MAKE THIS[HOW TO: Create a shortcode](#) -->
	* You need to make a set of these fields for each tab you would like to show under the map
			
Values to set:
| Name | Value |
| --- | --- |
| bus_stop | Place Name or Address |
| tabs | my_tab |
| tab_my_tab | [my_tab_info] |

Adding fields:
* Click the **Enter New** link.
* Type the **Name** in the field above the link.
* Add the shortcode to the **Value** field.
* Click **Add Custom Field**
* Repeat for each value you need to add.

In this example **My Tab** would be the label of the tab and the shortcode with the title **my_tab_info** would be displayed.
Bus stop pages should contain a tab for each destination that picks up there. The order of the tabs is controlled by the order of the **tabs** fields.

The following is an example template taken from the Windham REI SoHo stop and should be saved in a short code. 
```
Departing from:
303 Lafayette Street (On Lafayette South of Houston)
New York, NY 10012

Trips Scheduled Regularly Throughout the Season on Wednesdays & Sundays

Bus Departs at 6:00am
```
<!-- COME BACK AND MAKE THIS PAGE [HOW TO: Create a shortcode](#) -->

# Publish
Click the **Publish** button to Publish this page.

# Add to Site Menu
[HOW TO: Modify Menu](https://wiki.ovrride.com/how-to/modify-menu)