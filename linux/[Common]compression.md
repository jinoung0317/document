### Linux compression 
### date : 2021-12-26
### tag  : \#압축, \#

---

zip vs tar.gz
zip    : 윈도우에서 사용, 폴더&파일을 묶고 압축
tar.gz : 리눅스에서 사용, 폴더 묶기, 압축을 따로 진행

### tar 명령어 사용법
```shell
    > tar OPTION FILE_NAME DIR_PATH
```
 - \-x : 묶음을 해제
 - \-c : 묶음을 묶음
 - \-v : 묶음/해제 과정을 화면에 출력
 - \-z : gunzip을 사용
 - \-f : 파일 이름을 지정
 - \-p : 권항을 원본과 동일하게 유지


### tar.gz 압축
```shell
    > tar -cvzf FILE_NAME DIR_PATH
```

### tar.gz 해제
```shell
    > tar -xvzf FILE_NAME DIR_PATH
```



[REPO]
 
 1. [tar,gz,zip 압축 및 압축해제](https://realforce111.tistory.com/40)

 2. [tar,gz,zip 압축 및 압축해제](https://brownbears.tistory.com/161)


 