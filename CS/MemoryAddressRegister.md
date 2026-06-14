# Memory Address Register(MAR)

- CPU가 ==현재== 접근하려는 메모리 주소를 저장하는 레지스터

    > PC와 비슷하지만, PC는 다음에 읽을 명령어의 메모리 주소를 저장한다.

- CPU에서 메모리 접근 순서

    1. 주소 계산
    1. MAR에 주소 저장
    1. Address Bus 출력
    1. 메모리 접근

- 명령어 Fetch과정에서는 다음에 읽을 명령어의 주소가 이제 현재 접근하려는 메모리의 주소가 되므로, MAR <- PC로 주소가 저장된다.

- MAR과 거의 항상 같이 나오는 **MDR(Memory Data Register)**

    > MDR은 MAR과 Address Bus을 통해 얻어낸 메모리 안의 ==내용물==을 저장한다.