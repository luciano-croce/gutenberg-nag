# Dismiss Gutenberg Nag
[![Build Status](https://travis-ci.org/luciano-croce/dismiss-gutenberg-nag.svg?branch=master)](https://travis-ci.org/luciano-croce/dismiss-gutenberg-nag)

Dismiss "<strong>try Gutenberg</strong>" nag, dashboard widget, when is activated, or automatically, if it is in mu-plugins directory.
* <strong>Tips</strong>: a neat trick, is to put this single file <strong>dismiss-gutenberg-nag.php</strong> (not its parent directory) in the <strong>/wp-content/mu-plugins/</strong> directory (create it if not exists) so you won’t even have to enable it, and will be loaded by default, also, since first step installation of WordPress setup!
* <strong>To date</strong>, try Gutenberg nag, preliminarily introduced in WP [4.9-beta3](https://wordpress.org/news/2017/10/wordpress-4-9-beta-3/) was already respectively removed in WP 4.9-beta4, in WP 4.9-RC1, in WP 4.9-RC2, in WP 4.9-RC3, in WP 4.9.0, in WP 4.9.1, in WP 4.9.2 and in WP 5.0-alpha, but <strong>is expected to land in core when WP 4.9.3 (4.9.3-beta1) is released</strong>, in late 2017/early 2018 according with this related [ticket](https://core.trac.wordpress.org/ticket/41316).
* <strong>Explanation</strong>: this, is <strong>different from the other similar plugins</strong>, because <strong>uses the filter hook, and not the action hook</strong>. Filters should filter information, thus receiving information/data, applying the filter and returning information/data, and then used. However, filters are still action hooks. WordPress defines add_filter/remove_filter as "hooks a function to a specific filter action", and add_action/remove_action as "hooks a function on to a specific action".
