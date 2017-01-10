UPnPscript
===

Scripts to set and delete port mappings using upnpc, a script provided by the MiniUPnP utility (http://miniupnp.free.fr/).

Usage:

```
. ./setport LOCALPORT
```

  outputs some stuff and somewhere in there shows you the random high port your port maps to publicly.

```
. ./delport LOCALPORT
```

  deletes the port mapping and outputs a bunch more unpnc status stuff.

notes
=
the reason I use . ./ in front of the command is to focre execution to set a session variable that stores the random remote port that was mapped. This allows the delport script to issue the upnpc call with that port number to delete the mapping. This way you only need to remember the local port number. I guess that's worth something, right?
