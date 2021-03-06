# Introduction to operating Systems

운영체제란 하드웨어 바로 위에 있는 소프트웨어

사용자와 다른 모든 소프트웨어, 하드웨어를 연결하는 **소프트웨어 계층**

**커널 : 운영체제의 핵심 부분으로 메모리에 상주 , 좁은 의미의 운영체제 = 커널**

### 운영체제의 목적

1.컴퓨터 시스템을 편리하게 사용하기 위함 

2.컴퓨터 시스템의 자원을 효율적으로 관리

(자원 = cpu , I/O장치 등등)

형평성 있는 자원분배, 주어진 자원의 최대한의 성능

프로세스, 파일, 메시지 등을 관리

하드웨어뿐만 아니라 소프트웨어 자원도 관리한다.

### 운영 체제의 분류

**동시 작업 가능 여부**

단일 작업(single tasking) : 한번에 하나의 작업만

다중 작업(multi tasking) : 동시에 2개 이상의 작업

요즘 운영체제는 다중 작업이다.

**사용자의 수**

단일 사용자

다중 사용자

**처리 방식**

**일괄 처리 (batch programing)**

→ 바로바로 처리하는게 아니라 작업 요청의 일정량 모아서 한꺼번에 처리

→ 현대 운영체제에서 찾아보기 힘든것, 현재 운영체제는 시분할 방식

**시분할(time sharing)**

→ interactive한 방식 : 키보드 입력했을시 바로 화면에 뜬다

→ 여러 작업을 수행 할 때 컴퓨터 처리 능력을 일정한 시간 단위로 분할하여 사용

→ 짧은 응답시간

정확한 데드라인이 있는건 아니지만 사람이 느끼게에 빠르고 

**실시간 (Realtime OS)**

데드라인이 있어서 정해진 시간 안에 어떤일이 반드시 종료되는걸 보장

특정한 목적을 가진 시스템

원자로/공장, 미사일 제어/ 반도체 장비/ 로보트 제어

오늘날 운영체제는 다중작업, 다중사용자, 시분할방식을 사용

Multitasking

Multiprogramming

Time sharing

Multiporcess

위의 4가지 용어는 유사한 용어로 컴퓨터에서 여러 작업을 동시에 수행하는 것

Multiprogramming은 여러 프로그램이 메모리에 올라가 있음을 강조

TimeSharing은 Cpu의 시간을 분할하여 나누어 쓴다는의미를강조

동시에 실행된다는건 CPU를 나눠가면서 빠르게 사용해 동시에 수행되는것처럼 보이는것

유닉스

대형컴퓨터를 위한 것.

코드 대부분 c언어로 작성

소스코드 공개

높은 이식성 : C언어로 작성됐기 때문에 환경이 달라져도 컴파일 하면 사용가능

### 운영체제의 구조

                  CPU

                      l

                  메모리

                        l

           디스크 /  IO device

CPU에서 뭔가 실행이 되려면 memory에 있어야 한다