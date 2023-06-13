# 기말고사 대비 문제 모음

대부분의 질문에 대한 답변은 강의 내용을 넣어서 작성할 것

## 1. 운영체제란?

운영체체에 대한 내용 서술

ex) 하나의 소프트웨어이다. 하드웨어를 관리하는 소프트웨어이다. 등등

## 2. 전체적인 챕터 검증

1. 배워야 하는 이유
2. 운영체제 주요 특성 중 어디에 해당하는지

- 프로세스 관리
- 메모리 관리
- 파일 관리
- 입출력 관리

## 3. scheduling에 대한 정의

(1+1) 일반적으로 scheduling 이란 무엇이며 언제 scheduling 이 발생하는가?

(CPU 스케줄링, I/O 스케줄링을 구분하여 각각 제시해야 함)

1. CPU 스케줄링
2. I/O 스케줄링

## 4. 멀티 프로그래밍

1) 멀티 프로그래밍이란 무엇이고, 이것이 가능하려면 운영체제는 무엇을 제공해야 하는가

## 5. 컴퓨터 시스템 하드웨어적 / 소프트웨어적구성

컴퓨터 시스템은 하드웨어적 / 소프트웨어적으로 어떻게 구성되어 있는가? 각각 구성에 대해서 중요 요소를 거론하고 간단히 설명하라.

1. 하드웨어적 구성
2. 소프트웨어적 구성

## 6. 파일을 구성할 경우 필요한 전체 사이즈 계산

2000K 의 텍스트 파일이 있다. 블록 사이즈를 120K 이라고 가정 할 때 인덱스 와 링크 리스트 방법으로 파일을 구성할 경우 필요한 전체 사이즈를 각각 제시하라. (인덱스 크기는 120K, 포인터 크기는 10K)

## 7. disk access time 이란?

disk access time 이란? 이것은 무엇에 의해서 지배를 받으며 시스템 효율에 어떠한 영향을 미치는지 상세히 논의하라.

## 8.메모리 관리 모듈의 요소 하드웨어 및 소프트웨어 관점

(1.5점+1.5점) 운영체제 중 메모리 관리 모듈의 요소를 하드웨어 및 소프트웨어 관점에서 제시하고, 이 운영체제가 가상 메모리를 가능하게 하기 위해서 필요한 요소를 하드웨어 및 소프트웨어 관점에서 구체적으로 제시하라.

## 9. 라운드 로빈 스케줄러

(2점) 라운드 로빈 스케줄러는 일반적으로 정확히 한번 나타나는 각 프로세스들과 함께 모든 수행 중인 프로세스들의 리스트를 유지한다. 만약 프로세스가 리스트에서 두 번 나타난다면 어떻게 되는가? 이것을 허용한 이유는 어떤 장점을 얻고자 함인가? 단점은 무엇인가?

## 10. Page Fault

페이지 부재 시 발생하는 일련의 과정이다. 이 때 아래 문제에 대해 적절한 답변을 서술하시오

![Image](https://github.com/fkdl0048/ToDo/assets/84510455/a404afa9-e53a-4905-bc32-3cd38940853b)

1. 2번의 과정에서 해당 프로세스의 상태가 변화하는 원인과 과정을 서술하시오(프로세스 상태도를 고려)

2. 위의 과정에서 Context Switch가 발생하는 과정 번호와 발생하는 원인, 위의 과정에서 Context Switch가 발생하는 총 횟수를 서술하시오.

3. 필요한 페이지가 메모리에 적재된 후 10번 과정에서 페이지 테이블에 어떤 변화가 생기는지 서술하시오.

## 11. file open statement

프로그램에서 file open statement를 수행할 때 일어나는 interrupt-driven I/O의 과정을 나타낸 것이다.

![Image](https://github.com/fkdl0048/ToDo/assets/84510455/02f1744f-18e3-44df-af93-4f0bec0ebeea)

여러분의 프로그램이 현재 파일을 읽고 있는 과정이고 그다음 step은 연산을 하는 statement 가 있다고 가정하고, 현재의 step 과 그 다음 연산을 하는 step 사이에 일어나는 일을 상세히 설명하라. 여러분의 프로세서 번호가 P1번이고, 다른 사용자의 번호가 P2-P9번, 그리고 OS가 P0 이다. (각 스텝 번호에서 어느 프로세서가 어떤 수행을 하는지 상세 제시해야 함, 그렇지 않으면 0점 처리).

## 12. 파일이 실제 디스크에 저장되는 과정

(0.8+0.8+0.8+0.8+0.8 = 4점) 여러분의 파일이 실제 디스크에 저장되는 과정을 아래의 그림을 참조해서 상세히 설명하라. applicatio programs 부터 devices 까지 각 모듈 간의 맵핑 방법을 제시해야 하고 그렇지 않으면 0점 처리.

![Image](https://github.com/fkdl0048/ToDo/assets/84510455/d6fcc915-0161-4be1-8830-003e8abc8242)

## 13. disk read

10, 22, 20, 2, 40, 6, 38 실린더와 같은 디스크 요청들이 Disk driver로부터 들어왔다. 실린더 1을 움직이는데 걸리는 탐색시간은 6msec이다. 다음 알고리즘들을 사용하면 얼마나 많은 탐색시간이 필요한가? 모든 경우에 arm은 cylinder20에서 시작한다고 가정하자

1. First Come, First Service
2. Elevator(SCAN) algorithm (initially moved upward)

## 14. time sharing

현재 컴퓨터 내에서 A 프로그램과 B 프로그램이 동시(time sharing)에 수행되고 있다고 가정하자. A 프로그램이 Data read instruction (I/O instruction) 을 수행하고 있고 B 프로그램이 수학적 계산 프로그램 (CPU instruction)을 수행하고 있는 경우 OPTIMAL 한 Operating System 이 하는 일을 I/O 관련 사항 (device, controller, driver)을 포함하여 매우 상세히 설명하라.

## 15

아래의 instruction 에서 address binding 은 compile time, load time, 그리고 execution time 등 3가지 경우에 발생할 수 있다. 세 가지가 발생할 때의 기계어 코드의 내용 변환 (if any) 을 쓰고, 이 세 가지중 가장 효율적이라고 생각되는 방법과 가장 비효율적이라고 생각되는 방법을 한 가지씩 선택하고 그 이유를 간략히 설명하라.

Load R7, abc : 메모리 abc 의 내용을 레지스터 7번에 저장

1010 0111 XXXXXXXX

(1010 : load, 0111 : register 7, XXXXXXXX : the rest 8bits are Memory address)

## 16

다음의 서로 다른 성격의 프로그램이 있다(below there are two different programs)

(1) 실시간으로 주어진 수학식을 계산하는 프로그램(A program that calculates the math equation in real time)

(2) 월별로 부서별 직원 봉급을 계산하는 프로그램(A program that calculates the employee salary for each departments monthly)

아래의 2단계는 운영체제의 발전과정을 나타낸다.(below two steps define the process of O/S development)

(i). No multiprogramming O/S

(ii). Multiprogramming support O/S

각각의 단계에서 운영체제가 제공해야 할 기능들(프로세서, 메모리, I/O)을 구체적으로 기술하고 (i)->(ii)로 upgrade 할 때 필수적인 것을 거론하라. (두 개의 서로 다른 프로그램이 수행되어야 한다는 점을 상기하기 바람)
(describe concretely the function about processor, memory, I/O which is provided by O/S and essential factor to be upgraded in initial O/S. Remind that above two different programs should be executed.)

(i) No Multiprogramming O/S

A. Processor management

B. Memory management

C. File management

D. I/O management

(ii) Multiprogramming support O/S (many program execute at the same time)

A. 전 운영체제에서 필수적으로 upgrade 되어야 할 것(essential upgrading factor in initial O/S)

B. Processor management

C. Memory management

D. File Management

E. I/O management
