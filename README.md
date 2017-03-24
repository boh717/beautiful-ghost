# Beautiful Ghost - A port of Beautiful Jekyll theme

This is a porting of [Beautiful Jekyll](http://deanattali.com/beautiful-jekyll/) theme by [Dean Attali](http://deanattali.com/aboutme#contact). It supports most of the features of the original theme.

Too see a live preview, just visit my [blog](https://runningcodes.net/)!

## TODO

- Tag support
- Comments count disqus
- Author pages (?)

## Installation

In your ghost directory:

```
    $ cd content/themes
    $ git clone https://github.com/boh717/beautiful-ghost.git beautifulghost
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

## License

MIT Licensed, see [LICENSE](https://github.com/boh717/beautiful-ghost/blob/master/LICENSE).
