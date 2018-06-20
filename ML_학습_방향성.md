
## 머신러닝 학습 방향성 정리 

* 특징 추출: 어떤 데이터가 어떤 특징을 갖고 있는지 확인하여 벡터로 만들어야 하며, 이를 '특징 추출'이라고 한다. 

* 머신 러닝의 종류:
    1. 지도학습: 데이터와 함께 답을 입력한 뒤, 다른 데이터의 답을 예측한다. (input: Answer / output: Answer) 
    2. 비지도학습: 데이터는 입력하지만 답을 입력하지 않고, 다른 데이터의 규칙성을 찾는다. (input: ~Answer / output: Pattern)
        * 예: 클러스터 분석(Cluster Analysis), 주성분 분석(Princicpal Component Analysis), 벡터 양자화(Vector Quantization), 자기 조직화(Self Organization) 등
    3. 강화학습: 부분적으로 답을 입력하여, 데이터를 기반으로 최적의 답을 찾아낸다. (input: partial Answer / output: Answer)
        * '행동의 주체'가 '환경(상황 또는 상태)'를 관찰하여 이를 기반으로 의사결정을 내려 행동한다.
        * 행동이 변화함에 따라 행동의 주체는 어떠한 보상을 받고, 이러한 보상을 받을 수 있는 방향으로 행동을 학습하게 된다.


* 머신 러닝의 흐름:
    1. 데이터 수집
    2. 데이터 가공
    3. 데이터 학습
        1. 학습 방법 선택: 학습 알고리즘 선택 (SVM, 랜덤포레스트, k-means 등)
        2. 매개변수 조정
        3. 모델 학습
    4. 모델 평가
    5. 정밀도 검사
    
    
* 머신러닝으로 할 수 있는 것
    * 클래스 분류(Classification) - 특정 데이터에 레이블을 붙여 분류 (e.g., 스팸 메일 분류, 필기 인식 등)
    * 클러스터링 - 그룹 나누기(Clustering) - 값의 유사성을 기반으로 데이터를 그룹으로 나눈다
    * 추천(Recommendation) - 특정 데이터를 기반으로 다른 데이터를 추천
    * 회귀(Regression) - 과거의 데이터를 통하여 미래의 데이터를 예측
    * 차원 축소(Dimensionality Reduction) - 데이터의 특성을 유지하며, 데이터의 양을 줄이는 것 (계산, 메모리 절약을 위해)
    

* 초과학습(overfitting): 훈련 전용 데이터가 학습되어 있지만 학습되지 않은 새로운 데이터에 대한 예측력이 낮은 상태
    * 원인(1) 데이터가 너무 적은 경우 
    * 원인(2) 모델에 비해 문제가 너무 복잡한 경우
    
    
**알고리즘의 개념을 먼저 어느정도 이해해야 하는 것 같다.**<br>
[scikit-learn에서 제공하는 링크](http://scikit-learn.org/stable/tutorial/machine_learning_map/index.html)를 기반으로 차례대로 알아보자.
![image](http://scikit-learn.org/stable/_static/ml_map.png)

**위 웹사이트에 가면 각각의 초록색 내용을 클릭 할 경우, 이에 해당하는 개념들에 대한 설명이 나온다.**

**혹은 이런 그림**

![image](https://swalloow.github.io/assets/images/ml-diagram.png) 

일단 이 그림에서 나와 있는 알고리즘 체계로 본다면, 

1. Regression
2. Classification
3. Clustering
4. Dimensionality reduction

으로 나뉘는데, 
![image](https://swalloow.github.io/assets/images/learning-diagram.png)
으로 살펴보면,

내가 공부를 해야 할 분야는
**지도학습** 부분이 우선이다. 이 부분에서는 결국 **Regression**과 **Classification**을 알아야 한다. 

이 관점에서 보았을 때, 

**Regression**
1. Linear Regression
2. Polynomial Regression
3. Decision Trees


**Classification**
1. Random Forests
2. KNN
3. Trees
4. Logistic Regression
5. Naive-Bayes
6. SVM

의 순서로 프로젝트를 해 볼 필요가 있다. 

일단 **지도학습**의 순서를 먼저 알아야 하고 (data collection, sampling 등) 이후 두 개의 알고리즘에 맞게 적어야 한다.
