# Impedance Data Analysis

This code is designed to analyse the difference in impedance between two data sets. It does this by visualising the data through a series of graphs. The individual data sets aren’t provided but "transfer.csv", which contains the difference between, them is included. Another dataframe could be analysed instead, as long as it is in the appropriate format.

To run:

**1 - Import required libraries and data for analysis
* Download “transfer.csv” and “Impedance Data Analysis” notebook to the same directory. 
* When reading in “transfer.csv”, ensure header = None so the first row of data isn't used as a header and excluded from analysis. Alter this as required if using another dataframe.

**2 - Initial data exploration
* Running the head function will show “transfer.csv” has three columns. The first is frequency in kHz, the second is time in minutes and the third is impedance difference.
* Sort the data by magnitude of impedance difference, investigating the greatest positive and negative differences over a range of rows.

**3 - Plot data in two dimensions
* Plot impedance difference against frequency using a 2D scatter graph. You should be able to see the largest differences in impedance are at frequencies below 1250 kHz, for example 400, 800, 1080 and 1180 kHz. This is in agreement with the sorting analysis performed before. 

* Next plot impedance difference against time in a scatter graph. There is a random spread of impedance differences across time, with most residing about 0 between -50 and 50. 

**4 - Plot data in three dimensions
* Run matplotlib as a notebook instead of inline, so you can interact with the 3D graphs.

* The first 3D plot is a trisurface, which is a surface plot made out of triangles.  Antialias = True makes the plot transparent, while False makes it opaque. Either can be used depending on how you want to view the plot.

* The second 3D plot is a scatter plot and shows individual data points, instead of a surface.

* The final 3D plot is a bar chart. Like the scatter plot it shows the increments of increasing time and frequency, unlike the surface plot which is continuous. However, the bar chart has depth to each data point, which the scatter plot doesn’t.

* The three 3D plots should look similar to the 2D plot of impedance against frequency if viewed along the time axis, and will resemble the 2D impedance difference against time graph if viewed along the frequency axis.