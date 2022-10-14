# fetch-replici.net

Get the latest 10 episodes of every show from Radio România Actualități.

It has two modes:
- one which creates HTML redirects:
```
./fetch-replici.net
```
- one which downloads the actual audio file:
```
./fetch-replici.net -a|--audio
```

If used as service, it repeats every one hour, thus achieving continuous retrieval of episodes.

Run `./install` to install as a service, it usually requires root access.

Episodes will be found in `/usr/share/replici.net/${show}`.

Version 1.0


## Dependencies

Install them yourself:
- [curl](https://curl.haxx.se) - retrieve data from servers
- [caddy](https://github.com/mholt/caddy) - serves the data on the web
- [pup](https://github.com/ericchiang/pup) - HTML parser
- [wget](https://www.gnu.org/software/wget) - retrieve data from web servers
