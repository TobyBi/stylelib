# Matplotlib style sheets

2021/02/26 and tested on Windows 10, Python 3.8.5 and matplotlib 3.3.4.



To create [custom matplotlib stylesheets](https://matplotlib.org/stable/tutorials/introductory/customizing.html) that are available across the system, they must be placed inside the configuration directory.



matplotlib's configuration directory is found using

```python
>>> import matplotlib
>>> matplotlib.get_configdir()
'C:\\Users\\<PROFILENAME>\\.matplotlib'
```



Within `C:\\Users\\<PROFILENAME>\\.matplotlib` create `stylelib` directory and place the `.mplstyle` file in there.



To check the available style sheets run the following:

```python
>>> import matplotlib.pyplot as plt
>>> plt.style.availabe
['Solarize_Light2', '_classic_test_patch', 'bmh', 'classic', 'dark_background', 'fast', 'fivethirtyeight', 'ggplot', 'grayscale', 'jupyter_notebooks', 'seaborn', 'seaborn-bright', 'seaborn-colorblind', 'seaborn-dark', 'seaborn-dark-palette', 'seaborn-darkgrid', 'seaborn-deep', 'seaborn-muted', 'seaborn-notebook', 'seaborn-paper', 'seaborn-pastel', 'seaborn-poster', 'seaborn-talk', 'seaborn-ticks', 'seaborn-white', 'seaborn-whitegrid', 'tableau-colorblind10']
```

where the returned list contains the default style sheets and any custom ones added to the configuration directory.



Another option is to clone [my GitHub repository](https://github.com/TobyBi/stylelib) containing my custom style sheets into the configuration directory.