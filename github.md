# **원격 저장소 (remote repository)**

## **기본 설정**

1. 로컬 git 저장소 준비

2. Github repository 생성![img](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/24222ced-cd02-43c0-bbf3-eba22d1d801e/image-20210623170259834.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20210624%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20210624T082531Z&X-Amz-Expires=86400&X-Amz-Signature=58314a8435d5f1195428572cfc2511ba271b79d88dac8cb4016b786ec641cc16&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22image-20210623170259834.png%22)

3. Repository default branch 변경 (settings -> repositories)

   - main -> master로 변경

   

   

   ![img](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/c405a7c2-8fc4-4537-99e0-b62da2ac2cfb/tempsnip.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20210624%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20210624T081237Z&X-Amz-Expires=86400&X-Amz-Signature=f331f84553acbebb1eb7214dadce761733bdfc610cc9043280142765f4a3a6e4&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22tempsnip.png%22)

   

   

   **명령어**

### **원격 저장소 주소 추가**

```
$ git remote add origin 저장소URL
```

> "git아, 원격 저장소(remote) 추가해줘(add) origin 이라는 이름으로 저장소  URL을!!!"

- origin은 원격 저장소 이름!

### **원격 저장소 목록 보기**

```
$ git remote -v
origin  <https://github.com/woongedu/TIL.git> (fetch)
origin  <https://github.com/woongedu/TIL.git> (push)
```

> 잘못 add 한 경우 삭제하기$ git remote rm origin

### **원격 저장소에 업로드 (push)**

```
$ git push -u origin master

Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (8/8), 645 bytes | 645.00 KiB/s, done.
Total 8 (delta 0), reused 0 (delta 0), pack-reused 0
To <https://github.com/woongedu/TIL.git>
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
```

> "git아, push 해줘 origin이라는 이름의 원격저장소에 master 브랜치로!!!!"

> 원격 저장소에는 commit이 올라간다 !!!즉, commit 이력이 없다면 push 할 수 없다.

- 두번째 push 부터는 `u` 생략 가능

### **pull**

- 원격 저장소의 변경사항을 받아옴 (업데이트)

```
$ git pull origin master
```

### **clone**

- 원격 저장소 전체를 복제

```
$ git clone 저장소URL
```

> [주의사항]clone 받은 프로젝트는 이미 git init이 되어있음 (remote 도 추가되어 있음)