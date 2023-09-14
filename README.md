# 유성구 도서관 대출 데이터 분석
유성구에 거점 도서관인 8개의 도서관 데이터를 분석하여 간단한 통계와 이를 통한 W_socre, K-NN 두 가지 도서추천 방식을 적용해본다. 
https://lib.yuseong.go.kr/
https://www.data4library.kr/

## Getting Started
### Environment
 - python 3.10
 - pandas
 - pickle
 - matplotlib
 - seaborn
### Prerequisites
**Step 1 - 데이터 전처리 진행 [link](https://forums.developer.nvidia.com/t/pytorch-for-jetson/72048)**   
**Step 2 - 키워드 분석 진행**
**Step 3 - 추천 알고리즘 진행**

## Issues
If you got TLS block issue when import the sklearn in ipynb, add this
```python
import os
os.environ['LD_PRELOAD']
```

## Customize
Moving the Robot in real world you should have to change the parameters of Robot movements  for adaptable real world
```python
if gesture_joints == 1: # stop
    robot.stop()
```

## Running the tests
![](/동감_워드클라우드.png)
![](imgs/run.gif)
![](imgs/backward.jpg)


## References
- [kaggle](http://github.com/NVIDIA-AI-IOT/jetcam) - 책 추천 알고리즘에 대한 코드
