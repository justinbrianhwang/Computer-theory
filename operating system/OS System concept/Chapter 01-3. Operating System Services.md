# Services Provided by Operating Systems

---

## 1. Booting Services

### Booting and Bootstrapping

- The process of loading the operating system into main memory.
- Ensures the computer hardware is ready and initializes software components.

### Bootstrap Loader

- A small program stored in ROM, responsible for loading the operating system from secondary storage into main memory.

![Booting Service](https://i.imgur.com/WlU25YO.png)

---

## 2. User Services

### Providing User Interfaces

1. **CLI (Command Line Interface):**
   - A text-based interface where commands are entered manually.

   ![CLI](https://i.imgur.com/yHujTD4.png)

2. **Menu Interface:**
   - Interaction through menus, often used in simpler systems.

   ![Menu Interface](https://i.imgur.com/PiuzBeG.png)

3. **GUI (Graphical User Interface):**
   - A graphical environment enabling intuitive interaction (e.g., Windows, macOS).

   ![GUI](https://i.imgur.com/VW4n3EX.png)

---

### Program Execution

- Loads programs into memory and allocates CPU time.
- Handles scheduling, memory allocation, and process termination.

---

### I/O Operations

- Provides methods for user programs to perform input/output indirectly.
- Manages user inputs and produces the desired outputs efficiently.

---

### File System Manipulation

- Handles file operations such as creating, reading, writing, deleting, and organizing files.
- Ensures secure and efficient file operations.

---

### Communication

- Facilitates data exchange:
  1. Between processes on the same machine.
  2. Across networked systems using shared memory or message passing.

---

### Error Detection

- Detects and handles errors at hardware and software levels.
- Common error types:
  1. **Hardware Errors**: Memory faults, power failures.
  2. **I/O Errors**: Printer paper jams, disk read failures.
  3. **Software Errors**: Division by zero, memory access violations.

---

## 3. System Services

### Resource Allocation

- Allocates CPU, memory, and other resources to concurrent processes and users.
- Ensures fair and efficient resource usage.

---

### Accounting

- Tracks resource usage by users and applications.
- Helps in performance evaluation and optimization.

---

### Protection and Security

1. Prevents unauthorized access to system resources and data.
2. Ensures processes do not interfere with each other.
3. Enforces validation for system calls to prevent misuse.
4. Implements authentication to protect external devices and user data.

---

## 4. System Calls

### Definition

1. **Interface Between User Programs and the OS:**
   - Provides access to low-level hardware and kernel functions.
2. **Execution:**
   - Transfers control from user mode to kernel mode, performs the request, and returns control.

---

### OS System Call Services

1. **Process Management:**
   - Functions: Create, terminate, allocate memory, and set attributes.
2. **File Manipulation:**
   - Functions: Open, close, read, write, delete, and manage files.
3. **Device Management:**
   - Functions: Request, release, read/write devices, and configure attributes.
4. **Information Management:**
   - Functions: Access system date, time, and resource attributes.
5. **Communication:**
   - Functions: Establish connections, send/receive messages, and manage remote devices.

---

### Example of System Calls

![System Call Example](https://i.imgur.com/jzlDHpw.png)



# Korean

# 운영체제의 서비스 제공

---

## 1. 부팅 서비스

### 부팅과 부트스트래핑

- 운영체제를 메인 메모리에 적재하는 과정.
- 컴퓨터 하드웨어를 초기화하고 소프트웨어를 준비 상태로 만듦.

### 부트스트랩 로더

- ROM에 저장된 소규모 프로그램으로, 보조 기억 장치에서 운영체제를 메인 메모리로 적재.

![Booting Service](https://i.imgur.com/WlU25YO.png)

---

## 2. 사용자 서비스

### 사용자 인터페이스 제공

1. **CLI(명령어 라인 인터페이스):**
   - 사용자가 텍스트 명령어를 직접 입력하여 컴퓨터와 상호작용.

   ![CLI](https://i.imgur.com/yHujTD4.png)

2. **메뉴 인터페이스:**
   - 메뉴를 이용해 시스템과 상호작용.

   ![Menu Interface](https://i.imgur.com/PiuzBeG.png)

3. **GUI(그래픽 사용자 인터페이스):**
   - 그래픽 환경에서 직관적인 방식으로 사용자와 상호작용 (예: Windows, macOS).

   ![GUI](https://i.imgur.com/VW4n3EX.png)

---

### 프로그램 실행

- 프로그램을 메모리에 적재하고 CPU 시간을 할당.
- 메모리 할당, 프로세스 스케줄링 등 작업 처리.

---

### 입출력 동작 수행

- 사용자 입력을 처리하고 필요한 출력을 생성.
- 간접적인 입출력 방법을 제공하여 효율적 운영.

---

### 파일 시스템 조작

- 파일 생성, 읽기, 쓰기, 삭제 등 작업을 지원.
- 디스크 블록 할당 및 관리.

---

### 통신

- 프로세스 간 또는 네트워크를 통한 데이터 교환 지원:
  1. 컴퓨터 내 프로세스 간 정보 교환.
  2. 네트워크로 연결된 시스템 간 정보 교환.

---

### 오류 탐지

- 하드웨어 및 소프트웨어 오류를 감지하고 적절히 대처.
- 주요 오류 유형:
  1. **하드웨어 오류:** 메모리 손상, 전력 문제.
  2. **입출력 오류:** 프린터 종이 부족, 디스크 읽기 실패.
  3. **사용자 프로그램 오류:** 메모리 초과 접근, 잘못된 연산.

---

## 3. 시스템 서비스

### 자원 할당

- 다수의 사용자와 작업에 대해 메모리, CPU 등의 자원을 효율적으로 할당.

---

### 계정 관리

- 사용자가 사용한 자원량을 기록 및 추적.
- 시스템 성능 개선과 재구성에 활용.

---

### 보호와 보완

1. 사용자와 작업의 자원 접근 제한.
2. 동시 실행 중인 프로세스 간 간섭 방지.
3. 시스템 호출 매개변수의 적합성 확인.
4. 사용자 인증을 통해 시스템과 데이터를 보호.

---

## 4. 시스템 호출

### 정의

1. **운영체제와 사용자 프로그램 간 인터페이스:**
   - 사용자 프로그램이 운영체제의 기능을 요청할 수 있게 함.
2. **작동 원리:**
   - 사용자 모드에서 커널 모드로 제어권을 전달한 뒤 요청 처리 후 반환.

---

### 운영체제의 시스템 호출 서비스

1. **프로세스 관리:**
   - 생성, 종료, 메모리 할당, 속성 지정.
2. **파일 조작:**
   - 생성, 읽기, 쓰기, 삭제, 파일 속성 변경.
3. **장치 관리:**
   - 장치 요청, 해제, 읽기/쓰기, 속성 설정.
4. **정보 관리:**
   - 시스템 시간 및 자원 속성 접근.
5. **통신:**
   - 연결 생성, 메시지 송수신, 원격 장치 관리.

---

### 시스템 호출의 예시

![System Call Example](https://i.imgur.com/jzlDHpw.png)














