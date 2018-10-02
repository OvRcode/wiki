<!-- TITLE: Create A New Destination Page -->
<!-- SUBTITLE: Create a front end page for a destination -->

# Destination page vs destination
Destination pages are just a window dressing to show products organized in a category. A destination in the system allows the trips plugin to store some custom information and helps us organize trips on the lists.
[HOW TO: Create a new Destination](https://wiki.ovrride.com/how-to/create-a-new-destination)

# Log into admin dashboard
Vist [https://ovrride.com/wp-admin](https://ovrride.com/wp-admin)
If you cannot access the admin dashboard contact devops@ovrride.com to have your account checked out.

# New Page
![Page Add New](/uploads/page-add-new.png "Page Add New")
From the admin menu on the left side of the screen select **New Page** from the **Pages** heading.

# New Page view
![Destination Page View](/uploads/destination-page-view.png "Destination Page View")

# Set Page Title
![Destination Page Title](/uploads/destination-page-title.png "Destination Page Title")

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
![Destination Page Body](/uploads/destination-page-body.png "Destination Page Body")

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

The Destination Page template only uses the custom fields for tab data.
Fields named **tabs** have a **value** which is used for the tab label and as part of the second field with the tab content. Names should be lower case with no special characters except underscores to replace spaces.
Fields named **tab**_my_tab_name should contain shortcodes to be used for tab content			

For destination pages tabs usually include bus times, rates, includes, description, pics & video.

Values to set:
| Name | Value |
| --- | --- |
| tabs | my_tab |
| tab_my_tab | [my_tab_info] |

Click **Enter new** and then fill in pairs of names and values.
The order of the **tabs** fields will determine the order of the tabs.

 Need to make a new shortcode? [HOWTO: Create a new shortcode](https://wiki.ovrride.com/how-to/create-a-shortcode)

# Save
Click **Save draft** or **Publish**

# Add to Site Menu
[HOW TO: Modify Menu](https://wiki.ovrride.com/how-to/modify-menu)