# MTK Machine Learning

## 大綱

降維

> 1. PCA
> 2. Face Recognition
> 3. Word Embeddings

進階回歸

> 1. Kaggle House Price w. Lasso

## PCA

### (如果沒Keras) 讀取MNIST資料集

先下載 [MNIST資料集](https://storage.googleapis.com/tensorflow/tf-keras-datasets/mnist.npz)

```python
def load_data(path):
    with np.load(path) as f:
        x_train, y_train = f['x_train'], f['y_train']
        x_test, y_test = f['x_test'], f['y_test']
        return (x_train, y_train), (x_test, y_test)

(x_train, y_train), (x_test, y_test) = load_data('../input/mnist.npz')
```

## 人臉辨識

[Colab](https://colab.research.google.com/drive/1pk1Vnqh5S0eEZq99BmItU12CNah4D_It)



## 語意分析

[Colab](https://colab.research.google.com/drive/1QXW5-A-Wxx1fsPxpyYFs6E-S3bVtuMTU)

## 進階回歸

[Kaggle競賽連結](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)

[RandomForesetRegressor比較](https://github.com/Elwing-Chou/MLDemo/blob/master/hourseprice.ipynb)

## 語法: Lambda

```python
def test(func):
    print(func(3))
def m2(n):
    return 2 * n
test(m2)
test(lambda n : 2 * n)

```

## 如果你是3.7

1. tensorflow==2.0.0

## 3.6
1. tensorflow==1.18.0

2. keras==2.1.5

3. protobuf==3.5.2.post1

## colab基底

[PCA](https://colab.research.google.com/drive/1pi0IXMPqNYwoeGYxHuflesjUe5h-nhTR)

[Face](https://colab.research.google.com/drive/19U7o4lpLU2Tl2Bw9kXWDuBHF8udfVtff)

## 0312colab基底

[sample](https://colab.research.google.com/drive/1JZR6Rl1BDYGD60g6iTbnR8NDDO62uo7G)

[face](https://colab.research.google.com/drive/1GIbcYKP54QmOWCt2T2GsBNP7vX8lFSvR)

## 1123素材

[PCA製作](https://colab.research.google.com/drive/14Q5OH8YPiFTGeW_uYY_LyMe6hw1ydJ3Q?usp=sharing)

[PCA觀察](https://colab.research.google.com/drive/11YJK9SdttgQeeZ-WzWockha5ThzJbTgj?usp=sharing)

[PCA MNIST基底](https://colab.research.google.com/drive/1kVFZjVg4XZjcW6yFXueDqIzndC95mxCI?usp=sharing)


[Face基底](https://colab.research.google.com/drive/1fe7_ewgj8PM9320_R2VXIPURzr9I2pIS?usp=sharing)
