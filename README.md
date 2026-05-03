В каталожике */usr/local/bin* размещены сценарии резервирования сопровождаемого общего программного обеспечения:
- */etc*, */opt/luxmsbi/conf*, */opt/luxmsbi/web*, */var/lib/pgpro/std-15/data*.

Периодичность (средствами cron) - каждый четверг каждого месяца в 10:00.

В каталожике */usr/local/sbin* размещены сценарии резервирования БД *mi*.

Периодичность (средствами cron) - ежедневно в 03:10.

Синтаксис cron:
```copy
# m     h       dom     mon     dow      command
10      03      *       *       *        /bin/nice -n 20 /usr/local/sbin/backup.run
00      10      *       *       4        /bin/nice -n 20 /usr/local/bin/backup.run
```

## Add your files

- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
- [ ] [Add files using the command line](https://docs.gitlab.com/topics/git/add_files/#add-files-to-a-git-repository) or push an existing Git repository with the following command:

```
cd existing_repo
git remote add origin git@github.com:tserkowny/backup_db_opo.git
git branch -M main
git push -uf origin main
```
