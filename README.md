# emotion_detect_ML

## 목적

Kaggle의 얼굴 표정 Emotion Detection으로 진행한 머신러닝 학습 프로젝트입니다.

## 접근  

총 7가지 감정으로 행복, 혐오, 슬픔, 분노, 놀람, 두려움, 무표정으로 분류하는 것이 목적입니다.

데이터 증강과 오버샘플링을 활용하여 다양한 모델을 학습한 뒤 가장 성능이 우수한 3개의 모델을 선정하여 앙상블 기법을 적용했습니다.

학습에서 사용한 모델은 kaggle에서 좋은 결과를 보였던 CNN , DenseNet, VGG, ResNet, AlexNet를 선정

모델의 성능이 Top-3 였던 DenseNet , ResNet, VGG를 학습때 찾았던 HyperParameter를 기반으로 앙상블 기법 수행 / Soft Voting 방식 사용


![image](https://github.com/user-attachments/assets/20d8398f-148d-41a5-a9a8-6c5054c53ab6)

![image](https://github.com/user-attachments/assets/2243705c-3b13-40ef-814f-9e6fb14a9850)

Accuracy: 0.659

Top-2 Accuracy: 0.8183 

으로 가장 잘 나왔던 단독 모델 ResNet의 Accuracy 0.6272 보다 우위였다는 것을 알 수 있었습니다.

해당 데이터 세트는 아래에서 보실 수 있습니다.

https://www.kaggle.com/datasets/ananthu017/emotion-detection-fer/suggestions?status=pending&yourSuggestions=true

더 자세한 보고서 자료는 아래에 첨부합니다.

[20250217145508_9882487311845.pdf](https://github.com/user-attachments/files/18821960/20250217145508_9882487311845.pdf)









--------------------------------------
### TODO
- 서영
    - 모델 최적 hyperparameter로 학습하기
    - DensNet, CNN, VGG, ResNet, AlexNet
    - 최종 val accuracy는 50 +- 로 나와야 함, 결과가 20~30선 이라면 뭔가 잘못된 것
---
- 준혁
    - 모델 학습 결과 중 최적 3개 골라 ensemble
    - soft voting 방법으로 구현
    - 학습 시키기
---
- 보길
    - 위에서 나온 모델을 test set에서 시험하기
    - precision, recall, roc curve, f1_score, confusion matrix, learning curve 등
    - 다양한 지표 보여주기
 --- 

---------------------------------


