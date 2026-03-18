# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
import numpy as np

#Basic 2D Plot
x = np.arange(76, 100)
y = np.arange(101, 125)

plt.scatter(x, y, label='Scatter Points')
plt.plot(x, y, color='red', marker='*', linestyle='dashed', linewidth=2, markersize=12, label='Dashed Line')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2D Diagram')
plt.legend()
plt.savefig('basic_plot.png')
plt.show()
plt.clf()

#2. Subplots (2x2 Grid) 
plt.subplot(2, 2, 1)
plt.plot(x, y, 'r--')
plt.title('Red Dashed')

plt.subplot(2, 2, 2)
plt.plot(x, y, 'g*--')
plt.title('Green Star-Dash')

plt.subplot(2, 2, 3)
plt.plot(x, y, 'bo')
plt.title('Blue Dots')

plt.subplot(2, 2, 4)
plt.plot(x, y, 'go')
plt.title('Green Dots')

plt.tight_layout() # Prevents overlap
plt.savefig('subplots.png')
plt.show()

plt.clf()

#3. Sine and Cosine Waves 
x_wave = np.arange(0, 5 * np.pi, 0.1)
plt.subplot(2, 1, 1)
plt.plot(x_wave, np.sin(x_wave), 'r--')
plt.title('Sine')

plt.subplot(2, 1, 2)
plt.plot(x_wave, np.cos(x_wave), 'g--')
plt.title('Cosine')

plt.tight_layout()
plt.savefig('waves.png')
plt.show()

plt.clf()

# Bar Graph
x_bar = [2, 8, 10]
y_bar = [11, 16, 9]
x2_bar = [3, 9, 11]
y2_bar = [6, 15, 7]
plt.bar(x_bar, y_bar, label='Set 1')
plt.bar(x2_bar, y2_bar, color='g', label='Set 2')
plt.title('Bar Graph')
plt.legend()
plt.savefig('bar_graph.png')
plt.show()

plt.clf()


#Pie Chart
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0.1, 0, 0, 0) # explode 1st slice
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal') # Equal aspect ratio ensures that pie is drawn as a circle.
plt.title('Programming Languages')
plt.savefig('pie_chart.png')
plt.show()
```
<img width="987" height="538" alt="Screenshot 2026-03-18 154142" src="https://github.com/user-attachments/assets/c0819596-a599-42b4-aee2-a422c4755ed6" />

<img width="825" height="552" alt="Screenshot 2026-03-18 154150" src="https://github.com/user-attachments/assets/8af6c0f7-54f9-47ce-b2a8-b549553139ae" />
<img width="828" height="561" alt="Screenshot 2026-03-18 154202" src="https://github.com/user-attachments/assets/541a0782-2586-4f34-80ad-58a20bda9eb1" />
<img width="825" height="517" alt="Screenshot 2026-03-18 154214" src="https://github.com/user-attachments/assets/eece645f-4502-447b-a4c0-b09eb12e4aa9" />
<img width="827" height="468" alt="Screenshot 2026-03-18 154222" src="https://github.com/user-attachments/assets/d33f000e-208a-4aaf-a156-002797e2c17b" />

# Result:
Thus, data visualization using matplotlib library is completed successfully
