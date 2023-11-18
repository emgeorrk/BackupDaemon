# BackupDaemon
### Installation
1. Fill in the `config.yaml` as follows:
```yaml
sourceDirectory: /home/user/mydir
backupDirectory: /home/user/mydir_backups
frequency: minutely/hourly/daily/monthly   # choose one
```
2. Run `create_service.sh` script:
```command
sudo sh create_service.sh
```
### Usage
```bash
systemctl status backupdaemon   # check the daemon's status
systemctl [start/stop] backupdaemon   # start/stop the daemon
systemctl [enable/disable] backupdaemon   # enable/disable launch the daemon on system startup
systemctl reload backupdaemon   # reload the daemon's configuration
```
