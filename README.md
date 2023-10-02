# Alexnet-fashionMNIST

<br />
<img src="https://meme2515.github.io/neural_network/images/alexnet_1.png" style="width: 505px" />


# 🛠 코드 설명

<br />

 인공지능2 과제를 통해 Alexnet을 사용한 코드를 처음 구현해 보았습니다. fashionMnist데이터를 사용하여 10개의 레이블을 분류하는 모델을 생성하였는데 pytorch에서 기본적으로 제공하는 api를 통해 간편하게 데이터를 가져올 수 있었습니다. train_data 6만개, test_data 3만개 중 실제 모델 학습 과정에서는 절반만 사용하여 train 3만, test 1.5만의 데이터를 사용하였습니다. 32의 크기로 미니배치를 나누었으며 학습에 사용한 데이터 수로는 약 5회 정도의 epoch가 넘어가면서 과적합이 조금씩 발생되는 것으로 보아 7회로 설정하였습니다. Alexnet의 input 이미지의 크기들은 입력에 들어가기전 모두 image transforms을 적용하여 (3, 227, 227)크기로 설정하였습니다. optimizer의 경우 최근 가장 성능이 좋다고 하는 Adam을 사용하였고 그와 함께 loss function의 경우 multi-classificationd을 위한 crossEntropy를 사용하였습니다. 최종적으로 evaluation loss: 0.25391, evaluation accuracy: 0.90540, 약 90프로의 정확도를 보여주며 좋은 결과를 확인하였습니다.

<br />

# 🙋‍♀️ 느낀점

<br />

 인공지능2 
