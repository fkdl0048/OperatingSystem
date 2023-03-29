# OperatingSystem

## 03/27

하드웨어 인터럽트 2가지

소프트웨어 인터럽트 2가지

다음 주 퀴즈

## 03/29

### Process management

![image](https://user-images.githubusercontent.com/84510455/228408546-f2a2afcc-6b89-403d-98b4-e0835f04b1d9.png)

프로세스란?

실행중인 프로그램으로 메모리에 올라와 있는 프로그램

프로그램 카운터란? 

프로그램 카운터는 프로그램이 실행되는 위치를 가리키는 레지스터

PCB란?

프로세스의 상태를 저장하고 있는 자료구조

인터럽트가 발생하면 컨트롤러가 PCB를 저장하고, 다음 프로세스의 PCB를 불러온다.

이를 컨텍스트 스위칭이라고 한다.

멀티쓰레드란?

하나의 프로세스 안에 여러개의 쓰레드가 존재하는 것

### Process Management Activites

* Creating and deleting both user and system processes

OS는 시스템 프로세스와 사용자 프로세스를 생성하고 삭제한다.

사용자는 인터페이스만 사용해서 시스템과 상호작용하지만 OS는 뒤에서 프로세스를 생성하고 삭제한다.(관리)

웁스~!🫢

* Scheduling

어플리케이션을 실행할 때 우선순위를 정해주는 것

*Suspend and resume*

* Synchronizing

* Allocating and deallocating resources

### Memory Management

![image](https://user-images.githubusercontent.com/84510455/228410853-fba91947-1c44-4062-ba99-998878e58085.png)

프로그램을 시작하기 위해서 어느 메모리를 사용할 것 인지 결정하는 것

순서를 따라가면 프로그램을 실행하기 위해서는 메모리에 올라와야 한다.

메모리에 올라가기 위해서는 메모리에 올라갈 위치를 결정해야 한다.

메모리에 올라갈 위치를 결정하기 위해서는 메모리에 어떤 프로그램이 올라가 있는지 알아야 한다.

이런 일련의 과정을 Memory Management이라고 한다.

ex) 메모리에 올라가 있는 프로그램이 3개가 있다. 이 때, 4번째 프로그램을 메모리에 올리려고 한다. 이 때, 4번째 프로그램을 메모리에 올릴 수 있는 공간을 찾아야 한다.

### Storage management

File에 대한 본질은 데이터의 묶음이다.

복잡하고 다양한 종류 파일 저장 장치: 컴퓨터  
단순한/일월화된 파일의 모습: 유저

### File System Management

* 사용자가 원하는 데로 구성이 가능하게
  * 생성, 수정, 삭제등등..

파일을 생성하기 위해선 먼저 파일을 저장할 공간을 할당해야 한다.

파일을 저장할 공간을 할당하기 빈 곳이 어디인지 파악해야 한다.

