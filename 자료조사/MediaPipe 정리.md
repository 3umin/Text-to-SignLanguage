# Mediapipe

- 설치
    - 단순히 파이썬에서 라이브러리 설치 명령어로 가능
- 기본 가이드
    - [MediaPipe Face Detection](https://google.github.io/mediapipe/solutions/face_detection#python-solution-api)
    - [MediaPipe Face Mesh](https://google.github.io/mediapipe/solutions/face_mesh#python-solution-api)
        
        실시간으로 얼굴의 468개의 3D 랜드마크 추정하는 얼굴형상 솔루션
        
        만약 표정을 수어로 활용한다면 사용하면 좋을 듯.. 근데 안하지 않을까?
        
    - [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands#python-solution-api)
        
        손을 탐지해서 손의 움직임을 실시간으로 감지하는 기능
        
    - [MediaPipe Holistic](https://google.github.io/mediapipe/solutions/holistic#python-solution-api)
        
        손가락, 몸(포즈), 표정 등을 한번에 추적할 수 있는 시스템
        
        모바일 기기를 활용해서 촬영할 때 유용함 → 데이터 수집을 포함해서, 나중에 실제로 사용할 때 input 값으로 입력하기에 유용해보임
        
    - [MediaPipe Objectron](https://google.github.io/mediapipe/solutions/objectron#python-solution-api)
    - [MediaPipe Pose](https://google.github.io/mediapipe/solutions/pose#python-solution-api)
        
        수어 인식에 가장 많이 사용될 듯
        
        손가락 발가락까진 인식을 못하지만, 신체의 전반적인 움직임을 잘 탐지
        
        근데 예시는 전신이 전부 나온 상태로 보여줘서 어떻게 상반신(특히 팔)만 추출해서 사용할지 생각해봐야할듯
        
    - [MediaPipe Selfie Segmentation](https://google.github.io/mediapipe/solutions/selfie_segmentation#python-solution-api)
    - 등등 해당 페이지에 더 많은 기능에 대한 설명
    - ML모델 훈련을 위해 데이터를 수집하는 방법에 대한 설명도 포함
- 코드 가이드
    - [MediaPipe Face Detection Colab](https://mediapipe.page.link/face_detection_py_colab)
    - [MediaPipe Face Mesh Colab](https://mediapipe.page.link/face_mesh_py_colab)
    - [MediaPipe Hands Colab](https://mediapipe.page.link/hands_py_colab)
    - [MediaPipe Holistic Colab](https://mediapipe.page.link/holistic_py_colab)
    - [MediaPipe Objectron Colab](https://mediapipe.page.link/objectron_py_colab)
    - [MediaPipe Pose Colab](https://mediapipe.page.link/pose_py_colab)
    - [MediaPipe Pose Classification Colab (Basic)](https://mediapipe.page.link/pose_classification_basic)
    - [MediaPipe Pose Classification Colab (Extended)](https://mediapipe.page.link/pose_classification_extended)
    - [MediaPipe Selfie Segmentation Colab](https://mediapipe.page.link/selfie_segmentation_py_colab)
    
- https://github.com/google/mediapipe 이하 더 추가적으로 필요한 모든 설명(오픈소스 프로젝트) - 기술자료, 예제 등
- 웹 페이지 개발 : [https://makernambo.com/155?category=774191](https://makernambo.com/155?category=774191)