# Thrashing (스래싱)

- 가상 메모리 환경에서 페이지 폴트가 과도하게 발생하여, CPU가 실제 프로그램 실행보다 페이지 교체 작업에 대부분의 시간을 소비하는 상태

- Thrashing 발생 조건 및 원인

	1. 메모리 용량 부족
	1. Page Fault 폭증
	1. 과도한 멀티프로그래밍
	1. Working Set 유지 불가
    	> Working Set이란, 일정 시간 동안 프로세스가 자주 사용하는 페이지의 집합이다.

- Thrashing해결을 위한 운영체제의 대응과 대체 방법

	1. 프로세스 수 감소
	1. Working Set모델 사용
	1. Page Fault 빈도 조절

        > Page Fault 발생 빈도를 감시한다. 빈도가 높으면 프레임을 더 할당하고, 빈도가 낮으면 프레임을 회수 하는 등의 방법을 사용한다.\
		> 이를 `PFF(Page Fault Frequency)`방식이라고 한다.
	1. RAM 추가