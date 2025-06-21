스탠포드 개 품종 분류기 🐶

임재서 / 한양대학교 정보공학과

본 프로젝트는 Stanford Dogs Dataset에 포함된 120가지의 강아지 품종을 자동으로 식별하는 딥러닝 모델을 개발한 것입니다. 사전 학습된 EfficientNet-B0 모델을 기반으로 전이 학습(Transfer Learning)을 적용하였으며, 모델 학습, 평가, 예측까지 전 과정을 구현했습니다.

📁 포함된 파일

2020069852_video.mp4
Git LFS를 통해 업로드된 영상으로, 프로젝트 구조와 실행 결과를 요약 설명합니다.

2020069852_dogs_classifier.ipynb
데이터 전처리, 학습, 평가 및 예측을 포함한 전체 코드

2020069852_ppt.pdf
프로젝트 요약 발표 자료 (PPT 기반 PDF)

📊 프로젝트 요약

데이터셋: Stanford Dogs Dataset
데이터 다운로드 링크
모델: EfficientNet-B0 (Pretrained) + Transfer Learning
분류 대상: 총 120개의 강아지 품종
📌 코드 구조 요약 (ipynb)

블록	내용
1	라이브러리 임포트 및 파라미터 설정 (디바이스, 하이퍼파라미터 등)
2	.mat 파일을 로드하고 DataFrame으로 변환하는 함수 정의
3	학습용 및 테스트용 DataFrame 생성
4	커스텀 클래스 정의 (이미지 크롭, 전처리 포함)DogBreedDataset
5	이미지 변환 규칙 정의 (데이터 증강 포함)
6	Dataset 및 객체 생성DataLoader
7	모델 정의 (EfficientNet-B0 불러오기 및 수정), 손실 함수 & 옵티마이저 설정
8	학습 및 평가 함수 정의
9	메인 학습 루프 및 학습/평가 결과 시각화
10	학습된 모델 가중치 저장
11	단일 이미지에 대한 품종 예측 수행 및 시각화
✨ 주요 특징
PyTorch 기반 학습 파이프라인
EfficientNet을 이용한 고성능 전이 학습
Git LFS를 활용한 대용량(>100MB) 영상 파일 관리
작성자: 임재서
소속: 한양대학교 정보공학과
