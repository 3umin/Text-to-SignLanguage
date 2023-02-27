## 수어를 애니메이션으로 구현하기 위한 모델링
- 모든 코드 및 파일은 아래에서 참조하여 사용
https://github.com/lanthaon/sl-animation-blender


### load_mp_landmark
- 가장 먼저 실행해야 할 코드
- 블렌더 위에 탭 오른쪽으로 쭉 넘기다보면 script가 있음. 그게 블렌더에서 실행할 수 있는 파이썬인데 그 창과 cmd창을 이용해 패키지 설치여부 확인필요
- load_mp 스크립트에서 사용하는 패키지가 `cv2`, `bpy`, `mediapipe`, `pathlib`인데 각각 `import`문만 한번씩 실행해보고 없는 패키지 설치


### assign_animation_to_avatar
- 스크립트에 나와있는대로, animate_avatar.blend를 복사한 뒤 복사된 파일의 파일명을 모션캡쳐파일의 파일명과 동일하게 맞춘다
- 스크립트에 나와있는대로, blend 파일을 실행 후 file >import > bvh로 모션캡쳐파일을 로드한다
- 우측상단에 Scene Collection에서 모션캡쳐파일을 복사 붙여넣기한 뒤, 스크립트에 arm_title과 arm_title_head의 이름을 모션캡쳐파일 명에 맞게 수정한다
- 코드를 실행한다
- 스크립트 내용대로, 아바타를 baking한다
- 모션캡쳐 파일을 전부 지우고, 왼쪽에 add > camera로 카메라를 추가한다
- Modeling 탭에서 카메라 위치를 캐릭터의 정면에 향하도록 수정한다
- 카메라를 추가했으면, Rendering 탭에 들어가면 뜨는 우측탭에서 인코더를 Eevee로 맞추고, Performance에서 High quality를 체크해제(렌더링 속도를 빠르게하기 위함)
- 우측 탭에서 프린트모양을 누르고 해상도를 설정한다. 그리고 Output에서 파일 경로를 설정하고, 파일 포맷으로 FFmpeg Video를 선택한다.
- 좌측상단 Render > Render Animation을 클릭한다.

- 렌더링
    - 카메라 위치는 Transform에서 좌표를 설정할 수 있으니 아래 작성된 좌표로 입력
    - 렌더링 시간을 낮추기 위한 설정
        - 안티앨리어싱 줄이기
        - 쉐이드끄기
        - Glossy 끄기
        - gravity 끄기
        - simplify 옵션들 다 0까지 낮추기
        - grease pencil 다 낮추기



    
    - 전구
    
    X : 1.89248 cm
    
    Y : -74.0159 cm
    
    Z : 188.21 cm
    
    밝기 100W
    
    - Plane Axes
    
    X : 0.65639 cm
    
    Y : -7.38562 cm
    
    Z : 129.4 cm
    
    - Camera
    
    X : -0.165564 cm    63.5243도
    
    Y : -458.853 cm    0.66004도
    
    Z : 160.176 cm    65.7911도
    
    track to plane axes 설정된 상태
