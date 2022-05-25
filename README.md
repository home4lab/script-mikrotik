# script-mikrotik

step by step logic

 1. master device will push backup file to backup device with automatic [master scheduler](https://github.com/home4lab/script-mikrotik/blob/main/master-system-scheduler)
 2. backup device will toggle disable and enable netwatch with [backup scheduler](https://github.com/home4lab/script-mikrotik/blob/main/backup-system-scheduler)
 3. backup device will check every 10 second if master available or not with [backup netwatch](https://github.com/home4lab/script-mikrotik/blob/main/backup-tool-netwatch)
 4. once master device goes down, backup device will restore that file configuration already backed up before

