
# git organization 사용법 - 작성자 amm0124

## Overview
main branch는 최종적으로 완료된 코드만 올립니다.
각자 이름별로 branch가 있습니다.





## step1 - 자신의 branch에 문제 해결하기
	
    git clone https://github.com/mensa-algorithm/2024-2.git
   
 을 통해 local 저장소에 repository를 clone합니다. main branch만 clone이 됩니다.
   
	git branch 
   
 명령어를 통해 main branch만 있는지 확인해주세요. 이제 clone한 repository로 경로를 이동합니다.
	 
	cd 2024-2

이동했으면, 자신이 작업 할 branch를 생성해야 합니다. 

![image](https://github.com/user-attachments/assets/aeb21be6-4d6f-421f-9269-29342d5776f4)

각자 이름(닉네임)별로 미리 branch를 만들어놨습니다.
이후 아래 명령어를 통해, 자신의 local에 branch를 만들고, 이동합니다.
  
    git branch <자신의 이름(닉네임)>
    git checkout <자신의 이름(닉네임)>

자신의 닉네임에 해당하는 directory를 생성합니다. 

    mkdir <자신의 이름(닉네임)>
    touch <자신의 이름(닉네임)>/README.md
    cd <자신의 이름(닉네임)>

README.md는 디렉토리임을 알려주기 위해 임시로 생성했습니다. 경로를 이동했습니다.
이후 ps를 진행하는 플랫폼 디렉토리를 생성합니다.

    mkdir <platform .. ex boj, programmers..>

플랫폼 디렉토리를 생성했으면, 디렉토리로 이동 후, 문제 소스 코드를 작성합니다.
이후, 문제를 push합니다.

    git push origin <자신의 이름(닉네임)>

이후, push가 완료 됐는지 확인합니다.

이후 PR을 진행합니다.


## step2 - Pull Request

나중에 작성하겠습니다.

    

 

