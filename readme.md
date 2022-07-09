# Image Classfication

# 데이터 다운로드 방법
URL:
https://www.kaggle.com/datasets/alessiocorrado99/animals10

1. 위 URL에서 animal dataset을 다운로드하고 압축해제한다.
2. 폴더 안에 아래 구조 처럼 "raw-img" 폴더만 추가한다. (translate.py 파일은 들고 올 필요 없습니다)

```
classfication
├── raw-img
│   ├── cane
│   ├── cavallo
│   └── ...
|
├── class.py
├── split.py
└── translate.py
``` 

# 데이터 전처리 방법

1. cv2, numpy 설치

``` 
pip install opencv-python, numpy
``` 
2. split.py 실행

``` 
python split.py
``` 

3. 최종 폴더 구조

- classfication 폴더 안에 train_img 와 test_img 폴더가 생기면 됩니다.


# Task!!
pytorch 또는 tensorflow로 동물들을 구분할 수 있는 파이프라인을 만들고 전처리된 testset에 대해서 어느 정도의 성능이 나오는지 지표도 기입해주세요.

TODO:
1. 전체적인 파이프라인 코드 구현
2. trainset으로 인공지능 모델 학습
3. testset에 대한 평가 (metric은 accuracy, recall, precision, f1-score 등 confusion matrix에서 쓰는 지표 중 1개 이상 값을 내면 됩니다.)
