# CanhazIP.com DDclient support
This patch adds support to DDclient for canhazip.com


### Step 1. install DDclient (I'll let you figure that out)

### Step 2. locate DDclient (Ubuntu = /usr/sbin/ddclient):
```
# which ddclient
/usr/sbin/ddclient
```

### Step 3. make a backup copy of the config file:
```
$ cp /usr/sbin/ddclient /usr/sbin/ddclient.orig
```

### Step 4. patch the DDclient config file:
```
$ patch /usr/sbin/ddclient < canhazip.patch
patching file ddclient
```

### Step 5. that's it -- use DDclient, or add CloudFlare support also: [CloudFlare DDclient patch](http://blog.peter-r.co.uk/cloudflare-ddclient-patch.html)
