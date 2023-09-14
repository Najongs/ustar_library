# 유성구 도서관 대출 데이터 분석
유성구에 거점 도서관인 8개의 도서관 데이터를 분석하여 간단한 통계와 이를 통한 W_socre, K-NN 두 가지 도서추천 방식을 적용해본다. 
https://lib.yuseong.go.kr/
https://www.data4library.kr/

## Getting Started
### Environment
 - python 3.10
 - pandas
### Prerequisites
**Step 1 - Download PyTorch and Torchvision for Jetson nano. [link](https://forums.developer.nvidia.com/t/pytorch-for-jetson/72048)**   
**Step 2 - Install [torch2trt](https://github.com/NVIDIA-AI-IOT/torch2trt)**
```
$git clone https://github.com/NVIDIA-AI-IOT/torch2trt
$cd torch2trt
$sudo python3 setup.py install --plugins
```

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
elif gesture_joints == 2: # left
else:
    robot.stop()   
```

## Running the tests

![](imgs/run.gif)
![](imgs/backward.jpg)


## References
- [kaggle](http://github.com/NVIDIA-AI-IOT/jetcam) - 책 추천 알고리즘에 대한 코드
