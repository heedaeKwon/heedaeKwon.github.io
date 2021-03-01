# Going deeper with convolution

---

**1. Introduction**

**2. Related work**

**3. Motivation**

**4. Architecture**

**5. GoogLeNet**

**6. Training**

**7. Results**

---



### Introduction
---
###### 이전 연구들에서 object classification 과 detection 은 deep learining과 convolution networks에의해 향상되었습니다.
###### 이 논문은그래서 deep neural network architecture에 집중을 하였고, 새로운 모듈인 'Inception module'을 소개합니다



### Related work
---
###### Related work로는 LeNet-5 에서 시작한 convolution neural networks(CNN)과, Network in Network(NIN)이있습니다.
###### 요기서 NIN은 1x1 convolution layer를 추가합니다.
###### 이 효과로는 dimension reduction이있습니다
###### 그리고 depth와 width를 연산량 증가없이 증가시킬수있습니다

![logo]()



### Motivation 
---
###### motivation 이 이루어진 과정을 보면
###### 먼저 좋은 performance를 보여주려면 size와 depth를 증가시겨야합니다.
###### 그렇게 되면 2개의 주된 결함이 생기는데 
###### 먼저 첫번째는 parameters이 엄청많아지는 것입니다.
###### 그리고 overfitting현상도 일어날 확률이 높아집니다
###### 두번째는 computational resources양이 어마어마하게 증가하는 것입니다
###### computational budget은 한정이 되어있기 때문에 효율적으로 써야하기때문에
###### 이 resources양을 줄여야합니다
###### 그래서 이 두 문제를 해결할 근본적인 방법인 sparsity 를 소개하고 fullyconnected layers를 sparse ones로 교체하는것입니다



### Architecture
---
###### Inception module은 다음과 같이 생겼습니다.

![logo]()

###### 이렇게 1x1 ,3x3 ,5x5로 다양한 결과를 이용하여서 Feature map을 효과적으로 추출하려고 했습니다.
###### 근데 5x5와같은 비싼 연산에 많은 필터가쌓이면 연산량이 많아지게 되므로 두번째 idea가 나왔습니다

![logo]()

###### 이것은 비싼연산인3x3,5x5에 많은 양이 들어가기 전에 1x1 conv로 필터수를 줄이게되는 것입니다. 
###### 그렇게 함으로써 size와 depth를 늘려도 연산량이 줄어들게 될 수 있습니다.



### GoogLeNet
---

![logo]()

###### GoogLeNet은 다음과 같이 구성되어있습니다.
###### 아까 말했던 inception module을 여러개 합쳐서 한 것인데
###### 중간에 보시면 softmax layer가있습니다.
###### 이유는 이 구조가 깊게 형성되어있다보니 gradient vanishing현상이 일어날 수도 있기 때문에
###### 중간에 classifier를 넣은 것입니다.

![logo]()
###### 다음은 전 구조를 표를 이용해서 표현한 것인데 #3x3 reduction,#5x5 reduction을 보시면 채널수가 적은것을 확인할 수 있습니다.



### Training
---
###### 
###### 
###### 
###### 
###### 



### Results
---
###### 
###### 
###### 
###### 
###### 
