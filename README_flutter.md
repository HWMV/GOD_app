# Go Dance Up App 프로젝트 (Flutter)
# Flutter UI & UX

# 1. 기능
[기능 이미지]
<img src="./images/flutter.png" width="500" height="450"/>

* 기능 : 업로드 영상 평가 , 실시간 평가, 필터링, 학습 모드
* 엔드 포인트, upload_and_evaluate (업로드 및 평가) : npy 파일로 포즈 매칭 (model: MediaPipe)
* 윤곽선 Canny model
* 필터링 : MobileNetV2(Encoder), Unet(Decoder)

[필터링 이미지]
<img src="./images/humanseg.png" width="500" height="450"/>

* 위에 이미지 처럼 분할 된 영역에 준비한 Parts 별 캐릭터 이미지 대입 예정

---

# 2. 진행 상황

홈 화면, 로그인 화면, 현재 업로드 화면, 평가 점수 출력 화면 (로그인 화면 진행중)

<디바이스 화면>
[메인 > Login > main > upload > score]
<img src="./images/main.png" width="250" height="500"/>
<img src="./images/login.png" width="250" height="500"/>
<img src="./images/upload.png" width="250" height="500"/>
<img src="./images/file.png" width="250" height="500"/>
<img src="./images/score.png" width="250" height="500"/>

---

# 3. 진행 예정

* Train.py 작성

* dataload.py & person_extraction.py : Pascal voc 2010 mat 형식의 데이터 선별 및 전처리

* 훈련 및 검증

---

# 4. 예상되는 변수

* 영상에 실시간 추적 및 대입 가능할지?
* 옷에 가려지는 부위 자세하게 Segmentatino 할지?
* 분할 된 mask 들의 랜드마크와 맞는 범위 설정 가능할지?

