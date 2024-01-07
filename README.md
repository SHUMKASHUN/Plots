# Plots
This repo is a Matplotlib Toolkit that helps you know how to customize every part of the plots. It also contains my customised style for NLP papers, and includes the reproduction for some papers' plots.

The repo are divided into three parts:
- Components # Showing you how to manipulate each sub-component
- Styles  # Showing you how to customize the styles
- Example # You can directly use this as template 

## Table of Contents
- [Components](#components)
- [Style](#style)

## Components
<div align="center">
<img width="400" height="400" src="./assets/overview.png" />
</div>

Basically, there are two components you need to customize : first is the figure (Figure, Axes) which you might want to have multiple subplots in one figure. Another is everything inside an axes, you can draw each subplot(axes) one by one.
- Figure (plt.figure) 画布
- Axes (ax.subplots) 坐标系，可以有多个坐标系
- Axis 坐标轴，一般为2维，即x和y
    - y Axis (ax.yaxis)
    - x Axis (ax.xaxis)
- Title  (ax.set_title) 标题，每个axes可以有标题，figure也可以有标题
- Legend (ax.legend) 图例
- Grid  (ax.grid) 网格
- Labelling 坐标轴名称
    - ylabel (ax.set_ylabel)
    - xlabel (ax.set_xlabel)
- Ticks 刻度相关的
    - Minor tick (ax.yaxis.set_minor_locator)
    - Minor tick label (ax.xaxis.set_minor_formatter)
    - Major tick (ax.yaxis.set_major_locator)
    - Major tick label (ax.yaxis.set_major_formatter)
- Line  (ax.plot) 线
- Markers (ax.scatter) 点的标志
- Spine (ax.spines) 图四周的框
- Artist (text, annoation)

You just need to go through above components one by one to check what you need to customize.


## Style
There are many kind of methods to customize the styles (e.g. color, linestyle, linewidth, font...), you can use run-time rc settings, matplotlibrc files or simply embedded all the styling codes into your main code snips.
In this folder, all the styling properties of the component are listed as a refenrece, and you can directly call it in your main code by insert {key:value}.


## Examples

### Colors
This includes my usual colors for reference

### Roboto
This is my usual font, you can use it by specifying

```python
import matplotlib.font_manager as font_manager

font_dir = ['./Roboto']
for font in font_manager.findSystemFonts(font_dir):
    font_manager.fontManager.addfont(font)

```