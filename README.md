C++ 개발 환경 구축 가이드

1. mingw64 설치
2. mingw64 환경 변수 지정
3. cmd or powershell에서 g++ --version, gcc --version으로 설치 되어있는 버전 확인
4. VSCODE에서 C++ 패키지 에디터 설치
7. 설정에서 C/C++ Edit Configuration(UI)로 진입
8. 컴파일러 경로 지정(역슬래쉬가 아닌 일반 경로 설정 슬래쉬로 작성)
9. IntelliSence모드에서 gcc-x64 설정
10. C 표준을 gnu-11 C++ 표준을 gnu++14로 설정
11. cpp 파일 만들어서 코드 입력하기
12. tasks.json 파일을 만들기 위해서 터미널 - 기본 빌드 작성 구성..을 클릭
13. 디버깅을 실행하기 위해서 launch.json 파일을 생성 설정은 C++ (GDB/LLDB)로 지정
14. 여기서 launch.json을 만들면 빈깡통 상태라서 구성 추가 - gdb 시작을 클릭하면
15. ctrl + shift + c or 바로가기키에 컴파일 키를 입력하면 파일명.exe가 생성된다.
16. 빌드가 됬다면 exe가 생성될 것이고 빌드에 오류가 발생했다면 지정한 컴파일러가 문제일 확률이 굉장히 높다

컴파일러는 두 종류로 gcc는 C언어용이며 gc++이 C++언어용 컴파일러다.

17. 이후 cpp 파일을 클릭하고 디버깅을 실행하면 출력에서 입력한 코드의 출력을 확인할 수 있다.

파일 구조도
C-_language/
│
├── hello.cpp               # 소스 코드 파일
├── hello.exe               # 컴파일된 실행 파일
└── .vscode/                # VSCode 설정 폴더
    ├── c_cpp_properties.json # C/C++ 설정 파일
    ├── launch.json         # 디버깅 설정 파일
    └── tasks.json          # 빌드 설정 파일

 