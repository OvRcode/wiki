<!-- TITLE: WooCommerce Product Types -->
<!-- SUBTITLE: product types and settings -->

# Types of products
WooCommerce has four built in product types and we run a custom product type for trips.

## Product settings
* Virtual: There is no physical product, nothing to ship
* Downloadable: This product has a file the customer downloads after purchase. Could be paired with the virtual setting but could also be an add on to a physical item
* Type: Simple Product, Grouped Product, External/Affiliate Product, Variable Product, Trips Product
 
## Simple Product
Simple products are the basic WooCommerce product. You can assign shipping info like dimensions, set prices, set stock levels etc.
In our shop items like physical products (hats, beanies, coozies, goggles) would be simple products. Gift cards and high fives are also simple products.

### General Settings
* Regular Price: Price of the product
* Sale Price: Sale price of product, can also be set on a schedule
* Coupons: Customers who buy this product will recieve the selected coupon/s

### Inventory Settings
* SKU: a unique identifier for this product. EX: XX1999
* Manage Stock?: Checked = Manage inventory for this product, Unchecked = manually set in/out of stock on the product page
	* Stock Quantity: Number of items in stock, when zero is reached product will be out of stock
	* Allow backorders?: Take back orders when product is out of stock
* Sold individualy?: Only allow one per order

### Shipping Settings
Physical dimensions of the object and a shipping cost class.

### Linked Products
* Upsells: Recommend something instead of this product
* Cross-sells: Recommend something to go with this product

[HOW TO: Create a gift card product](#)


## Grouped product
A collection of simple products. 
Ex: Selling an album with the option to buy individual tracks


## External/Affiliate Product
Link to a product sold on another store.

### General Settings
* Product URL: Link to product
* Button Text: Text on button

## Variable Product
Products with selectable attributes like T shirts with selectable size and color.
[WooCommerce Variable Products Documentation](https://docs.woocommerce.com/document/variable-product/)

## Trips Product
Our custom plugin with offers the ability to assign a date/s to the product, packages and to collect rider information.

### Virtual Setting
Every trip should be set to virtual unless we're mailing out some kind of physical item for a special event.


### General Settings
Just going over the differences from simple product.
* SKU and Stock settings are on the general tab
* **Destination:** Assign a destination to this trip
	* [HOW TO: Create a new destination](#)
* **Trip type:**
	* This setting will impact the form shown to the customer and fields available for packages
	* Bus: This is a bus based trip with one set of pickup locations and up to 3 packages. Can be single or multi-day
	*  Beach Bus: Bus based trip with multiple routes.
*  **Age check:**
	*  Is the guest at least X years old?
	*  options are 18, 18+, 21, 21+
		*  options with + have a hard limit on birthday
		*  options without plus allow underage and show a link to our age policy
	*  **Start Date:** Starting date of trip
		*  it's important that the start/end dates are right so the trip shows up on the calendar properly
	*  **End Date:** End date of trip

