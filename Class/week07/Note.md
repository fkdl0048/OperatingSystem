# OperatingSystem

## 04/10

### Operating System structure

1. Operating System Services
2. User Operating System Interface
3. System Calls (Program Operating Interface)
4. Types of System Calls
5. System Programs
A. Operating System Design and Implementation
B. Operating System Structure
C. Operating System Debugging
D. Operating System Generation
F. System Boot

![image](https://user-images.githubusercontent.com/84510455/230811580-8a214e71-5a43-4b86-8073-b675a031e158.png)

### Operating System Services

1. User Interface

- Command Interpreter
- Graphical User Interface

2. Program Execution

- Process Management
- Job Control
- Process Scheduling
- CPU Scheduling

유저를 위해

1. I/O Operations

유저를 위해

2. File Systems manipulation

유저를 위해

3. Communications

유저를 위해

4. Error Detection

프로그램을 위해

5. Resource Allocation

리소스는 CPU, 메모리, I/O 장치 등이다.

프로그램을 위해

8. Accounting

현재는 클라우드로 대체, 원래는 한개의 컴퓨터를 나눠서 사용

프로그램을 위해

9. Protection and Security

**이러한 서비스를 user interface와 연결하는 것이 System Call이다.**  

CLI에서 다양한 명령어를 입력하면 System Call이 실행되고, 이를 통해 OS가 서비스를 제공한다.  

시스템은 하드웨어와 소통한다.  

### user operating system interface

- user operating system interface는 user와 operating system 사이의 interface이다.

ex) CLI의 ls, dir 등이 user operating system interface이다.

*(API - Application Programming Interface)*

### System Call

![image](https://user-images.githubusercontent.com/84510455/230815506-a7175a41-4287-4ede-95d4-54619336e54d.png)

- System Call은 프로그램이 OS에게 서비스를 요청하는 것이다.

operating system의 서비스를 제공받을려면 system call을 사용해야 한다.  

구조도를 보면 전체적인 운영체제 시스템의 구조를 알 수 있다.  

- programming interface는 프로그램이 운영체제와 소통하는 방법이다.

c언어의 fork()가 system call이다.

- user interface는 사용자가 운영체제와 소통하는 방법이다.

컴퓨터 사용시

시스템 콜에서 open()을 통해서 인자값을 넘겨준다.  

여기서 인자값은 파일의 이름이다.

인자값의 파일 이름은 레지스터에서 꺼내옴

user program과 operating system의 소통과정

### Types of System Calls

1. Process Control
2. File Management
3. Device Management
4. Information Maintenance
5. Communications
6. Protection

![image](https://user-images.githubusercontent.com/84510455/230815558-eeb6514e-e374-48b7-aabe-9ef779ba08eb.png)