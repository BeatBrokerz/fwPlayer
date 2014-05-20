Flex Widget: Standalone Player
=============

This is a standalone embedded music player for the flex framework. It has display formats for a range of different sizes, and it includes built in access to the full current playlist, licensing options, and shopping cart as well as all the standard song controls.

### Pre-requisites

This widget requires a flex app to be installed to your webpage in order for it to work. Refer to the [flex installation guide](http://www.beatbrokerz.com/flex/start) for more information on how to set up your own app.

Once you have a flex app configured for your page, follow these steps to use this widget:

1. Download the widget package [.zip file](https://github.com/beatbrokerz/flex-fwplayer/archive/master.zip)
2. Extract the contents and upload the files/folders to a public location on your webserver.
3. Add a script tag on your webpage to link to the "widget.js" file you just uploaded to your server.
4. Also add a reference to the "widget.css" stylesheet you just uploaded to your webpage.
 
> **Example:** 
> ```html
> <script type="text/javascript" src="/path/to/fwplayer/widget.js"></script>
> <link rel="stylesheet" type="text/css" href="/path/to/fwplayer/widget.css" />
> ```

### Autoloading Support

This widget can also be loaded using the [widget autoloader](http://www.beatbrokerz.com/flex/start/settings#autoloader) feature in your flex app settings. To autoload this widget, just enter the full url to your uploaded widget.js script into the autoloader section of your flex store configuration page. When autoloading this widget, all of its other resources (such as the css file) will automatically be added to your page for you.

### Widget Settings

The widget supports the following settings:

1. **width**: Optional. An integer value that defines the width of the widget when its rendered
2. **height**: Optional. An integer value that defines the height of the widget when its rendered
3. **cart**: Optional. A string value ('top', 'bottom', or 'off') which controls where the cart shows. Default: 'bottom'
4. **theme**: Optional. A string value which allows you to define a custom [theme prefix](http://www.beatbrokerz.com/flex/widgets/theming) for the widget
 
### Usage Instructions

Add the widget inline with your content using any of the standard [widget display methods](http://www.beatbrokerz.com/flex/widgets#display-methods). 

> **Example:** 
> ```html
> <div data-bbflex="widget:fwplayer,width:620,height:150"></div>
> ```
