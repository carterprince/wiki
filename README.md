# wiki

"I'm feeling lucky"-type search for MediaWiki-based sites such as Wikipedia.

## Usage

```bash
wiki [query]
```

This will open the closest match for `[query]` on Wikipedia in your browser. It will use `$BROWSER` if it is set, and `xdg-open` otherwise.

You can also pass the `--site` argument to specify a different site. For example, to search on RationalWiki, you can specify the `rationalwiki.org` domain:

```bash
wiki --site rationalwiki.org [query]
```

You can read from `/dev/stdin` using `-i`. If you pass `-rofi`, it will prompt the user for a query using [`rofi`](https://github.com/davatorium/rofi).