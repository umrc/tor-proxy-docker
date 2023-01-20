a simple dockerfile and compose file to connect other containert to tor network
note: alpine version may not resolve v3 onion addresses due outdated tor version in the repo

## test:

without proxy

```curl https://check.torproject.org/api/ip```

with proxy

```curl --socks5 127.0.0.1:9050 https://check.torproject.org/api/ip```
