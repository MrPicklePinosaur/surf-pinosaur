## surf - simple webkit-based browser
pinosaur's patched version surf from suckless.

The following patches are applied:
- [bookmarking](https://surf.suckless.org/patches/bookmarking/)
- [homepage](https://surf.suckless.org/patches/homepage/)
- [search engine](https://surf.suckless.org/patches/searchengines/)
- [playexternal](https://surf.suckless.org/patches/playexternal/)

### Requirements
In order to build surf you need GTK+ and Webkit/GTK+ header files.

In order to use the functionality of the url-bar, also install dmenu[0].

### Installation

Edit config.mk to match your local setup (surf is installed into
the /usr/local namespace by default).

Then run the following:
```
make && sudo make clean install
```

### Running surf in tabbed
For running surf in tabbed there is a script included in the distribution,
which is run like this:
```
surf-open.sh [URI]
```

Further invocations of the script will run surf with the specified URI in this
instance of tabbed.
