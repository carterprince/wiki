# wiki

"I'm feeling lucky"-type search for MediaWiki-based sites such as Wikipedia.

## Usage

```bash
wiki [query]
```

This will open the closest match for `[query]` on Wikipedia in your browser. It will use the `$BROWSER` environment variable if it is set, and `xdg-open` otherwise.

You can also pass the `--site` argument to specify a different site. For example, to search on [RationalWiki](https://rationalwiki.org/wiki/Main_Page), you can specify the `rationalwiki.org` domain:

```bash
wiki --site rationalwiki.org [query]
```

You can read from `/dev/stdin` using `-i`. If you pass `-rofi`, it will prompt the user for a query using [`rofi`](https://github.com/davatorium/rofi).

## Installation

Clone this repository with `git clone https://github.com/SoopaKhell/wiki`.

Change directories into the cloned repo, and move `wiki` into `/usr/local/bin`:

```bash
cd wiki
sudo mv wiki /usr/local/bin
```

## Requirements

* [pup](https://github.com/ericchiang/pup) (`yay -S pup-git`)
* [curl](https://github.com/curl/curl) (`sudo pacman -S curl`)

# License

This software is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/quick-guide-gplv3.html).