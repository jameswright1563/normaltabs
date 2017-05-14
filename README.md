# Normal Tab Size

Chrome extension with a user stylesheet that applies a single rule to the root element:

```css
html {
  tab-size: 2;
}
```

This fixes the default [`tab-size`][tab-size] value being 8, which is too large for most types of code.

## Security

A global user stylesheet requires global content permissions, so it's a good security practice to avoid extension like this unless they're from reputable vendors. Possible workarounds are:

 * Making your own extension (like I've done here), but hosting it in the Chrome Web Store requires a developer account
 * Loading an unpacked extension after enabling *Developer mode* in `about:extensions`, but this will cause Chrome to nag about it on startup

## Configuration

It's a static stylesheet, so there's no configuration, and hopefully also no impact on performance.

## Installation

Install the extension from [Chrome Web Store][web-store] or load it [unpacked][load-unpacked].

## License

MIT

[web-store]: https://chrome.google.com/webstore/detail/normal-tab-size/kjjblpbmpgkbfnonlanolpcmlolafamn
[tab-size]: https://developer.mozilla.org/en-US/docs/Web/CSS/tab-size
[load-unpacked]: https://developer.chrome.com/extensions/getstarted#unpacked
