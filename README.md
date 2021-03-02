# Originpro Plot
Matplotlib style for making originpro plot figures
This repo has Matplotlib OriginPro style to format your figure for scientific publications and presentation.

# Getting Started
The easist way to install OriginproPlot is to use [pip](https://pip.pypa.io/en/stable/): 
```
# to install the latest release (from PyPI) 
pip install OriginproPlot

# to install latest commit (from GitHub)
pip install git+https://github.com/mcekwonu/OriginproPlot.git
```

The pip installation will automatically move all of the Matplotlib style files ```*.mplstyle``` into the appropriate directory on your computer.

Please see the FAQ section for more information and troubleshooting.

# Using the Style
"originpro" is the main style from this repo. Whenever you want to use it, simply add the following to the top of your python script:
```python
import matplotlib.pyplot as plt
plt.style.use('originpro')
```
To use any of the styles temporarily, you can use:
```python
with plt.style.context(['originpro']):
    plt.figure()
    plt.plot(x, y)
    plt.show()
```

You can adjust the legend borderpad for proper placement if you have more that four parameters using:

```python
# for example, manually set the borderpad after trying out the position values and update the matplotlib parameters.
plt.rcParams['legend.borderaxespad'] = -4.5
plt.rcParams.update()
```
# Examples
The ```Originpro``` style:

# Help and Contribution
Please feel free to contribute to the OriginproPlot repo! For example, it would be good to add new styles for different journals. Before starting a new style or making any changes, please create an issue through the GitHub issue tracker. That way we can discuss if the changes are necessary and the best approach.

If you need any help with OriginproPlot, please first check the FAQ and search through the previous GitHub issues. If you can't find an answer, create a new issue through the GitHub issue tracker.

You can checkout Matplotlib's documentation for more information on plotting settings.

# FAQ
1. Installing OriginproPlot manually
If you like, you can install the ```*.mplstyle``` files manually. First, clone the repository and then copy all of the ```*.mplstyle``` files into your Matplotlib style directory. 
If you're not sure where this is, in an interactive python console type:
