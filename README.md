See [netdata](https://github.com/firehol/netdata) for more general information.


```
docker run -d --cap-add SYS_PTRACE \
           -v /proc:/host/proc:ro \
           -v /sys:/host/sys:ro \
           -p 19999:19999 positionly/netdata
```

You can optionally mount configuration file via `-v /your/netdata.conf:/etc/netdata/netdata.conf`
