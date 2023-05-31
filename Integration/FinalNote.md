# OperatingSystem Note

## 9장.Virtual Memory

버츄얼 메모리, 가상 메모리는 물리적 메모리의 한계를 극복하기 위해 나온 개념이다.

프로세스를 실행할 때 실행에 필요한 일부분만 메모리에 로드하고 나머지는 디스크에 두는 것이다.

현재 필요한 page만 메모리에 올리는 것을 Demand Paging이라고 한다. 

### Demand Paging

Demand paging은 실제로 필요할 때 page를 메모리에 올리는 것이다. 

이를 통해 CPU 이용률과 처리율이 높아지고, 더 많은 사용자를 수용할 수 있다.  

## 10장. File System

파일은 논리적 저장단위로 관련된 정보 자료들의 집합에 이름을 붙인 것이다.

컴퓨터 시스템의 편리한 사용을 위해 정보 저장의 일괄된 논리적 관점을 제공한다.  

일반적으로 레코드(Record) 혹은 블록(Block) 단위로 비휘발성 보조기억장치에 저장된다.  

파일 속성(File attribute) 또는 파일의 메타데이터(metadata)는 파일을 관리하기 위한 각종 정보들이다. 파일 자체의 내용은 아니다. 

파일 이름, 유형, 저장된 위치, 파일 사이즈, 접근 권한, 소유자, 시간(생성/변경/사용) 등 파일에 대한 전반적인 정보를 말한다. 

파일 시스템(File System)은 운영체제와 모든 데이터, 프로그램의 저장과 접근을 위한 기법을 제공한다.

시스템 내의 모든 파일에 관한 정보를 제공하는 계층적 디렉터리 구조이고, 파일 및 파일의 메타데이터, 디렉터리 정보 등을 관리한다.

파티션(Partition)은 연속된 저장 공간을 하나 이상의 연속되고 독립적인 영역으로 나누어 사용할 수 있도록 정의한 규약이다. 하나의 물리적 디스크 안에 여러 파티션을 두는 게 일반적이지만, 여러 물리적 디스크를 하나의 파티션으로 구성하기도 한다. 
