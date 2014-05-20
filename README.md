Flex Widget: Standalone Player
=============

![Standalone Player Preview](http://www.beatbrokerz.com/flex/widget/fwplayer/preview.png)

This is a standalone embedded music player for the flex framework. It supports a wide range of different sizes, and it includes built in access to the full current playlist, licensing options, and shopping cart as well as all the standard song controls.

* [LIVE DEMO](http://jsfiddle.net/beatbrokerz/ASL69/)

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

### Theme & Structure Reference

The rendered widget uses the following template structure and css classing.

```html
<div class="flex-player-cart-container">
  <div class="flex-player-cart-container-inner">
    <div class="cart-summary-wrap">
      <span class="cart-totals">
        <i class="fwicon-basket"></i> 0 Items: $0.00
      </span>
      <span class="cart-checkout">
        <button class="cart-checkout-button btn btn-success btn-xs">
          <span class="cart-checkout-button-text">
            <i class="fwicon-right-circled"></i> Checkout
          </span>
        </button>
      </span>
    </div>
  </div>
  <div class="cart-list-wrap">\
    <!-- Stock Cart Widget (http://www.beatbrokerz.com/flex/widgets/stock) -->
  </div>
</div>
<div class="table-row preview">
  <div class="table-cell fw-preview-area">
    <div class="fw-content-image">
      <img />
    </div>
    <div class="fw-content fw-content-nowplaying fw-outer-content reserved">
      <div class="table"><div class="table-row"><div class="table-cell">
        <div class="fw-nowplaying-producer"></div>
        <div class="fw-nowplaying-songname"></div>
        <div class="fw-nowplaying-genres"></div>
      </div></div></div>
    </div>
    <div class="fw-content-buttons">
      <div class="fw-button-tab nowplaying">
        <a class="jp-button fw-button fw-button-nowplaying active">
          <i class="fwicon-info"></i><span class="button-text"> Now Playing</span>
        </a>
      </div>
      <div class="fw-button-tab playlist">
        <a class="jp-button fw-button fw-button-playlist">
          <i class="fwicon-music"></i><span class="button-text"> Full Playlist</span>
        </a>
      </div>
      <div class="fw-button-tab buynow">
        <a class="jp-button fw-button fw-button-buynow">
          <i class="fwicon-dollar"></i><span class="button-text"> Buy Now</span>
        </a>
      </div>
    </div>
    <div class="fw-content-div fw-inner-content">
      <div class="fw-content fw-content-playlist">
        <!-- Stock Playlist Widget (http://www.beatbrokerz.com/flex/widgets/stock) -->
      </div>
      <div class="fw-content fw-content-nowplaying active">
        <div class="table"><div class="table-row"><div class="table-cell">
          <div class="fw-nowplaying-producer"></div>
          <div class="fw-nowplaying-songname"></div>
          <div class="fw-nowplaying-genres"></div>
        </div></div></div>
      </div>
      <div class="fw-content fw-content-buynow">
        <!-- Stock Licensing Widget (http://www.beatbrokerz.com/flex/widgets/stock) -->
      </div>
    </div>
  </div>
</div>
<div class="table-row controls">
  <div class="table-cell controls">
    <!-- Stock Playbar Widget (http://www.beatbrokerz.com/flex/widgets/stock) -->
  </div>
</div>
```
