=== Website Screenshots ===
Contributors: dirk94
Tags: screenshot, website screenshot, generator, tool, automatic, shortcode, automate, screenshots, shots, web browser, window, snap, website, website screenshot, website preview
Requires at least: 4.0
Tested up to: 5.5
Stable tag: 1.0.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Automatically create website screenshots

== Description ==

Use the `[website-screenshot]` shortcode to automatically insert an up to date webiste screenshot.

= Shortcode Examples =

`// Website screenshot of wordpress.org
[website-screenshot url="https://wordpress.org" width="1680"]

// You can also resize the generated images
[website-screenshot url="https://wordpress.org" width="1680" thumbnail_width="100"]

// And you can add custom html tags
[website-screenshot url="https://wordpress.org" target="_blank" class="my-image-class"]`

= Parameters =

* url (required) - The url
* width - the width of the screenhsot
* height - the height of the screenshot
* thumbnail_width - Resize the image to the desired width, preserves the aspect ratio
* alt - the image alt text
* target - browser target. For example: use _blank to open in a new window
* class - add a class to the screenshot

= Generating the screenshot in PHP =

You can also use our PHP class to generate a screenshot:

`<img src="<?php echo WebsiteScreenshot::screenshot(['url' => 'https://wordpress.org']); ?>" />`

= Notes =

* This plugin relies on [screenshotapi.net](https://screenshotapi.net) you should create an account there and paste your API token into the settings page.

== Installation ==

1. Install the plugin from the Wordpress admin panel, or upload the `website-screenshots` folder to `/wp-content/plugins/`
2. Activate the plugin through the 'Plugins' menu in WordPress

== Changelog ==

= 1.0.1 - 20 August 2020 =
* Updated the readme.

= 1.0.0 - 19 August 2020 =
* The initial release.
