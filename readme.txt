=== Better Anchor Links ===
Contributors: Luděk Melichar
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=48CZMVXER28PE&lc=CZ&item_name=Plugin%20development&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted
Tags: anchor links, content links, content, sidebar, links, widget, better
Requires at least: 3.0
Tested up to: 3.1.4
anchor links, bal, lm-bal
Stable tag: 1.2

Creates anchor links to heading tags in the content and displays automatically at the top of the content, or allows for custom placement with tags.

== Description ==

Creates anchor links to heading tags in the content and displays them automatically at the top of the content, or allows for custom placement with tags or sidebar widget.

Features:

* Has option to auto display anchor links to Heading tags in content.
* Allows control of which content to auto display links.
* Can disable plugin css to allow custom styles to be applied.
* Has widget available for display
* Insert custom title to display above links
* Clears all traces from any excerpts displayed

== Installation ==

1. Upload to your Wordpress plugins folder.
2. Activate in Wordpress admin area.
3. Update options under "Settings->B. Anchor Links"

== Frequently Asked Questions ==
= How Do I Place In Custom Locations? =

In Content
1. Using the visual editor
   Add the tag [mwm-aal-display] into your individual content using the visual editor.
2. PHP Template Tag(must be below the_content())
   `<?php global $mwm_aal; echo $mwm_aal->output_content_links(); ?>`

In Sidebar
	1. Activate Widget
		- Go to Appearance -> Widgets in Wordpress admin "Better Anchor Links".
	2. PHP Template Tag
		`<?php global $mwm_aal; $mwm_aal->output_sidebar_links(); ?>`
		
= How Do I Add Custom Styles? =
	The content display and side bar are wrapped with a <div> with an assigned css class. You can put the classes into your own style sheet and use further declarations to target elements within the div.
	
	For Content:(uses <ol>,Does not use an H tag for title)
		.mwm-aal-container{}
		.mwm-aal-container-title{}
		
	For Sidebar: (uses <ul>, traditional h2 tag for title)
		mwm-aal-sidebar-container{}

== Screenshots ==
1. Admin options
2. Display in default wordpress template

== Changelog ==
= 1.2 =
* fixed widget issue

= 1.1 =
* Program rename
* Fixed dysfunctional save options.
* Default changed for H1 and H2 only

= 1.0 =
* Fork of Auto Anchor Links.

== Upgrade Notice ==
= 1.1 =
* For upgrade from Auto Anchor Links 1.0 uninstall old AAL and remove addon. Install Better Anchor Links 1.1. If you used manual tags to contents, they are compatible.
