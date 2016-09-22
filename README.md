# Snap of InfluxDB

This repo allows you to create a snap of
[InfluxDB](https://github.com/influxdata/influxdb).

On an Ubuntu system, simply run:

    $ git clone https://github.com/dholbach/influxdb-snap.git
    $ cd influxdb-snap
    $ snapcraft

and install the resulting snap.


## Caveats

You currently need to install it with `--devmode`, because it stores its
database in `/root/.influxdb/meta/meta.db`, shipping a custom config which
uses `$SNAP_USER_DATA` should probably not be too hard.
