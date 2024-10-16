# hello-world
인프런 강의를 들으며 실습해보는 Git 공부용 레파지토리 입니다.

# Origin / HEAD
미션1. origin/HEAD 가 뭐하는 기능인지, HEAD가 변경되는 시점 조사 (+실습, 및 강의내용 예습) </br>
미션2. 어뎁터 패턴이 무엇인지 이론 학습 (+응용 예제 코드 작성)</br>
</br></br>
'origin'이란? </br>
원격 저장소를 클론하면 원격 저장소의 실제 이름(hello-world)과는 별개로, Git은 원격 저장소를 'origin'으로 참조하여 관리한다. </br>
또한 클론해오는 과정에서 로컬 저장소의 원격 참조는 다음과 같이 설정된다. (origin -> https://github.com/Heahu/hello-world.git) </br>
</br>
'origin'의 'HEAD'란? </br>
'origin'의 'HEAD'란 원격 저장소의 기본 브랜치에서 가장 최근의 커밋을 가리킨다. </br>
이를 통해 사용자는 원격 저장소의 최신 상태를 확인할 수 있으며, 자신의 로컬 저장소와 업데이트 상태를 비교할 수 있다. </br>
</br>
'origin'의 'HEAD'가 변경되는 시점 </br>
1. Push </br>
   로컬에서 작업한 내용을 원격 저장소에 푸시할 때, 원격 저장소의 'HEAD'가 해당 브랜치의 최신 커밋으로 업데이트된다. </br>
2. Pull / Fetch </br>
   원격 저장소의 변경 사항을 로컬로 가져올 때(Fetch)는 'HEAD'가 변경되지 않지만, 로컬 브랜치가 원격 브랜치와 동기화되는 과정(Pull)에서 'origin'의 'HEAD'가 업데이트된 커밋을 반영하게 된다. </br>
   즉 Fetch는 'HEAD'를 변경하지 않고, Pull일때 'HEAD'는 변경된다. </br>

![img](https://i.imgur.com/CyAZMrB.png)
![img](https://i.imgur.com/zmZS2gN.png)

