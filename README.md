# device-proxy
Provides control over the proxies the system might use to connect to the internet..

This appliance does the following:

- All parameters passed to the device commands are syntax checked and canonicalised,
  with bash completion.
- Allows specification of an HTTP proxy to be used with services that require it..

## before

- Deploy the device-proxy-http package.

```
[root@server ~]# dnf install device-proxy-http
```

## set proxy

To set the proxy on the machine, run this. If unspecified, the port defaults to 3128.

```
[root@server ~]# device system proxy http set name=proxy.example.com
```


