# Quiz

* remote 깃과 local 을 clone명령어를 통해 동기화 합니다. 
> git clone https://github.com/lini1634/Quiz.git

* 깃 remote에다가 origin을 추가합니다. 
> git remote add origin https://github.com/lini1634/Quiz.git

* 리모트 저장소에서 identity를 위해 환경설정을 해줍니다.
> git config --global user.email "lini1634@naver.com
> git config --global user.name "lini1634"


* 20190924 quiz를 .ipnyp형태로 다운받아서 로컬 C드라이브 Pattern recognition, quiz에 추가합니다.
> git add . 

* staging area로 옮기기 위해 add한 파일을 commit합니다.
> git commit -m "20190924_Quiz1"


* 웹으로 올리기 위해 commit한 파일을 push해줍니다.
> git push

* 원래는 master브랜치가 디폴트인데 solution 브랜치를 하나 더 생성합니다. 
> git branch --create "solution"

* HEAD가 master를 가리키고 있는데 solution으로 옮깁니다
> git switch solution

* solution에다가 퀴즈 정답을 다운받은것을 add .와 commit을 통해 올리고, push해줍니다
> git push --set-upstream origin solution

* solution 을 master에 합쳐줍니다.
> git branch merge

* 이때까지 한것을 확인합니다.
> git log

* 브랜치를 지워줍니다.
> git push origin --delete solution
