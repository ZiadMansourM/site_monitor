# site_monitor
This is a Simple lightweight Script to monitor a website uptime.

# Features:
- [X] Uptime
- [ ] CPU Usage
- [ ] RAM Usage
- [ ] Drive Usage


# CPU Usage
```shell
# CPU USAGE:
echo $[100-$(vmstat 1 2|tail -1|awk '{print $15}')]
```


# RAM Usage
```shell
# MEMORY USAGE:
free | grep Mem | awk '{print $3/$2 * 100.0}'
```
