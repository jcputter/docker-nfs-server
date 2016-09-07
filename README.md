Docker NFS Server
================

Usage
----
```bash
docker run -d --name nfs --privileged cpuguy83/nfs-server /path/to/share /path/to/share2 /path/to/shareN
```

```bash
docker run -d --name nfs-client --privileged --link nfs:nfs cpuguy83/nfs-client /path/on/nfs/server:/path/on/client
``` 

