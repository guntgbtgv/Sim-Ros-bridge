# Sim-Ros-bridge

## Why real-time simulation software? 
- 일반적으로 simulation이라 하면, 실제 시간의 흐름에 상관없이, 임의의 값으로 설정한 timestep으로 수치적 실험(numerical experiment)을 하는 것을 의미. 
    - (예: implicit Euler method 사용하여, $\Delta t$ = 0.001s 으로 대포발사를 3초동안 시뮬레이션하는 데에 0.1초도 안걸릴 것)
- 장점:
    - Real-time 으로 시뮬레이션을 진행함으로서, 보다 실제 hardware 로 실험하는 것과 유사한 환경에서 데이터를 뽑아볼 수 있음
    - 다관절 구동하는 로봇의 경우, 실제 시스템에서 발생할 수 있는 사고 (발산하다가 모터가 타버린다던지 ㅎㄷㄷ)를 미리 발견할 수 있어, 고장을 예방하고, 연구비도 절감하고, 수리에 들어가는 시간을 아낄 수 있음
- 단점: 
    - 사용법이 다소 까다롭기 때문에, 빠르고 간단한 prototyping 에는 적합하지 못할 수 있음


## How to use simulation software

### 시뮬레이션 소프트웨어의 API 를 사용하는 방법
API documentation 을 참고해가며 환경, 제어, 센서 등을 직접 코딩
- 장점: 
    - 시뮬레이션에서 제공하는 모든 기능을 쓸 수 있음
- 단점: 
    - software-specific 한 지식에 시간을 쏟아야함
    - software API 가 제공하는 프로그래밍언어만 쓸 수 있음 
    - 과연 이 software API가 본인에게 필요한 skill set 인지 고민해볼 필요 
    - 

### 시뮬레이션 소프트웨어와 ROS간의 통신을 이용하는 방법

## How to communicate between simulation software & ROS

