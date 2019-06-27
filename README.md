# mtaserverlist-python
Python parser for inspecting the MTA:SA serverlist

# Usage

```py
import MTAServerlist
import urllib.request, urllib.parse, urllib.error

svr = MTAServerlist.MTAServerlist()
svr.parse(urllib.request.urlopen("https://master.multitheftauto.com/ase/mta/").read())
print(svr.servers)
```
