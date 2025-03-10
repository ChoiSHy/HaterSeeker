# 혐오표현 감지 시스템

## 다먹자 프로젝트에서 혐오 표현을 검수하는 기능을 구현하기 위한 시스템입니다.
* 다먹자 프로젝트: https://github.com/ChoiSHy/project_LetsEatAll
* PyTorch를 통해 Deep-Learning 모델을 만들어 혐오표현을 감지해 리뷰 생성에 제한을 둠
* beomi/KcELECTRA-base-v2022 모델을 이용해 학습함
* 과정 Client(Review 저장 요청) --> Spring api server(AWS EC2) --> Fast api server (Local, 리뷰 혐오표현 판단) --> Spring api server(AWS EC2, 데이터 저장) --> Client(결과 전달)

* 현재 모델 파일은 용량이 너무 커 github에선 내려간 상태입니다.
