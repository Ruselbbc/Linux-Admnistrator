# Mdadm home work

Copy all files on your machine

1. vagrant up
2. copy mdadm.conf to /etc/mdadm/mdadm.conf
3. restart VM

   OR use this command to setup this raid

   1.vagrant up
   2.copy raid_up.sh to home directory
   3.sudo sh raid_up.sh                  #Run this script
                       or
                            chmod +x
                            raid_up.sh && ./raid_up.sh
   
   commands in this sh script:
   mdadm --zero-superblock --force /dev/sd{b,c,d,e,f,g}
   mdadm --create --verbose /dev/md0 -l 10 -n 5 /dev/sd{b,c,d,e,f,g}
