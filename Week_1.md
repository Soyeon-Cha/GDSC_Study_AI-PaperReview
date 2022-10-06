##### 날짜: 2022.09.26.~2022.10.03.
##### 논문명: LeCun, Yann, Yoshua Bengio, and Geoffrey Hinton. "Deep learning." Nature 521.7553 (2015): 436-444. [pdf] (Three Giants' Survey)
##### 논문소개: Deep Learning 기술에 대한 review 논문
##### 논문 선정 이유 : 인공지능 관련 논문을 제대로 읽어보는 것이 처음이라 다른 기술보다 익숙한 딥러닝을 주제로 하는 이 리뷰 논문을 선택했다.

- Deep learning
  - representation learning
  - engineering by hand 부분이 적어 더 큰 양의 계산과 데이터를 다룰 수 있게 함
- Supervised learning
  - 가중치와 그에 따른 gradient vector 이용
- Backpropagation to train multilayer architectures
  - 모듈이 상대적으로 smooth functions이면 backpropagation procedure로 gradient 계산 가능
- Convolutional neural networks
  - 여러 배열 형태의 데이터 처리
  -  convolutional layer : 특징의 local conjunction을 탐지함
  - pulling layer : 의미적으로 비슷한 특징을 하나로 합침
- Image understanding with deep convolutional networks
  - 얼굴 인식, 자율 이동 로봇, 자율주행 자동차 기술과 관련됨
- Distributed representations and language processing
- Recurrent neural networks
  - 다음에 올 텍스트를 예측하는 데에 탁월
  - LSTM network : RNN보다 더 긴 시간 동안 정보 저장함
- The future of deep learning
  - 인공지능은 representation learning과 complex reasoning이 합쳐진 시스템을 통해 크게 발전할 것이라고 봄

backpropagation에 대해 기울기로 설명하는 부분이 있는데 saddle point 같은 모르는 개념도 있었고 이해하지 못했다. 다른 논문을 통해 다시 접해보려 한다.


###### 용어
- backpropagation algorithm(역전파 알고리즘) : 다층(multilayer)이고, 순행 공급(feedforward) 신경망에서 사용되는 학습 알고리즘이며, 학습 방법은 지도 학습(supervised learning) (출처:실험심리학용어사전)
- deep convolutional network
- recurrent neural network(RNN, 순환신경망)
- representation learning
- supervised learning (지도 학습)
- stochastic gradient descent(SGD)
- linear classifier(선형 분류기)
- rectified linear unit(정류 선형 유닛, ReLU)
- convolutional neural network(ConvNet)
- saddle point(안장점)
