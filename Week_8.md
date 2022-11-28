날짜 : 2022.11.21.~2022.11.28.
논문명 : Simonyan, Karen, and Andrew Zisserman. "Very deep convolutional networks for large-scale image recognition." arXiv preprint arXiv:1409.1556 (2014).

- 대규모 이미지 인식 설정에서 컨벌루션 네트워크 깊이가 정확도에 미치는 영향 연구
  - 깊이에 따른 네트워크 평가


#### ConvNet Configuration
- Architecture
- Configuration
  - 모든 구성은 일반 설계를 따르고 깊이만 다름
  - 여기서의 net는 더 크지만 얕은 net보다 작은 가중치를 가짐
- Discussion
  - 기존의 것과 달리 첫 번째 conv layer에 큰 receptive field를 사용하는 대신 전체 net에 작은 3*3 receptive field 사용
  - layer를 1개가 아니라 3개를 합해서 사용함으로써 구별이 더 쉽게 만듦
  - 매개 변수를 줄임

#### Classification Framework
- Training
  - andom initialization을 통한 훈련 없이 가중치 초기화 가능
- Testing
  - 자르지 않은 이미지를 여러 배율로 학습하고 평가
- Implementation Details
  - 다중 GPU 훈련


#### Classification Experiments
- Single Scale Evaluation
  - A-LRN network를 사용하는 것은 normalization layer 없이 model A에서 개선되지 않음
  - A의 layer에서 ConvNet depth가 증가함에 따라 분류 오류가 감소
  - 훈련 시간에 있어 scale jittering은 가장 작은 면이 고정된 이미지로 훈련시키는 것보다 더 좋은 결과를 만듦
- Multi-Scale Evaluation
- Multi-Crop Evaluation
- ConvNet Fusion
- Comparision with the State of the Art


#### Conclusion
- representation depth는 분류 정확도에 기여함
