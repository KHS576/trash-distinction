# 명문나루

## 팀 소개

|  이름  |  역할  | GitHub Profile |
|--|--|--|
| 최주희 |  팀장  | https://github.com/cjh820
| 김의환 | 설계자(부팀장) | https://github.com/Uihwan12
| 정지성 |  프로그래머 | https://github.com/megarail
| 김희수 |  엔지니어  | https://github.com/KHS576

## 프로젝트 개발 이유
주거 침입 범죄는 전 세계적으로 중요한 사회 문제 중 하나 입니다. 특히, 빈 집에 침입하여 범죄를 저지르거나, 밤늦은 시간에 주택에 침입하려는 사건이 사건들이 발생하고 있습니다. 이는 주민들의 안전을 위협하고 불안감을 초래합니다. 물체 감지 기술과 알람 시스템을 활용하여 집의 보안을 강화하고 안전성을 높이기 위해 이 프로젝트를 기획하게 되었습니다.


## 프로젝트 개요

>프로젝트 이름: 안전 경보 시스템 


주요 기능:

사람 판별-웹캠을 이용해 사람을 인식

소리 센서 작동- 사람을 인식하면 경보음이 울림

![시스템 구조](https://github.com/KHS576/trash-distinction/blob/main/group_photo.png)

https://www.youtube.com/watch?v=c6BtrwxBb4A

https://www.youtube.com/watch?v=r4ctN6aEg7s

## 실행 방법

라이브러리 설치 

%pip install pygame
%pip install -q "openvino>=2024.0.0" "nncf>=2.9.0"
%pip install -q "torch>=2.1" "torchvision>=0.16" "ultralytics==8.3.0" onnx tqdm opencv-python --extra-index-url https://download.pytorch.org/whl/cpu

VIDEO_SOURCE = "person2.mp4"에서 파일 이름을 자신이 원하는 파일로 변경후 디바이스 실행, 
    run_object_detection(
    source=VIDEO_SOURCE,
    flip=True,
    use_popup=True,
    model=det_ov_model,
    device=device.value,
    # video_width=1280,
)

