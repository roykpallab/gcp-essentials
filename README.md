# gcp-essentials


### Prepare a data disk 
```
sudo mkdir -p /home/minecraft
```
- create Mount point 



```
sudo mkfs.ext4 -F -E lazy_itable_init=0,\
lazy_journal_init=0,discard \
/dev/disk/by-id/google-minecraft-disk

```

- To mount the disk, run the following command

```
sudo mount -o discard,defaults /dev/disk/by-id/google-minecraft-disk /home/minecraft

```
