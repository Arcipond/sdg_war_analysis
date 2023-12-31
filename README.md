# 전쟁과 지속가능한 발전

## 운정고등학교 2023 1학기 자율교육과정

![](res/sdg.png)

## I. 도입

최근 전세계 전쟁에 대해 사람들의 주의가 상승하였다. 그러나 지속되는 전쟁의 노출은 전쟁을 무덤덤하게 받아들이게 하였고, 또한 국가들의 이해관계로만 세계를 바라보는 관점을 증가시켰다. 전쟁이 지속 가능한 발전의 17가지 목표에 어떠한 상관관계가 있는지 분석하고 더 나아가 어떠한 방향으로 지속 가능한 발전을 추구할 수 있을 지를 분석한다.

## II. 사용 데이터 & 라이브러리

### 사용 데이터

    https://www.kaggle.com/datasets/prasertk/historical-commodity-prices-from-20002022

    Major commodity price(2000-2002) by Prasert Kanawattanachai

    포함된 commodity : Gold, Palladium, Nickel, Brent Oil, Natural Gas, Wheat

    그러나 Wheat가 전세계 빈곤/식량과 밀접하게 연관되어있기에 Wheat를 중점적으로 살펴볼 것이다.

    https://www.kaggle.com/datasets/nathaniellybrand/los-angeles-crime-dataset-2020-present
    LA 범죄 집계

### 사용 라이브러리

- Pandas
- Numpy
- Matplotlib : 시각화
- 

## III. 데이터 분석 과정

### 연도에 따른 밀 가격 시각화

![](res/plot1.png)

    위의 이미지는 2015년 1월 1일부터 2022년 4월 8일까지의 밀 가격 변화(USDPT)를 그래프상으로 표현한 것이다.

    러-우 전쟁이 발발한 2022년 2월 이후 급격히 치솟은 것을 확인할 수 있다.

![](res/plot2.png)


### 국가별 밀 생산량 시각화(2016년)

![](res/plot3.png)

2016년 기준 지도를 보면 러시아와 우크라이나가 전세계 밀 생산량에 상당한 기여를 하는 것을 볼 수 있다. 따라서 우크라이나 전쟁에 의해서 우크라이나와 러시아의 밀 생산량은 감소했으며 그에 따른 식량에 대한 위협이 가격을 상승시켰다.

### 범죄 집계수와 밀 가격 상승의 관계

![](res/plot4.png)

위 그래프를 보면 밀 생산량이 증가하는 2022년에 범죄율이 증가했음을 볼 수 있다. 상관계수는 **0.352261**로 낮은 상관관계가 있음을 알 수 있다.

### 선형 회귀 분석(sklearn)

![output](res/output1.png)

score = 0.20512625378837623

## ARIMA 시계열 데이터 선형 회귀 분석

![](res/output2.png)

aic = 2764.5130360428975

## VI. 정리

  파이썬 데이터 시각화 과정을 통해 간단하게 전쟁이 우리의 삶에 어떠한 영향을 줄 수 있을 지 알아보았다. 우리가 원하는 방향으로 사람들의 인식을 이동시키려면 사람들에게 접근이 가장 쉬운 방법으로 가는 것이 좋을 것이라는 것을 깨달았다.
