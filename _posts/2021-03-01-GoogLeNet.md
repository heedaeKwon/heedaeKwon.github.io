# Going deeper with convolution

---

*1. Introduction*
*2. Related work*
*3. Motivation*
*4. Architecture*
*5. GoogLeNet*
*6. Training*
*7. Results*

---


### Introduction
---
###### 이전 연구들에서 object classification 과 detection 은 deep learining과 convolution networks에의해 향상되었습니다.
###### 이 논문은그래서 deep neural network architecture에 집중을 하였고, 새로운 모듈인 'Inception module'을 소개합니다
###### 
###### 
###### 

### Related work
---
###### Related work로는 LeNet-5 에서 시작한 convolution neural networks(CNN)과, Network in Network(NIN)이있습니다.
###### 요기서 NIN은 1x1 convolution layer를 추가합니다.
###### 이 효과로는 dimension reduction이있습니다
###### 그리고 depth와 width를 연산량 증가없이 증가시킬수있습니다
###### 
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
###### 
###### 
###### 
###### 
###### 

### GoogLeNet
---
###### 
###### 
###### 
###### 
###### 

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
