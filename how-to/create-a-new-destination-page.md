<!-- TITLE: Create A New Destination Page -->
<!-- SUBTITLE: Create a front end page for a destination -->

# Destination page vs destination
Destination pages are just a window dressing to show products organized in a category. A destination in the system allows the trips plugin to store some custom information and helps us organize trips on the lists.

# Log into admin dashboard
Vist [https://ovrride.com/wp-admin](https://ovrride.com/wp-admin)
If you cannot access the admin dashboard contact devops@ovrride.com to have your account checked out.

# New Page
![Page Add New](/uploads/page-add-new.png "Page Add New")
From the admin menu on the left side of the screen select **New Page** from the **Pages** heading.

# New Page view
![Destination Page View](/uploads/destination-page-view.png "Destination Page View")

# Set Page Title

This field will be displayed as the title on the destination page. 
The title field is at the top of the page.
Click **save draft** when done.

# Set Page Attributes
![Page Attributes](/uploads/page-attributes.png "Page Attributes")

Setting the correct **Parent** here helps with organization. Setting the correct **Page Template** will let the site process the information here to display as a destination template.
Values:
* Parent: Destinations
* Template: Destination
* Order: 0

Click **Save draft**

# Set WooCommerce Product shortcode
In the body of the **Page** you need to add a **shortcode** which will display a category of products from the shop.
You are going to need to know the **slug** for the category in this short code. The **slug** is a version of the **product category name** in which the name is lower case and the spaces are replaced with dashes.
Ex: 
Category: My Category Slug: my-category

You can search for categories by visiting [Products > Categories](https://ovrride.com/wp-admin/edit-tags.php?taxonomy=product_cat&post_type=product)
<!-- COME BACK AND MAKE THIS: If this is a new stop and not on any products yet then you may need to [HOW TO: Create a new product category](#) -->


In the body of the page enter the following shortcode with your product category slug added
``` 
  [product_category category="slug-here" per_page="40" columns="4" orderby="date" order="desc"]
```
Click **Save draft**

# Set Custom Fields
![Destination Page Custom Fields](/uploads/destination-page-custom-fields.png "Destination Page Custom Fields")
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


