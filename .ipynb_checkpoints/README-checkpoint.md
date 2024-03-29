# juspy
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/juspreet51/juspy)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/juspreet51/juspy)
![GitHub followers](https://img.shields.io/github/followers/juspreet51?label=%40Juspreet51&style=social)
![Twitter URL](https://img.shields.io/twitter/url?label=%40Juspreet51&style=social&url=https%3A%2F%2Fwww.twitter.com%2Fjuspreet51)
[![Discord](https://badgen.net/badge/icon/discord?icon=discord&label)](https://discord.gg/BMSMBmuweD)

<img src="https://raw.githubusercontent.com/juspreet51/juspy/main/src/juspy/media/logos/logo_white_bg.png">


juspy is a library for making EDA and Modelling in Python quick and convinient. It's built on top of:
- pandas
- numpy
- seaborn
- and many such great libraries

___
Our reccomended path of getting started with `juspy` 
<br>
- Download & install [Anaconda](https://www.anaconda.com/products/individual)
- Open `Anaconda Prompt`
- In `Anaconda Prompt` type
```python
conda install -c conda-forge jupyterlab
```
- and then
```python
pip install juspy
jupyterlab
```
<br>

<b>Incase if you're having any trouble regarding installation or dependencies, kindly make sure you're using updated versions</b>

```python
conda update conda
conda update pip
conda update python
```
<br>
And now try the above steps again

___
# Demo Notebooks:
<ol>
<li>
        
To test library's proper installation and working:

```python
import juspy
print(juspy.__version__)

from juspy import greet
print(greet.namastey())
```
<br>
    
Or, try greeting 
```python
print(greet.hello())
print(greet.ni_hao())
print(greet.hola())
print(greet.bonjour())
print(greet.schatz())
print(greet.ahlan())
print(greet.privet())
```
    
</li>
<br><br>
    If they're producing some output, we're good to go
<li>
    
 jpplot.[confusion_matrix()](https://github.com/juspreet51/juspy/blob/main/src/juspy/demo_nbs/01_confusion_matrix.ipynb)
```python
import numpy as np
import seaborn as sns
from sklearn.metrics import confusion_matrix

y_true = [0, 1, 0, 1, 0, 1, 0]
y_pred = [1, 1, 1, 0, 1, 0, 1]
cf_matrix = confusion_matrix(y_true, y_pred)

from juspy import plot as jpplot
jpplot.confusion_matrix(cf_matrix)
```
<br>
<img 
src="https://raw.githubusercontent.com/juspreet51/juspy/main/src/juspy/media/plot_cfm_output.PNG" 
style="width:35%;  display: block; margin-left: auto;  margin-right: auto;">
</li>
<br><br>
<li> 

jpplot.[piechart()](https://github.com/juspreet51/juspy/blob/main/src/juspy/demo_nbs/02_piechart.ipynb)

```python
import pandas as pd
df_name = pd.read_csv("https://raw.githubusercontent.com/juspreet51/juspy/main/src/juspy/datasets/default.csv")

from juspy import plot as jpplot
jpplot.piechart(df_name["student"])

```
<br>
<img 
src="https://raw.githubusercontent.com/juspreet51/juspy/main/src/juspy/media/plot_piechart_output.PNG" 
style="width:25%;  display: block; margin-left: auto;  margin-right: auto;">
</li>

<br><br>
    
## Future Release:

<li> 

from juspy.linear_models import [LinearRegression](#)
<br>
```python
from juspy.linear_models import LinearRegression as lin_reg
```
</li>
</ol>

___