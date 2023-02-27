# Text to Sign Language

- [http://www.causw.com/capstone/86](http://www.causw.com/capstone/86)
    
    Text to sign language by avatar animation을 정확하게 구현한 예제
    
    각 수화 동작을 아바타 애니메이션으로 구현한 다음, 정해진 문장(단어)의 순서에 맞추어 동작 진행하는 방법
    
    감성분석을 이용해 캐릭터의 배경 색이 바뀌어 해당 문장의 감정을 간접적으로 표현
    
    결과적으로 모델을 만든다는 느낌이 아니라 형태소 분석을 통해 번역하려는 문장의 단어만 추출한 뒤, 데이터베이스와 매칭해서 해당하는 수어 동작을 아바타 기능에 맞추어 구현하게 만듬
    
    한계점 : 수화를 단순히 한글 자음, 모음, 숫자에 대응하는 동작만 만들어서 각 단어가 나올 때 계속 자음 모음 조합으로 구현됨
    
    - [https://www.wenyanet.com/opensource/ko/6112508fb4d0cb7c9f2776fa.html](https://www.wenyanet.com/opensource/ko/6112508fb4d0cb7c9f2776fa.html)
    - [https://github.com/lanthaon/sl-animation-blender](https://github.com/lanthaon/sl-animation-blender)
        
        위의 한계점에 대응(둘이 같은 내용임)
        
        mediapipe를 통해 영상을 모션캡쳐 한 다음 그 모션을 아바타로 구현
        
        이 방법을 활용하게 된다면 수화 번역하는 애들이 사용하는 데이터와 동일한 데이터로 각 단어의 모션까지 구현하는 모델을 만든 다음,
        
        입력된 문장의 단어 순서대로 아바타의 동작을 출력하는 코드를 짜면 될 것
        
        [Blender](https://www.notion.so/Blender-f6fb86b2d2b14bc2833321d36bcc6b84)
        
        [데이터베이스](https://www.notion.so/e0505db0718f41a8a7cfce8f8ee93982)
        
    - [https://github.com/homuler/MediaPipeUnityPlugin](https://github.com/homuler/MediaPipeUnityPlugin)
        
        만약 위 mediapipe 모션캡쳐를 할 때 블랜더가 아니라 유니티를 사용한다면, 이걸 사용하면 됨