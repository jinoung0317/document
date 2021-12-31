### Docker mariaDB container setting
### date : 2021-12-26

---

### mariadb 추가 기능 설정
 사유 : volumnes 설정 오류로 인로 보완 작업
 
 1. apt 업데이트
 2. openssh-server 설치
 3. crontab 설치
 
 1. apt 업데이트
 ```sql
  > dpkg --configure -a
  > apt update -y
 ```

 2. openssh-server 설치
 ```sql
  > apt install openssh-server -y
  > service ssh start
 ```

 3. crontab 설치
 ```sql
  > apt install cron
 ```
 
 
 
[REPO]
 
 1. [crontab 명령어 관련](https://rudi2e.com/28)


 