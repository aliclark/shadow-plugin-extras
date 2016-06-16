"quux": a Shadow plug-in
=========================

This plug-in provides a quick example of how to interface with Shadow.
The most important features of the code that enable this are:
 + no process forking
 + no busy loops

copyright holders
-----------------

No copyright is claimed by the United States Government.

licensing deviations
--------------------

No deviations from LICENSE.

last known working version
--------------------------

This plug-in was last tested and known to work with `Shadow v1.11.1-11-gf349fe5 2016-03-11`

usage
-----

Please see the `example.xml`, which may be run in Shadow

```bash
shadow example.xml
```

After running the above, check the following directories for process output:

  + `shadow.data/hosts/quuxclient/stdout-quux-1000.log`
  + `shadow.data/hosts/quuxserver/stdout-quux-1000.log`

A binary version of the code is available for usage outside of Shadow.
Run the program `quux` with no arguments to start the server:

```bash
quux
```

Run the program `quux` with the IP address or hostname of the listening
server to run client mode:

```bash
quux localhost
```
