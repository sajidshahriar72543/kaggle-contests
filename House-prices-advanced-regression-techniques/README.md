## Tutorial Followed
```
https://www.youtube.com/watch?v=vtm35gVP8JU
```
### Problem faced:
#### in training (prediction part)
```py
ValueError                                Traceback (most recent call last)

<ipython-input-49-3ee22fae4be8> in <cell line: 2>()
      1 knn_model = KNeighborsClassifier(n_neighbors=1)
----> 2 knn_model.fit(X_train, y_train)

6 frames

/usr/local/lib/python3.9/dist-packages/pandas/core/generic.py in __array__(self, dtype)
   2068 
   2069     def __array__(self, dtype: npt.DTypeLike | None = None) -> np.ndarray:
-> 2070         return np.asarray(self._values, dtype=dtype)
   2071 
   2072     def __array_wrap__(

ValueError: could not convert string to float: 'RL'
```