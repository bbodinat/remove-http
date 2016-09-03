=== Remove HTTP ===
Contributors: factmaven, ethanosullivan
Tags: protocol relative url, relative protocol, protocol rewriting, remove http, remove https, url, http, https, rewrite, cloudflare
Requires at least: 1.2.0
Tested up to: 4.6
Stable tag: 1.0.0
License: GPLv3
License URI: http://www.gnu.org/licenses/gpl-3.0.html

Automatically scan your website and removes both HTTP and HTTPS protocols from your URL links. Helps resolves the mixed content warnings.

== Description ==
**Remove HTTP** is a plugin that a automatically scans your website and removes both `http:` and `https:` protocols from your links without permanently changing anything. This helps resolve websites that are having "mixed content warnings" when your website has assets (images, JavaScript, and CSS) loading both HTTP and HTTPS.

No configuration is required. Simply install and activate Remove HTTP plugin and you will immediately see your changes. Links that had `http:` or `https:` will only have `//` making them protocol relative URLs.

= Before =
`
<link rel='stylesheet' id='some-id'  href='https://link.to/some/style.css' type='text/css' media='all' />
<script type='text/javascript' src='http://link.to/some/script.js'></script>
<a href="https://web.site" title="Fact Maven" rel="home">Some Link</a>
<img src="http://link.to/some/image.jpg" alt="Some Alt" width="150" height="50" />
`

= After =
`
<link rel='stylesheet' id='some-id'  href='//link.to/some/style.css' type='text/css' media='all' />
<script type='text/javascript' src='//link.to/some/script.js'></script>
<a href="//web.site" title="Some Title" rel="home">Some Link</a>
<img src="//link.to/some/image.jpg" alt="Some Alt" width="150" height="50" />
`

= Contribute on GitHub =
[View this plugin on GitHub](https://github.com/factmaven/remove-http)

We're always looking for suggestions to improve our plugin!

== Installation ==
1. Upload the plugin to the `/wp-content/plugins/` directory.
1. Activate the plugin through the `Plugins` menu in WordPress.
1. Let it settle in a for a minute and be amazed.

== Changelog ==
= 1.0.0 (00/00/00) =
* Initial release, huzzah!