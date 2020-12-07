## :clipboard: 논문의 정보를 알려주세요.
- Predicting Infectious Disease Using Deep Learning and Big Data
- Sangwon Chae,Sungjun Kwon and Donghyun Lee
- MDPI
- Published: 27 July 2018

## :page_with_curl: Abstract(본문)
- 질병관리본부는 감염병 전염을 최소화하기 위해 감시시스템을 운영하고 있음 
- 하지만 보고 누락과 지연으로 인해 감염병에 대한 즉각적인 조치가 어렵고 전염병 동향도 알려지지 않아 예측이 쉽지 않음
- 본 연구는 소셜 미디어 데이터를 포함한 빅데이터를 고려하면서 딥러닝 알고리즘의 파라미터를 최적화하여 감염병을 예측하는 모델을 만들고 비교

> Infectious disease occurs when a person is infected by a pathogen from another person or an animal. It is a problem that causes harm at both individual and macro scales. The Korea Center for Disease Control (KCDC) operates a surveillance system to minimize infectious disease contagions. However, in this system, it is difficult to immediately act against infectious disease because of missing and delayed reports. Moreover, infectious disease trends are not known, which means prediction is not easy. This study predicts infectious diseases by optimizing the parameters of deep learning algorithms while considering big data including social media data. The performance of the deep neural network (DNN) and long-short term memory (LSTM) learning models were compared with the autoregressive integrated moving average (ARIMA) when predicting three infectious diseases one week into the future. The results show that the DNN and LSTM models perform better than ARIMA. When predicting chickenpox, the top-10 DNN and LSTM models improved average performance by 24% and 19%, respectively. The DNN model performed stably and the LSTM model was more accurate when infectious disease was spreading. We believe that this study’s models can help eliminate reporting delays in existing surveillance systems and, therefore, minimize costs to society.

## :mag_right: 사용한 데이터를 적어주세요
### 검색데이터
- 네이버 데이터랩(https://datalab.naver.com/keyword/trendSearch.naver)
- 인터넷트렌드(2017년 상반기 보건의료 분야 검색엔진 http://internettrend.co.kr/trendForward.tsp)
### 기상데이터
- 기상청 기상정보 공개포털(https://data.kma.go.kr)
### 감염병 데이터
감염병 웹통계시스템(https://is.cdc.go.kr/dstat/index.jsp)

## :key: 핵심 키워드를 적어주세요.
- infectious disease prediction; deep neural network(DNN); long short-term memory(LSTM); deep learning; social media big data

## :paperclip: URL
- [Predicting Infectious Disease Using Deep Learning and Big Data](https://www.mdpi.com/1660-4601/15/8/1596/htm)

--------------------------------------------------------------

## :bulb: 방법은 무엇입니까?
- 모델 : OLS, ARIMA 전통예측모델과 DNN, LSTM 딥러닝 예측모델
- 최적화기 : Adadelta, Adagrad, Adam, Adamax, Nadam, RMSprop, SGD
- 평가 : RMSE

## :chart_with_upwards_trend: 실험과 그 결과는 어떻습니까?
### 실험
DNN, LSTM, ARIMA, OLS 방법을 사용하여 설계된 모델의 데이터 수집 프로세스와 비교

<img src = "https://github.com/gmksf99/Review_thesis/blob/main/img/0.png" width = "300px"/>

각 감염병에 대해 15개 회귀 모형의 수정된 R 제곱 값
관측된 회귀 모형 중에서 모든 변수의 조합인 모형이 가장 좋은 설명력을 가지고 있음

<img src = "https://github.com/gmksf99/Review_thesis/blob/main/img/1.png" width = "300px"/>

수두에 대한 모든 DNN과 LSTM 예측 모델 중 RMSE가 가장 낮은 최적 모델은 ARIMA 모델보다 각각 27.22%, 27.33%의 높은 성능을 보였다. 수두 DNN 상위 10개 모델은 평균 24.45%의 성능을, LSTM 모델은 평균 18.78%의 성능을 개선했다.

성홍열에 대한 DNN과 LSTM 예측 모델의 최저 RMSE는 ARIMA 모델에 비해 26.25%, 23.79%의 개선된 성능을 보였다. 성홍열 상위 10개 DNN 모델은 평균 23.28%의 성능을 개선했다. LSTM 모델은 성능을 평균 17.97% 향상

### 결과
딥러닝을 채용한 감염병 예측모델을 활용해 기존의 감염병 감시체계를 보완하는 동시에 감염병 동향을 예측할 수 있을 것이다. 또한 이를 통해 감염병 동향을 즉시 알 수 있도록 보고체계의 시간차를 줄일 수 있다면 감염병에 대한 즉각적인 대응이 가능해지고 사회에 대한 비용을 최소화할 수 있을 것으로 기대된다.

## :black_nib: 차후 연구방향 및 보완점은 무엇입니까?
- 한계점 : 상대적으로 짧은 데이터 수집 기간, 지역적으로 결합된 예측, 딥러닝 모델에서 좁은 범위의 매개변수
- 향후 연구방향 : 더 많은 매개변수를 고려하고 더 많은 예측 모델을 만들면 예측 성능을 어느 정도 높일 수 있을 것이다.

## :thumbsup: novelty와 논문을 통해 배운 것은 무엇입니까?
해당 논문을 통해 어떤 점을 새롭게 알게 되었는지 적어주세요.

## :loop: 궁금한 점이나 추가로 읽으면 좋은 레퍼런스가 있습니까?
추가적으로 궁금한 사항에 대해서 적어주세요.
같이 읽으면 좋은 레퍼런스의 제목과 URL을 덧붙혀주세요.

-----------------------------------------------------------------

## :star2: 참조
[논문 리뷰 양식](https://github.com/koptimizer/my_PaperLog/blob/master/review_form.md)
