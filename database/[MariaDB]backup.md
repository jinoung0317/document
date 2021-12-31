### Database backup
### date : 2021-12-26

---

### mariabackup 전체백업
```shell
    > mariabackup --backup --user=USER_NAME --password=PASSWORD --target-dir=DIR_PATH
```
 - \-\-bcakup : 묶음을 해제
 - \-\-no\-lock : 묶음을 묶음
 - \-\-host : database connect host 
 - \-\-port : database connect port
 - \-\-user : database connect user name
 - \-\-password : database connect user password
 - \-\-target\-dir : backup file path


### mariabackup 전체복원
```shell
    > mariabackup --copy-back --target-dir=DIR_PATH
```

[REPO]

 1. [mariabackup 사용법](http://www.linuxdata.org/bbs/board.php?bo_table=DB&wr_id=24)

 2. [Mariabackup을 이용한 증분 백업](https://velog.io/@tkfrn4799/mariadb-mariabackup)