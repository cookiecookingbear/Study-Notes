# Memory Buffer Register(MBR)

- CPU와 메모리 사이에서 실제로 이동하는 데이터나 명령를 임시 저장하는 레지스터

- 다른 말로 Memory Data Register(MDR)이라고도 한다.

- 메모리 접근 순서

	1. MAR과 Address Bus를 통해 정해진 주소의 메모리에 접근한다.
	1. Data Bus를 통해 물리적으로 메모리 안의 내용물이 CPU로 전송된다.
	1. MDR에 해당 내용이 전송된다.
	1. 만약 내용물이 명령어라면, MDR에 저장된 내용물이 IR로 전송된다.