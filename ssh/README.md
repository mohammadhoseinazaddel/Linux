
##### copy it in file and when you cal taht name just  type number of server you want

```bash
#!/bin/bash
if [[ -z $2 ]]
then
        echo '' > /home/ssoheilmhd/.ssh/known_hosts
        ssh -o StrictHostKeyChecking=no  root@172.20.12.$1 -p 2242
fi
```

```bash 
scp -P 2242 root@172.20.12.111:/var/log/sab-ui.log  Desktop
```
