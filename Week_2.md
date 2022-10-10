#### 날짜 : 2022.10.03.~2022.10.10.
#### 논문명 : Hinton, Geoffrey E., and Ruslan R. Salakhutdinov. "Reducing the dimensionality of data with neural networks." Science 313.5786 (2006): 504-507. (Milestone, Show the promise of deep learning)

## Dimensionality reduction
- 고차원 데이터 용이하게 함
- PCA가 많이 이용됨
- autoencoder
  - encoder(고차원 데이터->저차원 데이터)와 decoder(코드를 데이터로 복구) 이용
  - reconsrtuction과 원본 데이터의 차이를 최소화하도록 훈련

- 초기 가중치가 좋은 솔루션에 가깝지 않으면 gradient descent 이용 어려움 -> “pretraining” 과정 이용
-  shallow autoencoder는 deep encoder보다 총 학습 시간이 짧고, reconstruction 오류가 많음. 그러나 매개변수가 많아지면 deep encoder의 이러한 이점이 줄어듦.
-  restricted Boltzmann machines(RBM)
- 손으로 쓴 숫자 데이터, 문서 데이터를 이용한 실험에서 autoencoder가 PCA보다 성능이 좋았음.
- layer-by-layer pretraining은 분류와 회귀에 이용될 수 있음.
- autoencoder는 현재 아주 큰 data set에 적용될 수 있게 되었음.
