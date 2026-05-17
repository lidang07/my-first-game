# Week11 실습

## 오늘 한 것
- PyInstaller 설치 및 빌드
- resource_path() 함수 추가
- --add--data 옵션으로 에셋 포힘
- .exe 실행 확인
- 다른 컴퓨터에서도 실행 되는지 확인

## resource_path() 를 써야 하는 이유
개발 중 사용하는 .py와 배포할 때 사용하는 .exe에서 리소스 파일 경로가 다르기 때문에, 두 환경을 모두 커버하기 위해 사용한다.

## 빌드 명령어
- pip install pyinstaller (pyinstaller 설치)
- pyinstaller --version (pyinstaller 버전 확인)
- pyinstaller game.py (내 게임 .exe파일로 만들기)
- pyinstaller --onefile --windowed --add-data "assets;assets" --name=MyGame game.py (.exe 파일을 하나로 묶고 실행 시 터미널 창을 숨기고 assets폴더를 exe 안에 같이 포함하고 파일 이름을 MyGame.exe로 지정)

## AI 활용 내역
- 수업 중 resource_path()에 대해 잘 이해하지 못해 AI에게 물어봄
- 일반 실행 중엔 상대경로랑 똑같이 동작하고, exe로 배포할 때 경로가 깨지지 않도록 보호해주는 함수다.
