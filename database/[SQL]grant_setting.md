### Database grant setting
### date : 2021-12-26

---

### DB 권한 추가
```sql
    GRANT ALL [select|insert|update|delete] ON DB명.Table명 to user명.IP[%|localhost|...] identified by 'password';
```

 - 'identified by' : 권한 등록 시, 비밀번호 변경도 진행


### DB 권한 삭제
```sql
    revoke all DB명.Table명 from user명.IP[%|localhost|...];
```


### DB 권한 삭제
```sql
    drop user user명.IP[%|localhost|...];
```


[REPO]

 1. [mysql 사용자추가/DB생성/권한부여](https://nickjoit.tistory.com/144-0)