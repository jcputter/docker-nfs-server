Docker NFS Server
================

Usage
----
```bash
docker run -d --name nfs --privileged jcputter/nfs-server /path/to/share /path/to/share2 /path/to/shareN
```

```bash
docker run -d --name nfs-client --privileged --link nfs:nfs jcputter/nfs-client /path/on/nfs/server:/path/on/client
``` 

