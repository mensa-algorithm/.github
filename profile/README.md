
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

이후, 자신의 branch에 code가 push 완료 됐는지 확인합니다.

이후 PR을 진행합니다.
만약 문제를 해결하지 못했고, 다른 팀원들의 의견을 듣고 싶으면, `step1.1 및 step1.2` 로 넘어갑니다.

## step1.1 - Review (선택 사항)

팀원들에게 자신의 코드 리뷰를 듣고 싶으면 `Issue 발행 - Review 템플릿`을 선택합니다.
![image](https://github.com/user-attachments/assets/42b61416-8045-421a-b1bc-30e797ede083)

![image](https://github.com/user-attachments/assets/7ecc331c-8511-4f5f-9736-ad6818d0e8cc)

위 양식에 맞게 내용을 작성한 후, Issue를 발행합니다. 

## step1.2 - 문제 해결하지 못했을 경우 (선택 사항)

문제를 해결하지 못해서, 팀원들에게 조언을 얻고 싶다면 `Issue 발행 - 어려운 문 템플릿`을 선택합니다.
![image](https://github.com/user-attachments/assets/d742081c-5d84-4e61-a30a-09f88393dfd8)

![image](https://github.com/user-attachments/assets/808e9d7a-a27c-48fc-9bcc-12b39db0b8df)

위 양식에 맞게 내용을 작성한 후, Issue를 발행합니다.

## step1.3 - 팀원들의 의견을 들은 후 (선택 사항)

팀원들의 의견을 들은 후, 다시 문제를 해결합니다. 이후, PR을 진행합니다.

## step2 - 문제 해결 및 Pull Request

문제 해결을 했으므로, 문제 해결 Issue를 발행합니다.

![image](https://github.com/user-attachments/assets/a8beb040-0152-44f9-8f05-1366ecb4293b)

이후, PR을 진행합니다.
![image](https://github.com/user-attachments/assets/307949d5-fd4c-488b-9f67-e2ff060f759e)

만약, `수정 사항이나 edge case`가 발견 되어 pr이 거부당한 경우는, PR을 닫지 말고, 다시 commit을 하면 됩니다.  
그러면 자동적으로 PR에 반영이 됩니다.
이후 `amm0124`의 pr 승인이 완료되면 끝입니다.

## step3 - 유의 사항

여러 사람이 사용하는 repository이므로 `다른 사람의 디렉토리 및 branch에 가서 내용을 수정하는 일은 없도록 합니다!!!!`

pr conflict 해결하기 힘듭니다!!! 

## step3.1 - local과 원격의 동기화

만약 자신의 원격 저장소(github/<자신 이름>)에 수동으로 내용을 변경하였고, local과 동기화를 원한다면 아래 명령어를 실행해주세요.

	git fetch 
 	git pull origin <자신의 branch 이름>

이는 변경 사항을 받아와서, pull하는 과정입니다. 이 때, local 작업 사항은 날아가므로, 반드시 다른 곳에 저장해주세요! 만약 안 된다면 저에게 말해주세요.



이상 모두 즐거운 알고리즘 ~
