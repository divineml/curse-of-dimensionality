import plotly.offline as offline
import plotly.graph_objs as go
import matplotlib.pyplot as plt
offline.init_notebook_mode()

# class 1 data points
f1 = [1, 1,1,1,1,1,1,1,1,1,2, 2,2,2,2,2,2,2,2,2,3, 3,3,3,3,3,3,3,3,3,4, 4,4,4,4,4,4,4,4,4]
f2 = [1, 2, 3, 4, 5,6,7,8,9,10, 1, 2, 3, 4, 5,6,7,8,9,10, 1, 2, 3, 4, 5,6,7,8,9,10, 1, 2, 3, 4, 5,6,7,8,9,10]
f3 = [9,9,9,9,9,9,9,9,9,9, 9,9,9,9,9,9,9,9,9,9, 9,9,9,9,9,9,9,9,9,9, 9,9,9,9,9,9,9,9,9,9]

# class 2 data points
f1_y2 = [6, 6,6,6,6,6,6,6,6,6,7, 7,7,7,7,7,7,7,7,7,8, 8,8,8,8,8,8,8,8,8,9, 9,9,9,9,9,9,9,9,9]
f2_y2 = [1, 2, 3, 4, 5,6,7,8,9,10, 1, 2, 3, 4, 5,6,7,8,9,10, 1, 2, 3, 4, 5,6,7,8,9,10, 1, 2, 3, 4, 5,6,7,8,9,10]
f3_y2 = [1,1,1,1,1,1,1,1,1,1, 1,1,1,1,1,1,1,1,1,1, 1,1,1,1,1,1,1,1,1,1, 1,1,1,1,1,1,1,1,1,1]

trace1 = go.Scatter3d(x = f1, y = f2, z = f3, name = 'Class 1')
trace2 = go.Scatter3d(x = f1_y2, y = f2_y2, z = f3_y2, name = 'Class 2')
data = [trace1, trace2]

layout = go.Layout(scene = dict(
xaxis = dict(title = 'Feature 1'),
yaxis = dict(title = 'Feature 2'),
zaxis = dict(title = 'Feature 3')))

figure = go.Figure(data = data, layout = layout)
offline.iplot(figure, filename = 'Curse_of_dimensionality_blog')
