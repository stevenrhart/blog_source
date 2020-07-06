+++
title = "Test"
date = "2020-07-06"
author = "Steve Hart"
categories = ["python", "data-science"]
tags = ["tag1", "tag2", "tag3"]
+++


## Test notebook

This is a test notebook to see if I can embed the notebook into a Hugo site. 
    


```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

data = {'apple': 10, 'orange': 15, 'lemon': 5, 'lime': 20}
names = list(data.keys())
values = list(data.values())

fig, axs = plt.subplots(1, 3, figsize=(9, 3), sharey=True)
axs[0].bar(names, values)
axs[1].scatter(names, values)
axs[2].plot(names, values)
fig.suptitle('Categorical Plotting')
```




    Text(0.5, 0.98, 'Categorical Plotting')




![png](output_2_1.png)


## Second H2

This is another section of my test post showing how it will render in the hugo site.



```python
index = pd.date_range('1/1/2000', periods=8)
s = pd.Series(np.random.randn(5), index=['a', 'b', 'c', 'd', 'e'])
df = pd.DataFrame(np.random.randn(8, 3), index=index, columns=['A', 'B', 'C'])
df.tail()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>A</th>
      <th>B</th>
      <th>C</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2000-01-04</th>
      <td>-0.065897</td>
      <td>0.185572</td>
      <td>0.309261</td>
    </tr>
    <tr>
      <th>2000-01-05</th>
      <td>1.224395</td>
      <td>-0.681050</td>
      <td>1.886576</td>
    </tr>
    <tr>
      <th>2000-01-06</th>
      <td>-0.040993</td>
      <td>0.465080</td>
      <td>-0.228796</td>
    </tr>
    <tr>
      <th>2000-01-07</th>
      <td>0.418251</td>
      <td>-1.051027</td>
      <td>-0.092839</td>
    </tr>
    <tr>
      <th>2000-01-08</th>
      <td>1.150586</td>
      <td>0.336295</td>
      <td>-0.599662</td>
    </tr>
  </tbody>
</table>
</div>




```python

```
