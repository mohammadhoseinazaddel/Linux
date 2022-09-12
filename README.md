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
free -th
```

```
grep MemTotal /proc/meminfo
```
```
sudo dmidecode --type 17 | more
```
#### disk size
```
df
```
```df -T``` shows the disk usage along with each block's filesystem type (e.g., xfs, ext2, ext3, btrfs, etc.)

```fdisk -l``` shows disk size along with disk partitioning information
#### file size in disk
```du``` shows the disk usage of files, folders, etc. in the default kilobyte size

```du -h``` shows disk usage in human-readable format for all directories and subdirectories

```du -a``` shows disk usage for all files

```du -s``` provides total disk space used by a particular file or directory
