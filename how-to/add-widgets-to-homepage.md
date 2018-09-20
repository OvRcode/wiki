<!-- TITLE: Add Widgets To Homepage -->
<!-- SUBTITLE: Add a widget or tile to the home page -->

# Widgets
[What is a widget anyway?](https://www.wpbeginner.com/glossary/widgets/)

Most of the elements on the home page are widgets. By making these elements widgets we can easily re-organize elements and change the layout of the page more easlily.

# Log into admin dashboard
Visit [https://ovrride.com/wp-admin](https://ovrride.com/wp-admin/)
If you cannot access the admin dashboard contact [devops@ovrride.com](mailto:devops@ovrride.com) to have your account checked out.

# Go to Appearance > Widgets
![Appearance Widgets](/uploads/appearance-widgets.png "Appearance Widgets")
From the admin dashboard look for the **Widgets** link under the **Appearance** heading

# Widgets View
![Appearance Widgets View](/uploads/appearance-widgets-view.png "Appearance Widgets View")

On the left side of the screen the grey boxes contain all the widgets available on the site. On the right side of the screen you see the areas of the site where widgets can be assigned.
**Note:** Widgets can also be assigned to an **Arbitrary** category. From there you can use the widget's **shortcode** to embed it in a post or a page.

# Custom widgets:
We have a custom plugin on the site that provides a number of widgets specific to trips or the way we run the site.

 * **OvR Blog Feature**
	 * Select a blog post to display in a tile
	 * Fields:
		 * Selected post: list of blog posts as titles, should be in date order
		 * Primary Image: 225px x 150px 
			 * Image to Show at top of tile
			 * You can upload a larger or smaller image but it will throw off the display on the tile
		 * Secondary Image: 150px x 50px
			 * This is designed to have a 150x50px mountain logo, like we use on product pages as the featured image.
	 * **OvR Calendar**
		 * The widget that drives the large and small calendars on the site.
		 * Fields:
			 * Mini: Unchecked = Large Calendar, Checked = Mini calendar (this is used on the homepage)
	 * **OvR Contact Form**
		 * **CURRENTLY NOT WORKING**, looking to get this fixed before 18/19 winter season
		 * A widget to get contact information and some text and email it to a specified email address
		 * Fields:
			 * Recipient: email where the completed form is sent
			 * Recipient Name: Name label on email
			 * Phone Number: Customer service email
	 * **OvR Email Signup Form**
		 * Widget for constant contact signup
		 * Fields: None, just assign it in a category and save
	 * **OvR Jumbotron**
		 * Used to display a large feature story, **NO LONGER IN USE**
	 * **OvR Dual Trip Feature**
		 * Display Two trips in a tile with one featue image and description text
		 * Fields:
			 * Widget title: *25 Character limit*, title shown at top of tile
			 * Widget Excerpt: *126 Character limit*, text shown under image
			 * Widget Main Image: *588x235px*, image shown at top of tile
				 * Images are not limited to this size but if you use an image with different dimensions it will throw the display of the widget off
			 * Trip One/Two: Fields are the same for these two sections
				 * Trip: List of titles of active trips arranged alphabetically
				 * Trip X image: *150x50px*, standard destination logo size for widgets and products
		 * **OvR Medium Trip Feature**
			 * This widget takes up two slots and shows 1 trip, basically the single trip version of the Dual Trip widget
		 * **OvR Trip Feature**
			 * Single trip, single slot. fields are basically the same as the dual trip widget.
		 * **OvR Featured Video**
			 * Displays a video player
			 * Fields:
				 * Video title: Title to display on widget
				 * Video URL: Vimeo or YouTube url
		 * **OvR Upcoming Events**
			 * This widget is the upcoming events feed shown at the top of the site under the menu
			 * Fields:
				 * Number of events to list: *1 to 30*, Default: 30
				 * Override date sorting with menu order field on products: checked = order products by menu order then date, unchecked = sort by date only
				 * Number of seats left to initiate countdown: *1-52*, Default: 30
			 * **OvR Wide/Small Ad**
				 * Display an image with a link and a title
				 * Need to find dimensions 


# Widget Areas
With the current theme you will find the following **Areas** where widgets can be assigned:
* Sidebar
	* This is a default WordPress area and is not used by our theme
* Top Banner Ad
	* This area shows up between the events feed and the body of the site
* Bottom Banner Ad Left/Right
	* These areas show up between the footer and the bottom of the site body
* Upcoming Events
	* This area is for the upcoming events widget and is displayed on every page of the site. This area displays directly under the menu.
* Feature Main/Top/Bottom
	* These areas make up the top of the site. Typically there is a slider in the *Feature Main* area, calendar in the *Feature Bottom* and Sponsor Ad in the *Feature Top*
* Rows One -> Four
	* The rest of the home page is divided into 4 rows
	* Each row has a left and right side
		* small widgets will fit two to a side
		* medium one to a side
* Footer Newsletter
	* The old space we used to keep the newsletter sign up form
* Arbitrary
	* This space has no display
	* This is a good space to start empty widgets and get them setup before putting them on the home page
	* You can save a widget here and then use the shortcode for the widget to put it on a page

# Add a widget
## Select widget
* Click on name of widget
* Select Area to Assign Widget
	* can be changed later
	* if you set it to **Arbitrary** first you can set the settings then move it when everything is set
* Set settings for widget and click Save

## Move widget 
Click and drag the widget from the existing area and move it to the new area

