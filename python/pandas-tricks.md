# Pandas Tricks

## Rename columns

```python
# Rename any number of columns
df = df.rename({'col one':'col_one', 'col two':'col_two'}, axis='columns')

# Rename all columns
df.columns = ['col_one', 'col_two']
```

## Reverse row order

```python
# Reverse rows
df.loc[::-1]

# Reverse rows and reset the index to let it start from zero
df.loc[::-1].reset_index(drop=True).
```

## Reverse column order

```python
# Reverse columns
df.loc[:, ::-1]
```

## Convert string to number

```python
df = df.apply(pd.to_numeric, errors='coerce').fillna(0)
```

## Create a DataFrame from the clipboard

```python
df = pd.read_clipboard()
```

## Filter a DataFrame by multiple categories

```python
# Use the "or" operator
movies[(movies.genre == 'Action') | (movies.genre == 'Drama') | (movies.genre == 'Western')]

# Use isin() method
movies[movies.genre.isin(['Action', 'Drama', 'Western'])]

# Exclude with tilde
movies[~movies.genre.isin(['Action', 'Drama', 'Western'])]
```

## Filter a DataFrame by largest categories

```pythonmovies[movies.genre.isin(counts.nlargest(3).index)]
```

## Split a string into multiple columns

```python
df[['first', 'middle', 'last']] = df.name.str.split(' ', expand=True)
df['city'] = df.location.str.split(', ', expand=True)[0]
```

## Aggregate by multiple functions

```python
orders.groupby('order_id').item_price.agg(['sum', 'count'])
```

## Combine the output of an aggregation with a DataFrame

```python
# The transform() method performs the same calculation but returns output data that is the same shape as the input data:
total_price = orders.groupby('order_id').item_price.transform('sum')
orders['total_price'] = total_price
```

## Change display options

```python
pd.set_option('display.float_format', '{:.2f}'.format)

# Reset any option back to its default
pd.reset_option('display.float_format')
```
