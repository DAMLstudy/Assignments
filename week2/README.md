# 2주차 과제
## Machine Learning With Iris Dataset
### Problem 1 : scikit-learn 내장 dataset 가져오기

---------------------------------------
 * [ 참고 ] Iris dataset의 구성
    * target_name : 예측하려는 값(class)을 가진 문자열 배열
    * target : Label(출력 데이터)
    * data : Feature(입력 변수)
    * feature_names : 입력 변수 각 항목의 이름
    * DESCR : 데이터셋에 대한 설명
---------------------------------------

(1) scikit-learn은 머신러닝 모델을 테스트하기 위한 데이터셋을 제공한다. 아래의 패키지와 함수를 이용하여 iris 데이터셋을 가져오세요. 
  - 패키지 : sklearn.datasets
  - 함수 : load_xxxx()

(2) keys()함수로 dataset의 key 값들을 출력하세요.
  - Answer  
```python
irisData의 키 :  dict_keys(['data', 'target', 'frame', 'target_names', 'DESCR', 'feature_names', 'filename'])
``` 
(3) dataset의 target 이름을 출력하세요.
  - Answer  
```python
타깃의 이름 : ['setosa' 'versicolor' 'virginica']
``` 
(4) dataset의 feature 이름을 출력하세요.
  - Answer  
```python
특성의 이름 : ['sepal length (cm)', 'sepal width (cm)', 'petal length (cm)', 'petal width (cm)']
``` 


### Problem 2 : Pandas DataFrame으로 구성
다음과 같이 데이터프레임을 생성 후 출력하세요.
 - Answer
 
![ans1](https://user-images.githubusercontent.com/90343268/134770341-0babbef2-effb-4b49-9c40-d337419f89c8.png)


### Problem 3 : 머신러닝 구현
(1) scikit-learn의 함수를 이용하여 Iris dataset을 분할하고 train data와 test data의 크기를 출력하세요.
  * train data와 test data의 비율 = 8 : 2
  - Answer  
```python
((120, 4), (30, 4), (120,), (30,))
# (X_train, X_test, y_train, y_test)
``` 
  
 (2) 모델 생성 및 학습 - 자신이 원하는 하나의 모델을 선택(생성)하여 모델을 학습시키세요.
   - Example answer  
```python
DecisionTreeClassifier()
# Try yourself
``` 

 (3) 평가 - Accuracy를 기반으로 모델을 평가해보세요.
   - Example answer  
```python
훈련 데이터 정확도 :  1.0 테스트 데이터셋 정확도 :  0.9666666666666667
# Try yourslef, your own result
``` 
 
