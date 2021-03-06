# Conditional URL Advertisements

Plugin for [YOURLS](http://yourls.org). 

## Description
This plugin allows you to redirect all shortlinks through a link monetizer. 

Currently, the following shorteners are supported:
  * [AdFly](https://adf.ly/?id=2777408), trigger: `a/`
  * [AdFoc.us](https://adfoc.us/?refid=287608), trigger `f/`
  * [ouo.io](https://ouo.io/ref/0IqYvHOo), trigger `o/`

Going to a shorturl with a trigger before it will automatically forward the url through the selected service (ex *sho.rt/a/test*). If it recognizes a trigger but there is no associated service it will not monetize the link.

If you have another sevice you want supported, make a ticket for it!

## Installation
1. Clone this repo to the `/user/plugins` plugins directory
2. Edit the plugin's settings (inside *plugin.php*) to suit your needs
3. Go to the Plugins administration page and activate the plugin
4. Test your shortlinks with each activated service
5. If everything works, celebrate!

## Getting your IDs
To properly setup this plugin, you need to manually change the IDs from the defaults to your's. These instructions should show you how to do this for each service:

### AdFly
1. Ensure you have a valid account and are logged in
2. Navigate to [this url](https://adf.ly/publisher/tools#tools-api)
3. Your ID is the number after 'Your User ID:' *not API key*

### AdFocus
1. Ensure you have a valid account and are logged in
2. Navigate to [this url](http://adfoc.us/tools/site-links)
3. Your ID is the number after '?id='

### ouo.io
1. Ensure you have a valid account and are logged in
2. Navigate to [this url](https://ouo.io/manage/tools/full-page-script)
3. Your ID is the bit inside the quotes for `ouo_token`

