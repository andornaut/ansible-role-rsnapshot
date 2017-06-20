# ansible-role-rsnapshot

## Example configuration

```
backup_directory: /var/backups/rsnapshot/
backup_hosts:
  - name: example.com
    user: root
    directories:
      - /etc/
      - /var/docker-volumes/
    scripts:
      - command: /usr/local/bin/backupdockerpostgresql
        args: --host root@example.com --container postgresql postgresql.gz
```

