# Multiple MySQL databases backup for Docker [![](https://images.microbadger.com/badges/image/thedrhax/mysql-backup.svg)](https://hub.docker.com/r/thedrhax/mysql-backup)

This lightweight (alpine-based) image can:

* Make backup of multiple MySQL databases
* Compress each `.sql` dump with GunZIP using `pigz`
* Store previous dumps for a $RETENTION_PERIOD

## Environment variables (with default values)

* `PROFILES="USER:PASS@HOST:PORT USER@HOST/DATABASE ..."` (required)
* `RETENTION_PERIOD=7`
* `MYSQLDUMP_OPTIONS="--lock-tables"`

