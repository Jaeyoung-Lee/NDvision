NDvision 인공지능 개발 키트 예제
이 저장소는 NDevice(엔디바이스)에서 개발한 NDvision 인공지능 개발 키트 사용자를 위한 공식 예제 코드와 가이드를 제공합니다. 모든 예제는 NDevice에서 제공하는 VS Code 확장판을 기준으로 작성되었습니다.

🚀 1. 빠른 시작
1.1. 필수 요구 사항
본 예제 코드를 사용하기 위해서는 다음 항목들이 PC에 설치되어 있어야 합니다.

- NDvision 개발 키트 하드웨어
- Visual Studio Code (VS Code, https://code.visualstudio.com/download): 개발 환경
- ND Controller VS Code 확장판: 장치 제어 및 시각화 도구
- Python 3.x: (가상 환경 권장)

1.2. 저장소 복제 (Clone)
- ND Controller 확장판에서 예제 복사
- VS Code 터미널 또는 Git Bash를 사용하여 이 저장소를 로컬 PC로 복제하십시오.

git clone https://github.com/[GitHub 사용자 이름]/[Repository 이름].git
cd [Repository 이름]

📦 2. 예제 코드 디렉토리 구조
핵심 기능별로 디렉토리가 구분되어 있습니다. 각 폴더 내부의 README.md 파일에서 자세한 실행 방법을 확인하십시오.

디렉토리	설명	주요 기술
01_device_control	장치 연결, 해상도 변경, 파라미터(노출 시간 등) 설정 예제.	SDK API, USB 통신
02_live_streaming	실시간 RGB 이미지 및 깊이 맵 데이터를 받아 화면에 출력하는 예제.	OpenCV, 깊이 맵 시각화
03_3d_liveness	획득한 깊이 데이터를 분석하여 **3D 정합성(Liveness)**을 확인하는 예제.	스테레오 정합 알고리즘
04_pytorch_npu	PyTorch 모델 학습 후, Luckfox NPU용으로 변환 및 배포하는 워크플로우 예제.	PyTorch, ONNX, 모델 최적화 툴
05_face_recognition	깊이 정보를 활용한 얼굴 인식 기본 파이프라인 예제.	FaceNet (PyTorch), 3DMM (선택적)
