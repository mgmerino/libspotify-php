Higly experimental libspotify PHP lib

For a lot of reasons the function names is not the same and does not work the same as the c-lib. Don't whine about it.

As this is higly experimental you should make note of a few things:
- The api might (and will) change.
- Don't whine if stuff crashes (because it will), fix it instead.

Installation:
# add appkey.c (fetch your key from developer.spotify.com; this will improve in the future)
phpize
make && make install

Usage:
spotify_init("user", "pass");
$starred_playlist = spotify_get_starred_playlist();
spotify_destroy();
