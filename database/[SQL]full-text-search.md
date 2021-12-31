### Database full text search sql 
### date : 2021-12-26

---

### setting 
 
  - /etc/mysq 경로에 my.cnf에 추가

```shell
    ft_min_word_len = 3 
    innodb_ft_min_token_size = 3
```

### 설정 확인
```sql
    show variables like '%ft_min%';

    OPTIMIZE TABLE TABLE_NAME;
```

### Table colume에 index 생성
```sql
    ALTER TABLE TABLE_NAME ADD FULLTEXT INDEX COLUMN_NAME (COLUMN_NAME) VISIBLE;
```


###  
```SQL
-- 검색어1 또는 검색어2 (or 검색) 
SELECT * FROM Table_Name WHERE MATCH(Col_Name) AGAINST('검색어1 검색어2'); 

-- 검색어 중간에 공백이 들어가는 경우 
SELECT * FROM Table_Name WHERE MATCH(Col_Name) AGAINST('"검색어 검색어"'); 

-- 검색어1을 검색한 결과에서 검색어2가 들어간것을 제외 할 때 
SELECT * FROM Table_Name WHERE MATCH(Col_Name) AGAINST('"검색어1" -검색어2' in boolean mode); 

-- 검색어1, 검색어2 함께 검색이 되는 경우 (and 검색) 
SELECT * FROM Table_Name WHERE MATCH(Col_Name) AGAINST('+"검색어1" +"검색어2"' in boolean mode); 

-- 검색어1과 검색어2 And 검색과 함께 검색어2의 결과도 함께 출력 
SELECT * FROM Table_Name WHERE MATCH(Col_Name) AGAINST('"검색어1" +"검색어2"' in boolean mode);

```
 

 
 
 
[REPO]
 
 1. [crontab 명령어 관련](https://stricky.tistory.com/435)

 2. [MySql Full-text Search 설정](https://kabkee.github.io/mysql/mysql-full-text-search/)