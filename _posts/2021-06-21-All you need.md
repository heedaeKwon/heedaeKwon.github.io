# *Attention is All You Need*

---

### *Introduction*

##### 이전 연구들은  RNN모델로 리커런트한 작업으로 수행을 하였습니다.
##### 이것은 한 단어를 넣는 방식으로 시퀀스에 포함되어있는 순서정보를 정렬하고
##### 반복적으로 넣어서 히든스테이트 값을 갱신시키는 방식이었습니다.
##### 그런 경우 시퀀스의 길이토큰 개수만큼 뉴어럴 네트워크에 넣어야 하기떄문에
##### 병렬적 처리가 불가능하여 문장의 길이가길어지면 그 길이만큼 능력을 수행해야하는 
##### 문제가 있습니다. 그래서 어텐션메커니즘과 같이 사용하여서 보다 효율적으로 
##### 출력단어를 만들 수 있지만 여전히 리커런트 특성으로인한 시퀀스 길이의 제약이 존재하였습니다.

##### 그래서 이 논문은 리커런스한 특성자체를 제거아고 어텐션 메카니즘만을 활용하여 한번의 행렬곱으로
##### 위치정보를 한번에 처리하였고 그렇기에 병렬처리가 가능해져서 기존의 문제점이였던
##### 시퀀스 길이에 대한 제약이 사라져서 좋은 성능이 나왔습니다.

---

### *Model Architecture*

##### 다음은 이 모델의 아키텍쳐입니다

![logo](https://user-images.githubusercontent.com/68374734/122783520-9b076500-d2ec-11eb-8c96-5e8a1e4af966.PNG)

##### 이 아키텍쳐는 전에 인코더 디코더의 기본적 구조는 사용을 하였고 앞서 말했던 리커런트한 특성은 이용하지 않고
##### 오직 어텐션 메커니즘만을 이용하였습니다.


