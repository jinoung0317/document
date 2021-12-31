### Linux crontab 
### date : 2021-12-26
### tag  : \#주기, \#

---

### 로그인한 계정의 crontab list 출력
```shell
    > crontab -l
```


### crontab 수정
```shell
    > crontab -e
```


### crontab 전부삭제
```shell
    > crontab -r
```


### crontab 사용 예제
```shell
    > * * * * * SHELL_COMMAND
```

첫번째 * 0 ~ 59 : 분 

두번째 * 0 ~ 23 : 시간

세번째 * 1 ~ 31 : 일

네번째 * 1 ~ 12 : 월

다섯째 * 0 ~ 6   : 요일 ( 0 : 일요일 )


## 예제

1. 매분 실행
```shell
   * * * * * COMMAND     
```

2. 매주 금요일 오전 5시 45분에 실행
```shell
   45 5 * * 5 COMMAND     
```

3. 매일 1시 0분 부터 30까지 실행
```shell
   0-30 1 * * * COMMAND     
```

4. 매일 매시간 0분, 20분, 40분 실행
```shell
   0,20,40 * * * * COMMAND     
```

5. 매 10분마다 실행
```shell
   */10 * * * * COMMAND     
```


### crontab 백업
```shell
    > crontab -l > BACKUP_PATH&FILE_NAME
```


[REPO]
 
 1. [주기적으로 실행해야하는 프로그램](https://yoonghee.tistory.com/64)


 