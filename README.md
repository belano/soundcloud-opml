A simple python script for generating an opml file from a list of soundcloud sets which 
can be imported from logitech media server (ie. squeezebox server).

## System requirements
* Python 3

## Setup
1. Install soundcloud client `pip install soundcloud`
2. Setup your client id, path and playlists in `$HOME/.config/soundcloud-opml/scopml.cfg`
```
[scopml]
api_key = your_client_id
path    = /tmp

[playlists]
sesiones-nanosonico = https://soundcloud.com/nanosonicoradio/sets/sesiones-musicales
brand-new-wayo      = https://soundcloud.com/abelano/sets/brand-new-wayo
...
```

## Running the script
```
soundcloud-opml.py [-h] [-k KEY] [-p PATH]

optional arguments:
  -h, --help            show this help message and exit
  -k KEY, --key KEY     soundcloud client id
  -p PATH, --path PATH  use a custom path this time
```

Will generate an opml file under specified path.


