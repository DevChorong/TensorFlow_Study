# Tensorflow 기본 연산 명령어

### [ import tensorflow as tf ]

#### 1. 변수 선언 방법

```Tensorflow
a = tf.constant(5, name="const_a")				#상수 선언
```



#### 2. 기본 4칙 연산

```Tensorflow
a = tf.add(5,4, name="add_a")					#덧셈
b = tf.subtract(10,3, name="sub_b")				#뺄셈
c = tf.multiply(2,5, name="mul_c")				#곱셈

```

