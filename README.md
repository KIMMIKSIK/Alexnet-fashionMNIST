# Alexnet-fashionMNIST

<br />
<img src="https://meme2515.github.io/neural_network/images/alexnet_1.png" style="width: 505px" />


# 🛠 코드 설명

<br />

 인공지능2 과제를 통해 Alexnet을 사용한 코드를 처음 구현해 보았습니다. fashionMnist데이터를 사용하여 10개의 레이블을 분류하는 모델을 생성하였는데 pytorch에서 기본적으로 제공하는 api를 통해 간편하게 데이터를 가져올 수 있었습니다. train_data 6만개, test_data 3만개 중 실제 모델 학습 과정에서는 절반만 사용하여 train 3만, test 1.5만의 데이터를 사용하였습니다. 32의 크기로 미니배치를 나누었으며 학습에 사용한 데이터 수로는 약 5회 정도의 epoch가 넘어가면서 과적합이 조금씩 발생되는 것으로 보아 7회로 설정하였습니다. Alexnet의 input 이미지의 크기들은 입력에 들어가기전 모두 image transforms을 적용하여 (3, 227, 227)크기로 설정하였습니다. optimizer의 경우 최근 가장 성능이 좋다고 하는 Adam을 사용하였고 그와 함께 loss function의 경우 multi-classificationd을 위한 crossEntropy를 사용하였습니다. 최종적으로 evaluation loss: 0.25391, evaluation accuracy: 0.90540, 약 90프로의 정확도를 보여주며 좋은 결과를 확인하였습니다.

<br />

# 🙋‍♀️ 느낀점

<br />

 처음에는 visual studio를 통한 jupyter notebook으로 코드를 작성하였습니다. 생각보다 시간이 오래걸리고 복잡한 작업이라는 것을 깨닫고 코랩을 통해서 gpu로 코드를 작동했는데 속도가 훨씬 향상되는 것을 느낄 수 있었습니다. 지금까지 gpu를 사용하는게 훨씬 유리하다는 것은 알고 있었지만 이렇게 직접 비교해 볼 수 있었던 경험은 처음인 것 같습니다. pytorch를 사용한 코드 구현 경험이 있어서 생각보다 어렵지는 않았지만 이미지를 다루다보니 input 이미지 채널 갯수 조정을 잘못해서 에러가 발생하는 사건으로 조금 당황하였습니다. 검색을 통해 다른 코드와 비교하면서 Alexnet에 대해서 좀 더 깊게 생각하고 구조를 이해할 수 있었던 시간이었던 것 같습니다. 확실히 코드를 작성하면서 실습해보니까 이론으로 배우는 것보다 전체 과정을 한번씩 경험해 볼 수 있어서 너무 좋은 시간이었던 것 같습니다.  
