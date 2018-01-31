grongor/knock
=============

Simple utility for port knocking written in python3.

If you find it useful but you think it lacks some functionality please let me know by creating an issue. Thank you!

Basic usage
-----------

`knock your.server.com 1234 8521 4785`

Options
-------

`knock --help` will tell you everything you need. Here is the output to save you a few seconds:

```
usage: knock [-h] [-t TIMEOUT] [-d DELAY] [-u]
             host port[:protocol] [port[:protocol] ...]

Simple port-knocking client written in python3. See more at
https://github.com/grongor/knock

positional arguments:
  host                  Hostname or IP address of the host to knock on.
                        Supports IPv6.
  port[:protocol]       Port(s) to knock on, protocol (tcp, udp) is optional.

optional arguments:
  -h, --help            show this help message and exit
  -t TIMEOUT, --timeout TIMEOUT
                        How many milliseconds to wait on hanging connection.
                        Default is 200 ms.
  -d DELAY, --delay DELAY
                        How many milliseconds to wait between each knock.
                        Default is 200 ms.
  -u, --udp             Use UDP instead of TCP by default.
```
