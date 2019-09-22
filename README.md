# MTL Machine Learning

## 大綱

降維

>> 1. PCA
>> 2. Face Recognition
>> 3. Word Embeddings

進階回歸

>> 1. Kaggle House Price w. Lasso

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
