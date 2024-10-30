=== Kannada Comment ===
Contributors: prasannasp
Donate link: http://www.prasannasp.net/
License: GPLv3
License URI: http://www.gnu.org/copyleft/gpl.html
Tags: kannada, comment, language, unicode, google transliteration, india
Requires at least: 3.5
Tested up to: 3.6
Stable tag: 2.2

Let your fellow blog readers to write their comments in Kannada language.

== Description ==

This plugin enables Google Transliteration in wordpress comment form. So your blog readers can leave comments in Kannada script without the need of any other input engines. This is a great step to encourage people to write comments in Kannada language in your Kannada blog. This plugin adds a transliteration controller at the top of comment form. You can change the place of Transliteration controller in plugin options page. Users can click on the transliterate switch or press **Ctrl+G** to toggle between English and Kannada input languages. Site admins can change default input language in WordPress Settings > Kannada Comment. You can see the live action of this plugin at [vedasudhe.com](http://www.vedasudhe.com).

**Get in touch:**

* Visit [developer's blog](http://www.prasannasp.net/) for news and updates.
* Follow my [GitHub repositories](http://github.com/prasannasp) for codes and goodies.
* Follow me on [twitter!](http://twitter.com/prasannasp).

== Screenshots ==

1. Transliterate control switch.
2. Writing comments in Kannada language when Transliteration is enabled.
3. Kannada Comment options page

== Installation ==

1. Upload the `kannada-comment` folder to the `/wp-content/plugins/` directory
2. Activate the Kannada Comment plugin through the 'Plugins' menu in WordPress
3. Default input language will be Kannada. You can change default language on WP-Admin > Settings > Kannada Comment
4. Transliterate controller will be automatically added at the top of wordpress comment form. You can change it's place in plugin options

== Frequently Asked Questions ==

= How to change the default language? =

Go to plugin options (WP-Admin --> Settings --> Kannada Comment) and set the default language to Kannada or English.

= Does this plugin work with Facebook comment, disqus or any other commenting systems? =

No, it works with default Wordpress commenting system only. Facebook comment, disqus or any other commenting systems are not supported in this plugin.

= Will this plugin affect Name, Email and Website fields in Wordpress comment form? =

No, Transliteration is enabled only for comment form `textarea` only. So, it will not transliterate input text in the above fields.

= How to change the position of Transliterate control switch? =

I've added an option to change the place Transliteration Controller in version 2.0. You can change it's position in plugin options page. You can move it to,

* Before comment form
* Top of the comment form, before name and email fields
* Within comment form, after comment text area
* After the comment form

Default is **Top of the comment form, before name and email fields**

== Other Notes ==

= How can I get help? =

Contact the developer using his [contact form](http://www.prasannasp.net/contact/) for help and support. Also, please leave him a message if you are interested in co-development of this plugin.

= How to style the Transliterate controller? =

**Transliterate control switch** is wrapped with **kncomment** div ID and description with **kncomment-text** class. Use them in your theme to style the controller.

= Compatibility with themes =
This plugin is tested and works well with default [Twenty Eleven](http://wordpress.org/extend/themes/twentyeleven) theme, [Twenty Ten](http://wordpress.org/extend/themes/twentyten) and [Graphene](http://wordpress.org/extend/themes/graphene) themes. It will and should work with other themes as well. If you have any compatibility issues with the other themes, please leave the developer a message with all the information you have. 

== Changelog ==

= 2.2 =
* Code optimizations. www.google.com/jsapi and kncm.js are now properly enqueued only on single posts/pages if the comments are opened.
* Moved inline JavaScript to kncm.js
* Using switch() instead of if .. elseif ... else .. to show transliteration controller

= 2.1 =
* Bug fixes
* The options stored in the database will be retained even after deactivating the plugin. This is to prevent the removal of plugin options upon plugin update/reactivation. If you want to clear the database entries upon plugin deactivation, select **Restore defaults upon plugin deactivation/reactivation** in plugin options.

= 2.0 =
* Added option to change the position of Transliteration Controller
* Added option to change the title of Transliteration Controller. You can now tell your blog readers how to use transliteration in Kannada script!

For devs,

Removed `var Text_Area=document.getElementsByTagName("textarea")[0].id;`. will be just using `var ids = ["comment"];` to enable transliteration on comment form. Hope it doesn't break on hard coded comment form!.

= 1.1 =
* Added an option to set default language.
If user has selected no default language, Kannada will be set as default language upon activation.

= 1.0 =

* Initial public release.

== Upgrade Notice ==
This version requires WordPress version 3.5 or newer. If you're using an older version of WordPress, it is better to stick with Kannada Comment 2.1.
