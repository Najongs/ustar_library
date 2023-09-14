# 유성구 도서관 대출 데이터 분석
유성구에 거점 도서관인 8개의 도서관 데이터를 분석하여 간단한 통계와 이를 통한 W_socre, K-NN 두 가지 도서추천 방식을 적용해본다. 
https://lib.yuseong.go.kr/
https://www.data4library.kr/

## Getting Started
### Environment
 - python 3.10
 - pandas
 - konlpy
 - pickle
 - matplotlib
 - seaborn
### Prerequisites
**Step 1 - 데이터 전처리 진행**   
  
**Step 2 - 키워드 분석 진행 [OKT](https://liveyourit.tistory.com/57)**  
  
**Step 3 - 추천 알고리즘 진행**

## Issues
pickle를 사용하여 데이터를 불러온다.
```python
import pickle
```

## Customize
W_socre를 구하는 방법
```python
#avg = 대출건수, count = 도서권수
v=popularite["count_rating"]
R=popularite["avg_rating"]
m=v.quantile(0.50)
c=R.mean()
popularite['w_score']=((v*R) + (m*c)) / (v+m)
```

## Running the tests
![](/동감_워드클라우드.png)
![](imgs/run.gif)

## References
- [kaggle](http://github.com/NVIDIA-AI-IOT/jetcam) - 책 추천 알고리즘에 대한 코드
