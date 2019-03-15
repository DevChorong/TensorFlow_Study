# Tensorflow Study

### # 개발환경 구축

1. Python 3.6 설치

2. Anaconda 설치

3. Anaconda prompt를 이용해서 다음을 설치

   > ```prompt
   > $ pip3 install tensorflow
   > $ pip3 install numpy
   > $ pip3 install matplotlib
   > ```



### # 실행 순서

**1. Anaconda Prompt 실행**

**2. 다음 명령어 작성**

```prompt
$ activate tensorflow
$ jupyter notebook
```

**3. Jupyter notebook 가서 Python3 파일 생성하기**



### # Tensor board 사용법

**1. Jupyter Notebook 소스코드에 다음과 같이 작성**

```Python
import tensorflow as tf
import numpy as np
tf.reset_default_graph()

...

with tf.Session() as sess:
    writer = tf.summary.FileWriter('D:\Tensorflow_Study\graph_log', sess.graph)
```

*나같은 경우는 D드라이브에 Tensorflow_study라는 폴더를 만들고 graph_log라는 폴더를 넣었다.*



**2. Anaconda Prompt 에 다음과 같은 명령어 입력**

```Anaconda Prompt 
$ activate tensorflow
$ tensorboard --logdir=D:\Tensorflow_Study\graph_log\
```



**3. 그래프 확인**

