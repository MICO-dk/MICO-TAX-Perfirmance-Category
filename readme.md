# MICO Custom Taxonomy: Performance Category
This is a very simple plugin, with the only purpose of adding a 
translation ready taxonomy named "performance-category" to wordpress. 

Out of the box you wont be able to see this in the admin. 
You need to add it to an existing post type like so:

```PHP
 
	/**
	 * Add taxonomies to objects
	 */
	add_action( 'wp_loaded', 'add_tax_to_post_type', 0);
	function add_tax_to_post_type() {
		register_taxonomy_for_object_type('performance_category', 'performance');
	}

```

Best to add this to a client-function plugin

##Languages
So far this plugins comes with translations for
* danish
