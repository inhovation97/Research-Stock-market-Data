# Research-Stock-market-Data
🔍Research Stock market Data as undergraduate research student   
#### [안홍렬]()교수님 지도하에 교내 DSML 연구센터에서 학부연구생으로서 주가 데이터에 대한 연구를 진행.   
#### 데이터는 [finance data 라이브러리](https://financedata.github.io/posts/finance-data-reader-users-guide.html#)를 이용함.    
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 논문 게재를 목표로 연구를 진행 [[code]](https://github.com/inhovation97/Research-Stock-market-Data/tree/main/code)   
> 2022.03 ~ 
> 데이터 속 잡음이 너무 많아 추론의 어려움을 겪었지만, 여러 조건들을 걸어가며 얻어 낸 인사이트를 통해 연구 방향을 잡음.   

#### 어떤 기업의 10일간의 주가 정보를 통해 다음날 종가가 상승할지 하락할지 이진 분류를 하는 모델을 연구한다.   
![image](https://user-images.githubusercontent.com/59557720/164187413-4b6d85fd-45fc-41fe-8150-4f94947d479a.png)

#### 이 과정에서 기업마다 액면가가 전부 다르며 시계열적인 특성을 가진 점에 초점을 맞추어 4가지 방식의 스케일링 고안하여 이를 비교함.   
1. [데이터 수집과정](https://inhovation97.tistory.com/54)   
2. [EDA 과정](https://inhovation97.tistory.com/59) -> 코넥스 기업 존재를 발견하여 종목 코드 선정 방식을 다시 고려   
3. [4가지 스케일링을 정의하여 비교](https://inhovation97.tistory.com/60) -> 논문의 주제로 선정   
4. [모델링 과정에서 데이터 불균형 문제를 해소함](https://inhovation97.tistory.com/61)   




## Stage 1,2
> 2022.01.03 ~ 2022.02.28   
> 교수님이 주신 과제를 수행하면서 피드백을 받고 수정함.   

<진행 절차>   
1. 서버PC를 이용하기 위한 리눅스 사용법을 익힘.   
2. 프로그래밍적 사고에 대한 피드백을 받고 과제를 수행함   
   -> "데이터 프레임의 사용을 최소한으로 변수명을 명확히하며 각 개체를 순차적으로 처리하는 간결하고 가독성 높은 코드를 지향"
3. 시간 복잡도를 줄이기위한 멀티 프로세싱을 이용.   
4. mysql을 통해 서버에 DB를 생성하여 데이터를 저장.
5. 본격적인 연구를 위한 기본적인 modeling   

+ sql을 이용하여 데이터베이스에 데이터를 올리는 방법을 경험.   
+ [멀티 프로세싱](2022-01-10_assignments_on_feedback.ipynb)을 이용하여, 5분 -> 10초로 시간 복잡도를 크게 줄이는 것을 경험.   
+ 해당 과정에서 [LSTM을 이용하여 주가 상승 여부를 예측](https://github.com/inhovation97/Research-Stock-market-Data/blob/main/stage1/2022-01-18_trying_lstm.ipynb)해보았지만 실패 
  -> 파이토치를 이용하여 시계열 모델 RNN 모델링을 경험, 데이터 퀄리티로 인해 전혀 수렴이 안되는 것을 경험.   
