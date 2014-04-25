=== Post Type Icons ===
Contributors: mboynes
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=5ANKZEUN8MR7W
Tags: custom post type, custom post types, icons, font-awesome, pizzazz, ui
Requires at least: 3.6
Tested up to: 3.9
Stable tag: 0.2.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Quickly and easily add Font Awesome icons to your custom post types.

== Description ==

Does the pushpin not describe your custom post type? Here are hundreds more icons to choose from. Icons are the GPL-compatible [Font Awesome Icons](http://fontawesome.io/).

This is the same icon features that comes with [SuperCPT](http://wordpress.org/plugins/super-cpt/) 0.2+, but pulled out of the plugin for those crazy birds who don't use it.

This adds a function you can use, `pti_set_post_type_icon( $post_type, $icon );` to set your post type's icon. For instance, `pti_set_post_type_icon( 'event', 'calendar' );`. You can also set the global variable $pti_icons as an array of post type => icon names. Using the global variable is safer, since it doesn't rely on a function (you could of course call `if ( function_exists( 'pti_set_post_type_icons' ) )` to be equally safe using the function).


== Installation ==

1. Upload to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Figure out which icon you want to use. Go to Tools &rarr; Post Type Icons page for a reference.
4. In your theme or a plugin, set the icons in one of the following ways:
	a. Call the function `pti_set_post_type_icon( $post_type, $icon_name );`, e.g. `pti_set_post_type_icon( 'event', 'calendar' );`
	b. Using the global variable `$pti_icons`, set the array key => value pair such that `'post_type' => 'icon-name'`, e.g. `$GLOBALS['pti_icons']['event'] = 'calendar';`


== Frequently Asked Questions ==

= Do I have to write code/edit my theme to use this plugin? =

For now, yes. The next version will come with a GUI.

= Does this do anything besides add icons? =

Not at all! If you want more functionality, check out [SuperCPT](http://wordpress.org/plugins/super-cpt/), which helps you create custom post types, custom taxonomies, and add meta boxes.

= I set my icons and they're never going to change. Is there a way to remove the plugin overhead and make it static? =

Sure thing! The plugin pretty much just adds CSS to the admin which get added to the document head. Move those to your theme/plugin (not your main style.css since this is the admin panel, you'll need an admin-only CSS file). You can leave the paths the same if you don't plan on uninstalling the plugin (you can still deactivate the plugin). If you want to uninstall it, you'll have to copy the fonts to your theme/plugin and change the paths in the CSS.

= I don't want my client seeing the Post Type Icons page in the admin, can I remove it? =

Yes. Add `add_filter( 'pti_plugin_show_admin_menu', '__return_false' );` in your theme/plugin.


== Screenshots ==

1. An example of a couple of icons next to the "Post" icon in a normal state
2. An example of a couple of icons next to the "Post" icon in a hover/active state


== Changelog ==

= 0.2.2 =

* Fixing issue with multiple post types

= 0.2.1 =

* Readme update

= 0.2 =

* FontAwesome 4.0.3 update
* Fixed PHP 5.2 error

= 0.1.1 =

Removed assets from trunk
