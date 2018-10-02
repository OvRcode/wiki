<!-- TITLE: Create A Shortcode -->
<!-- SUBTITLE: Shortcodes are used to display content in various places on the site -->

# What is a shortcode?
> Since Version 2.5 WordPress supports so called Shortcodes. They have been introduced for creating macros to be used in a post's content.


See [WordPress Codex Shortcode Page](https://codex.wordpress.org/shortcode) for more details.

On our site we mostly use shortcodes for tab content, like the tabs on products, destination pages and bus stop pages.

### Tldr;
Shortcodes let you save bits of text and HTML and use them in pages, posts and possibly as widgets.

# Why shortcodes?
We use shortcodes for data that needs to be displayed in multiple places. When a shortcode is used you only need to edit the information in one place and then all the instances of the shortcode show the new content automatically.

# Log into admin dashboard
Vist [https://ovrride.com/wp-admin](https://ovrride.com/wp-admin)
If you cannot access the admin dashboard contact devops@ovrride.com to have your account checked out.


# Go to shortcode Page
![All Shortcodes](/uploads/all-shortcodes.png "All Shortcodes")
From the admin menu on the left side of the screen click **All Shortcode** from the **Shortcode** heading.

# Before adding a new shortcode
**Shortcode titles must be unique. If two shortcodes share the same title you might not get the one you expect when you use the shortcode.**
It is a good idea to search for the shortcode you intend to create to make sure it doesn't already exist.
![Shortcode Search](/uploads/shortcode-search.png "Shortcode Search")
The search box is in the upper right hand corner of the shortcode screen.

# Add new shortcode
![Shortcode Add New](/uploads/shortcode-add-new.png "Shortcode Add New")
Click the **Add new shotcode** button in the top left corner of the screen.

# New shortcode view
![Shortcode View](/uploads/shortcode-view.png "Shortcode View")

# Set title
The title is the text you will use to display the shortcode. If the title is **example_shortcode** then you would use the tag ```[example_shortcode]``` to display the contents.
Shortcode titles can only contain letters, numbers and under scores.
### Make sure to use underscores instead of spaces when making shortcode titles
![Shortcode Title](/uploads/shortcode-title.png "Shortcode Title")
The title field is in the upper left corner of the screen.
# Set body
The body is the content that the shortcode displays. You can edit this field just like a normal page or post. For some shortcodes like rates and bus times (destination pages only) certain formats are required for the content to display properly, it's probably best to find one from the shortcode search and take a look at the way the html is structured.
![Shortcode Body](/uploads/shortcode-body.png "Shortcode Body")

# Save
Either click **Publish** button or **Save as draft**. Drafted shortcodes will show the tag where they are saved instead of the content so if **example_shortcode** contains the text *example content* and it was set to draft you would see ```[example_shortcode]``` any where you have the shortcode being displayed.

Published shortcodes are not displayed anywhere until they are inserted into a place on the site where shortcodes can be displayed like a destination page, bus stop page or home page widget.