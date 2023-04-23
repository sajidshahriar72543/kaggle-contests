### Problem faced:

```py
TypeError Traceback (most recent call last)

<ipython-input-87-5cf22e7770fd> in <cell line: 1>()
----> 1 exponential_smoothing(ri_ar.Rainfall_Le_Croci,[0.005,0.02])

<ipython-input-84-a8a1e5506f8f> in exponential_smoothing(column, alpha)
      3 
      4     for n in range(1, len(column)):
----> 5         old=alpha*column[n]+(1-alpha)*result[n-1]
      6         result.append(old)
      7 

TypeError: can't multiply sequence by non-int of type 'numpy.float64'
```
```py
---------------------------------------------------------------------------

MissingDataError                          Traceback (most recent call last)

<ipython-input-92-c805c576fd75> in <cell line: 1>()
----> 1 tsplot(ri_ar.Rainfall_Le_Croci, lags=40)

11 frames

/usr/local/lib/python3.9/dist-packages/statsmodels/base/data.py in _handle_constant(self, hasconst)
    132             exog_max = np.max(self.exog, axis=0)
    133             if not np.isfinite(exog_max).all():
--> 134                 raise MissingDataError('exog contains inf or nans')
    135             exog_min = np.min(self.exog, axis=0)
    136             const_idx = np.where(exog_max == exog_min)[0].squeeze()

MissingDataError: exog contains inf or nans
```