=== Encrypt Email ===
Contributors: LukeQuietus, Affinity4
Donate link: http://luke-watts.com/doesnt-want-donations
Tags: email, spam protection, encrypt, encryption, email encryption, encrypt email, encoder, encode email, email cypher, cypher
Requires at least: 3.0
Tested up to: 4.7.9
Stable tag: 3.2.1
 
This plugin allows users to encrypt emails in their content and widgets using a simple shortcode. The encryption uses a native Wordpress function antispambot().
 
== Description ==
 
This plugin allows users to encrypt emails in their content and widgets using a simple shortcode. The encryption uses a native Wordpress function antispambot().
 
To encrypt your email simply use the shortcode:

`[encrypt_email email="your@email-here.com" text="Text displayed"]`

or since v1.1.0 you can wrap your email in the shortcode using:

`[encrypted_email]your@email-here.com[/encrypted_email]`

If you want to display specific text use:

`[encrypted_email text="Text to be displayed goes here"]your@email-here.com[/encrypted_email]`

Since 2.0 you can use the 'Encrypt Email' button on the Visual Editor tab to wrap your selected email.

Since 2.1 a lock icon is displayed beside sucessfully encrypted emails, viewable only for logged in users.
 
= Future Features =
* Popup with text fields to insert email and display text for shortcode.
* Options panel with configuration options, including ability to pre-configure shortcode for one-click insertion of admin email and additional types of encryption including ASCII (SINGLE ENCRYPTION), ASCII (DUAL ENCRYPTION), DECHEX, WORDPRESS and RANDOM
 
= Want to contribute? =
* Fork the project on [Github](https://github.com/lukewatts/encrypt-email)
* Contact me through my website at [Luke Watts](http://luke-watts.com)
 
== Installation ==
 
1. Upload the entire `encrypt-email` folder to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Select your email in Visual Editor tab. 
4. Click "Encrypt Email" to wrap it in the [encrypted_email] shortcode and be spam free*

 *Of course there's no way for me 100% gaurantee you'll be spam free but this will certainly make it harder for email harvesters
 and spambots than doing nothing!
 
== Frequently Asked Questions ==
 
= Does this plugin work with the newest WordPress version and also older versions? =
Yes, this plugin works with WordPress 3 upwards!
 
= Will this work in my theme's widget areas? =
As long as the theme has enabled shortcodes in your sidebar / widgets then this method will work. However, if the widget is already inserting the <a href="mailto: "></a> link then this shortcode won't work in such fields. You'll notice upon saving the widget then it removes everything after the first " sign.
 
== Screenshots ==
 
No screenshots available at this time.
 
== Changelog ==

= 3.2.0 =
* Formatting code. Removing PHP 5.3+ array syntax from Shortcodes class

= 3.1.0 =
* MAJOR BUG FIX: Fixed issue where files in subfolders where not loading

= 3.0.0 =
* Added EncryptEmailShortcodes Class to handle creating shortcodes
* Added EncryptEmailAsset Class to handle loading scripts and styles
* Added EncryptEmailQuickTag Class to handle creating quicktag buttons
* Moved encrypt-email.css into assets/css directory
* Added QuickTag button for HTML editor

= 2.1.0 =
* Added icon to display beside sucessfully encrypted emails. ( Viewable only for logged in users )

= 2.0.0 =
* Added TinyMCE button which will allow you to simply select your email and click "Encrypt Email" to wrap it in the [encrypted_email] shortcode.

= 1.1.0 =
* Tested compatibility for WordPress 4.0
* Added shortcode [encrypted_email] which allows you to wrap emails in your content to encrypt them.

= 1.0.0 =
* Initial release
 
== Upgrade Notice ==

= 1.1 =
* Tested compatibility for WordPress 4.0
* Added shortcode [encrypted_email] which allows you to wrap emails in your content to encrypt them.

= 1.0 =
* Initial release
