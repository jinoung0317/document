### Linux network file move 
### date : 2021-12-26
### tag  : \#압축, \#

---

### SCP
 
  - ssh을 사용하여 파일 이동

### 파일 가져오기
```shell
    >  scp OPTION REMOTE_ID@REMOTE_IP:ORIGIN_FILE_DIR_PATH DOWNLOAD_DIR_PATH [옵션] [원격지_id]@[원격지_ip]:[원본 위치] [받는 위치]
```
 - \-x : 묶음을 해제
 - \-c : 묶음을 묶음
 - \-v : 묶음/해제 과정을 화면에 출력
 - \-z : gunzip을 사용
 - \-f : 파일 이름을 지정
 - \-p : 권항을 원본과 동일하게 유지


### 파일 파일보내기
```shell
    > scp OPTION FINE_NAME[ ...] REMOTE_ID@REMOTE_IP:UPLOAD_DIR_PATH
```

 - \-r : 하위 디렉토리 모든 파일 이동
 - FILE_1 FILE_2 ... : 복수 파일 가능 | 공백으로 구분



[REPO]
 
 1. [리눅스 scp 명령어 사용법](https://eehoeskrap.tistory.com/543)



 