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

[Optimizing data manipulation with vectorization](https://www.youtube.com/watch?v=nxWginnBklU)
![[Pasted image 20250125143833.png]]
Using np.where is equivalent to using the vectorization. Using .values explicitly sheds all things other than the value itself, furthering improving time.

np.select(conditon, choices, default="NA")
```python
conditions = [
	df['data_col1'] == df['data_col2'],,
	(df['norm_status'].str.startswith('cli') & df['norm_status'].str.endswith('.txt')) ,
	df['norm_status'].isin(multi_touch_leads),
	df['norm_status'].isin(eng_multit_leads)
	]

choices = [
	'new leads',
	'client leads',
	'mtouch leads',
	'emtouch leads'
	]

df['leafcat'] = np.select(conditions, choices, default='other')
```
equivalent to if elif else statements. note that the 2nd condition is an nested if statements.

### dictionary look ups
```python
def a_dict_lookup(row):
	if row['providers']>7:
		return 'upmarket'
	else:
		channel = channel_dict.get(row['Category'])
		return channel
#SAME BUT WAY FASTER
df['dict_lookup'] = np.where(df['providers']>7, 'upmarket', 
							 df['category'].map(channel_dict))
```
