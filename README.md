# Beautiful Ghost - A port of Beautiful Jekyll theme

This is a porting of [Beautiful Jekyll](http://deanattali.com/beautiful-jekyll/) theme by [Dean Attali](http://deanattali.com/aboutme#contact). It supports most of the features of the original theme.

Too see a live preview, just visit my [blog](https://runningcodes.net/)!

From version 1.1, beautiful-ghost will support only Ghost >= 1.0. It will work also on older versions, but some feature may be disabled (e.g., favicon).

## TODO

- Comments count disqus

## Installation

Easy way:

Head to the [releases page](https://github.com/boh717/beautiful-ghost/releases) and grab the last version. Then in your ghost installation go in Settings/Design and click on `Upload a theme`. You're done! :tada:

If you want to customize some parts, great! Clone the repository, make your modifications and recreate the zip file:

```
    $ git clone https://github.com/boh717/beautiful-ghost.git
    // Your modifications
    // Then move in theme root level
    $ cd beautiful-ghost
    $ zip -r beautiful-ghost.zip *
    // Upload the theme zip as before
 ```

## Features

### Responsive

This theme is designed for both large-screen and small-screen (mobile) devices.

### Syntax highlighting

This theme has support for syntax highlighting thanks to the PrismJS library.


### Disqus support

To use this feature, change `{{!> disqus}}` into `{{> disqus}}` in `post.hbs` and fill out the `disqus_shortname` parameter in `partials/disqus.hbs`.

### Google Analytics

To add Google Analytics, simply sign up to [Google Analytics](http://www.google.com/analytics/) to obtain your Google Tracking ID, add this tracking ID to `partials/google-analytics.hbs` and change `{{!> google-analytics}}` into `{{> google-analytics}}` in `partials/footer.hbs`.

### No header image in posts (but yes in social networks)

In `header_post_page.hbs` you will find a switch:

```
{{> header_image}}
{{!> no_header_image}}
```

The first one (`{{> header_image}}`) is the default: if you upload a post image it will be shown in post page AND on social networks when you share it; if you don't upload an image, then it won't show anywhere. Easy peasy.

The second option (`{{!> no_header_image}}`) is a little bit different: you will never see the uploaded post image on your blog, but if you share it, then the image will display, giving better visibility to your tweet/FB post.

The two options are mutually exclusive, only one at a time must be activated.

## License

MIT Licensed, see [LICENSE](https://github.com/boh717/beautiful-ghost/blob/master/LICENSE).
