##	Github page란?

git 레포지토리를 이용해서 손쉽게 웹사이트를 배포할 수 있는 기능이다. 



자기소개서나 블로그를 운영할 때 많이 사용된다. 



###	1.업로드 하고 싶은 홈페이지 코드를 가져온다.



실제로 코드를 작성해도 좋고, (HTML, CSS, JavaScript 활용) 이미 만들어진 코드를 가져와서 변경해도 좋다.



[템플릿 받는 링크](https://startbootstrap.com/)



###	템플릿 다운 받기



Startbootstrap → themes 메뉴 → portfolio-resume 메뉴  →  원하는 무료 템플릿 다운



![스크린샷 2021-06-26 오후 8.50.00](스크린샷 2021-06-26 오후 8.50.00.png)



다운로드 이후 

```
git init
git add .
git commit -m "커밋 메세지"
git remote add origin 레포지토리주소
git push --set-upstream origin master

```



GitHub 레포지토리에서 setting → page  에서 source 의 None →  master 로 변경

![스크린샷 2021-06-26 오후 8.56.20](스크린샷 2021-06-26 오후 8.56.20.png)



Your site is ready to be published at http://~~~~ 	라고 뜨면 완료 !



## 추후 웹페이지는 HTML , CSS , JavaScript를 활용해서 만듭니다.



