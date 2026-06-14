# Control Bus

- CPU에서 Address Bus로 특정 주소를 지정하면, Control Bus는 그 주소 안에 있는 데이터를 어떤 식으로 처리할 것인가를 결정.

### 종류

1. Read

    > 지정된 주소의 데이터 읽기

1. Write

    > 지정된 주소에 데이터 쓰기

1. Interrupt

    > 사용자 입력 등으로 인해 CPU가 우선적으로 처리해야할 작업을 요청할 때 발생

1. Clock
1. Reset
1. Memory Request
1. I/O Request

### 방향성

- Address Bus와 Data Bus와 다르게, Control Bus는 어느 방향성을 띄고 있다고 딱 잘라 말하기 어렵다.
-  신호마다 방향이 다르기 때문.
    
    > Read, Write같은 신호는 CPU가 다른 부품에 보내지만\
    > Interrupt같은 신호는 다른 부품에서 CPU에 보낸다.