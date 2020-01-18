# xlr8

#### Team: Ayush Yembarwar, Nikhil Khandelwal, Disha Jain, Ajinkya Vyas
#### College: BITS Pilani, Pilani Campus

Team Snowball's solution for the Mercedes-Benz Digital Challenge, India.

## Project Description

BCG reports that this number for Indians is between 1.3 and 1.6 times additional time in peak traffic amongst Asian cities. Today the average worker in urban India spends around 7% of their day in the office commute. In urban areas, traffic is the bottleneck for mobility, not the road infrastructure itself. Rapid urbanization is straining the transport network, and it necessitates a solution for the problem of congestion.

Congestion is a popular mathematical metric used in the world of route planning as a measure of the flow of traffic in a given road network. The problem at hand is to increase the overall mobility of the vehicles in the road network, i.e. reduce the time taken by the cars to reach their destinations.

Our idea posits an app similar to Google Maps with a new route planning algorithm - one that takes source and destination information for each vehicle using the app and computes the optimum route individually for each car such that the overall congestion is minimized. Keeping the principles the same, the same idea can be used to increase route planning efficiency for any high traffic transport system - aviation, railways, etc. The algorithm increases the mobility of all cars, ensuring optimum usage of the road infrastructure.

The algorithm can be used for route planning in commercial ride hailing applications, in fulfilment and delivery providers, and with emergency response services like ambulances and police vehicles as well. With minimal changes, the algorithm can be used for trips including multiple modes of transport as well. Another interesting use-case is for the self-driving cars of the future which would all be routed through a centralized platform. SInce our algorithm shows maximum improvement when applied large, dense vehicle networks, it would be very useful in this context.

This solution presented can scale well with Quantum Computing and other emerging technologies as well and thus can be a useful solution in the long term.


## Instructions to run

Our demo application "xlr8" is a web application, based on the Django web framework. It can be run either as a web app hosted at the aforementioned URL, or by hosting it locally on the machine that is running the application.

Steps for setting up a local xlr8 Django project:

1) Set up an isolated Python environment by first installing Python 3.

2) To install Python packages on your computer, Setuptools is needed. Download the latest version of Setuptools for your Python version.

3) Be sure to install the Python Package manager - "pip". This is usually included in the Python installation.

4) In the command prompt, execute the following command: pip install django.

5) Install the following dependencies: numpy, networkx.

6) Run the Django migrations to set up your models:

```
python manage.py makemigrations
python manage.py makemigrations polls
python manage.py migrate
```

7) Start a local web server:

```
python manage.py runserver
```

8) In your browser, go to http://localhost:8000:

```
http://localhost:8000
```

9) Press Control+C to stop the local web server.

10) The panel on the right can be used to add vehicles to the map by entering the source and destination of the vehicle. Up to 10 vehicles can be added to this demo application using the (+) and (X) signs displayed.

11) Hover on the red marker of any location on the map to know its location index and enter this index in the Source/Destination field in the right panel.

12) The most efficient paths from source to the destination for each of the entered vehicle would be displayed on the map on pressing Submit. (This may take some time for heavy inputs). The paths are decided so as to minimize the total congestion on the road network.

13) To resolve confusion between paths, click on a destination 'Flag' marker on the app. Clicking once will hide other paths. To redisplay all paths, click on the 'Flag' marker again.

Please Note: After each run of the application, please refresh the webpage before using it again. Using it multiple times without refreshing may result in the results from previous iterations overlapping.
