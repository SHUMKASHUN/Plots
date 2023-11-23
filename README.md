# Plots
This repo is a collection of plotting skills which contains my customised style python-based plots for NLP papers, and includes the reproduction for some papers' plots.


## Table of Contents
- [Components](#components)

plot types:

Pairwise data: plot(x,y), scatter(x,y), bar(x,height)

More can be seen [here](https://matplotlib.org/stable/plot_types/index.html#plot-types)

## Components
<div align="center">
<img width="400" height="400" src="./assets/overview.png" />
</div>

Basically, there are two components you need to customize : first is the figure (Figure, Axes) which you might want to have multiple subplots in one figure. Another is everything inside an axes, you can customize each subplot(axes) one by one.
- Figure (plt.figure) 画布
- Axes (ax.subplots) 坐标系，可以有多个坐标系
- Axis 坐标轴，一般为2维，即x和y
    - y Axis (ax.yaxis)
    - x Axis (ax.saxis)
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
- Markers (ax.scatter) 
- Spine (ax.spines) 图四周的框

You just need to go through above components one by one to check what you need to customize.
## styling Artists
And for each artist you can also customize the folloing property.
- Font
- Colors
- markers
- labels
- linewidth
- linestyle


