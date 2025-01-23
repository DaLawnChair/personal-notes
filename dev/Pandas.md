[Iterating pandas dataframes more efficiency](https://www.youtube.com/watch?v=SAFmrTnEHLg)
For changing values of a dataset, typically iterating over every row `for idx, row in df.iterrows()` is very slow. 

A faster way to always do it is with the apply function. `df['param'] = df.apply(function, axis=1)`. This is using the built-in iterator or something to make it way way faster.

Sometimes if you want to apply a function that is based on boolean values form the return of the enteries, then you can use vectorized iteration over the entire dataset:

```python
# base case of else condition
df['param'] = df['elseCondition']
# and then for the if case
df.loc[ (df['param1']==val1) & (df['param2']==val2) | .... ] = df['ifCondition']   
```

[Minimizing space taken by dataframes](https://www.youtube.com/watch?v=u4rsA5ZiTls)
* `df.to_csv("path",index=False)` is fairly slow
	* OK if you are sharing it and viewing it on Excel
* You can declare the column type with `df[param] = df[param].astype(type)`. This will greatly speed up loading and reduce the size of the file. 
	* However when exported as csv, pandas will need to infer the type, taking time
* `df.to_pickle("path",index=False)` is a bit faster and more space efficent
* BUT FOR THE BEST IMPROVEMENTS, use parquet
	* First ensure you have it installed with `pip install pyarrow` or `pip install fastparquet`
	* `df.to_parquet("path",index=False)`
