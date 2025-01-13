# 데이터 분석 질문 정리 

필수 역량:
- 데이터 핸들링: 데이터를 sql을 활용.
- 데이터 분석
- 대시보드 개발: 분석된 결과를 시각화하는 역할

+ 데이터 분석은 데이터 기반 인사이트를 기술적인 부분 뿐만 아니라 비즈니스적으로 풀어가는 것이 중요한 역량으로 작용한다.

+ Python/R: Tool을 활용하여 데이터 추출, 전처리, 모델링, 리포트 작성 등의 업무 가능.
+ 현업에 니즈를 파악하여 과제를 구체화시키는 단계/ 분석된 결과를 토대로 현업에 적용시키는 단계가 중요하다.

----------

### 데이터 랭글링 

- 데이터를 발견, 정제 그리고 검증을 하며 사용이 가능한 데이터 형식이 되도록 구조화하고 통합 및 변환하여서 유용한 정보로 가공하는것을 의미한다.
- 원자료 (Raw Data)를 가공하고 분석할 수 있도록 변환하는 과정이다.
- 보통의 원자료 데이터는 불필요한 정보, 오류 등으로 오염이 된 경우가 많은데 이때 이 데이터에서 유용한 상관관계를 발견하고 추출하는것이 목적이다.

**단계별 프로세스**
1. 데이터 발견
2. 데이터 구조화
3. 데이터 정제
4. 데이터 강화
5. 데이터 유효성 검사
6. 데이터 출판 (활용)

----------

### 정규 분포

- 데이터의 대부분 값이 중앙에 분포되어 있고, 중앙에서 멀어질수록 가늘어지는 종형의 모양을 띄고 있다.
- 또한, 치우쳐짐 (skewness)이 없이 대칭적으로 분포되어있다는 특징을 가지고 있다.
- 평균과 표준편차의 값으로 설명할 수 있다.
- 평균과 표준편차의 값이 달라지면 그래프의 모양도 변하는데, 표준편차가 커지면 그래프의 모양이 더 퍼지고, 평균값이 커지면 중앙값이 우측으로 이동한다.

----------

### 누락 데이터를 처리하는 방법 

1. Missing value인 부분을 데이터의 평균값으로 대체한다.
- 이런 방식을 이용하면 데이터를 분석하는데 방해가 되지 않고 쉽고 빠르게 처리할 수 있다.
- 하지만 데이터간의 상관관계를 포착하는데 도움이 되지 않는다.
  
2. 가장 빈번하게 나오는 값으로 대체한다.

3. K-NN imputation
- classification에 사용되는 알고리즘중 하나로 <ins>가장 근접한 데이터 K개</ins>를 찾아 거리에 따른 가중 평균을 대체한다.
- 

+ MICE, Regression Imputation(회귀 대치) - 관측치간의 회귀식을 이용하여 결측치를 예측한다.

------------

### 클러스터링 

- 비슷한 특성을 가진 데이터들끼리 같은 군집으로 묶는 것을 의미한다.
- 데이터 마이닝의 기법중 하나이다.

**데이터 마이닝**

- 데이터 안에서 통계적인 패턴을 분석해서 가치있는 정보를 찾아내는 일이다. 

### Outlier (극단치)

- 데이터의 분포에서 다르게 나타내는 값이며, 패턴 분석에 방해를 하는 요소(변수값) 이다.

### N-grams

- N개의 연속적인 단어 나열을 의미한다. (연속적인 단어 나열을 끊어서 '토큰'이라고 간주한다.)

### Statistical Model (통계 모델)
- 수학적 모델 그리고 통계 추정을 사용하여 수학적 관계로 규정하는 것이다.

----------

### Data Mining vs Data Profiling 

- 데이터 마이닝 = 데이터 분석을 위한 데이터 전처리 과정으로 가치있는 정보를 찾아내는 일이다. (** 특정 패턴을 찾아낸다)
- 데이터 프로파일링 = 데이터와 그 특성을 이해하는데 도움이 되는 과정이다. 


### 조인 vs 유니온 vs 블랜딩 차이 (in Tableau)

- Join = 두 데이터셋을 연결하며 (왼쪽, 오른쪽, 바깥쪽을 선택하여 어떤 방식으로 결합할지 선택할 수 있다.) ** 데이터를 결합한후 집계한다. **(두 데이터셋을 연결)**
- Union = 한 테이블의 행을 다른 테이블에 추가할 수 있는 방식 (* 데이터셋의 유형과 필드 수가 같아야 한다.)
- Blending =  조인과 비슷하게 데이터셋을 연결하지만 다른 소스에 있는 데이터셋을 결합할 수 있다. ** 데이터를 집계한후 결합한다.

**ETL** - 데이터를 추출, 정제하는 프로세스를 의미한다. 

**KDD 분석 방법론**
- 데이터 선정 -> 데이터 전처리 -> 데이터 변환 -> 데이터 마이닝 -> 평가
- 데이터의 패턴을 분석하기 위한 프로세스.

### 정확도 vs 정밀도
- 정확도 = 분석모델이 실제 값과 차이가 적은 것을 의미한다.
- 정밀도 = 분석모델이 여러번 반복해도 편차가 적은 것을 의미한다.

### Quantitative VS Qualitative (정상적 분석 vs 정량적 분석)
-  질적 분석 = 수학적 패턴과 통계를 통해 가설을 기정사실화 한다.
- 양적 분석 = 대화를 통해 이해하고 결과를 이끌어낸다. 

-----------

### 데이터 마이닝 vs 데이터 랭글링

- **데이터 전처리** = 데이터를 분석의 필요에 맞게 가공하는 과정. 
- **데이터 마이닝** = 데이터를 통계적 규칙이나 패턴을 분석하여 가치있는 정보를 추출해내는 과정.
- **데이터 랭글링** = 데이터를 분석하기 쉬운 형태로 가공하거나 통합하는 것. (비정형& 정형 데이터)
  (데이터 discover -> 데이터 구조화 -> 데이터 정제 -> 데이터 enrichment -> 데이터 검증 -> 데이터 출판)

### 정형 데이터 vs 비정형 데이터

- 정형 데이터는 데이터 테이블을 만드는데 적합한 형태의 데이터.
- 비정형 데이터는 데이터 테이블을 만드는데 적합하지 않다.

### Descriptive vs Predictive vs Prescriptive 
- Descriptive = insights to the answer (무엇이 일어났는지)
- Predictive = understands future to answer (무엇이 일어날지)
- Prescriptive = various course to actions (무엇을 해야 하는지)
  
### Univariate vs Bivariate vs Multivariate
- Univariate = Data being analyzed with only one variable
- Bivariate = analysis of two variables to find causes, relationships (두개의 변수간의 상관관계 분석)
- Multivariate = analysis of three or more variables to understand relationship

-------

### Twitter Sentiment Analysis Program

- Whether users are talking positively or negatively about the Notion
- Count the numbers of Tweet tagged as negative, positive and neutral
- Create the data visualization of each sentiments in relative terms 
