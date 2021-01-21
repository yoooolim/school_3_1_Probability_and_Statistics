# school_3_1_Probability_and_Statistics

#### 1.Gaussian distribution of Random variable
###### [문제] : random number를 생성하는 함수를 이용하여 Gaussian 분포를 갖는 random variable을 생성하도록 변경

###### [전략] : 
1. random number를 생성하는 rand함수를 이용해 uniform한 분포를 가지는 난수들 생성

![uniformpdf](./image/uniformpdf.png)

2. uniform한 확률밀도함수(pdf)를 누적분포함수(cdf)로 변환

![uniformcdf](./image/uniformcdf.png)

3. 수식을 이용해 uniform한 누적분포함수(cdf)를 gaussian 형태의 누적분포함수(cdf)로 변환

![gausiancdf](./image/gaussiancdf.png)
![equation](./image/equation.png)

4. 누적확률에 해당하는 z값을 찾기 위해 이진검색 기법을 활용해 gaussian 누적분포함수(cdf)의 역함수를 얻어냄

5. 얻어낸 역함수를 이용하여 gaussian 형태의 확률밀도함수(pdf)를 생성

![gausianpdf](./image/gaussianpdf.png)

###### [주요코드]

###### [결과화면]

![result](./image/result.png)

좌측, 위 = uniform한 pdf
우측, 위 = gaussian pdf
좌측, 아래 = gaussian cdf
우측, 아래 = 이론적 gaussian cdf와 생성한 gaussian cdf의 비교

----------------------------------

#### 2.Histogram Equalization
