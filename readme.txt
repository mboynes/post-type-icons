=== Post Type Icons ===
Contributors: mboynes
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=5ANKZEUN8MR7W
Tags: custom post type, custom post types, icons, pizzazz
Requires at least: 3.6
Tested up to: 3.6
Stable tag: 0.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Quickly and easily add icons to your custom post types. Built for the new dashboard design that should come out with 3.7 (you can use the [MP6 Plugin](http://wordpress.org/plugins/mp6/) until then).

== Description ==

Does the pushpin not describe your custom post type? Here are 361 more icons to choose from. Icons are the GPL-compatible [Font Awesome Icons](http://fontawesome.io/).

This is the same icon features that comes with [SuperCPT](http://wordpress.org/plugins/super-cpt/), but pulled out of the plugin for those crazy birds who don't use it.


== Installation ==

1. Upload to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Figure out which icon you want to use. Go to Tools &rarr; Post Type Icons
4. In your theme or a plugin, set the icons in one of the following ways:
	a. Call the function `pti_set_post_type_icon( 'post_type', 'icon-name' );`
	b. Using the global variable $pti_icons, set the array key => value pair such that `'post_type' => 'icon-name'`


== Frequently Asked Questions ==

= Do I have to write code/edit my theme to use this plugin? =

For now, yes. The next version will come with a GUI.

= Does this do anything besides add icons? =

Not at all! If you want more functionality, check out [SuperCPT](http://wordpress.org/plugins/super-cpt/), which helps you create custom post types, custom taxonomies, and add meta boxes.

= This looks like crap =

If you're not using the new admin design, you can install and activate the [MP6 Plugin](http://wordpress.org/plugins/mp6/) to get it. If you are using the new admin design, post to the support tab with your browser/OS/WP Version details.
