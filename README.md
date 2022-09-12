# Linux
#### check linux version and distribution

```
cat /etc/*-release
```
```
cat /proc/version
```
```
uname -a
```

#### see cpu 
```
lscpu
```
#### memory
```
grep MemTotal /proc/meminfo
```
```
sudo dmidecode --type 17 | more
```
