# Hotel Booking - a Vertex Coloring Algorithm project
This project was done as a personal project for the purpose of applying the Graph Theory algorithm with real-life data.

#### -- Project Status: Completed October 2019

## Project Intro
The famous [vertex coloring problem](http://mathworld.wolfram.com/ChromaticNumber.html) has many real-world applications, one of which is to optimise the allocation of resources for interval graph. This can be a simple model for a hotel booking system to allocate customers into rooms so that we can minimize the number of rooms required for a period of time; or a seat reservation system to allow maximum sales without overbooking or overbooking.

[MAST20018 - University of Melbourne](https://handbook.unimelb.edu.au/2019/subjects/mast20018) proposes the following solution for this example problem: **Suppose that we have 6 guests staying at a hotel for different durations, what is the minimum number of rooms to prepare to cater for everyone?**
![Algorithm Demonstration](https://github.com/danieltpham/hotel-booking-optimisation/blob/master/Slide1.gif)
* Represent every guest as a node
* All guests that stay on the same day are connected by an edge
* Apply the Vertex Coloring Algorithm (Welsh-Powell algorithm) to allocate guests to a room
* The number of colors used is the minimum number of rooms to prepare

This personal project applies the previous algorithm to [a real-life hotel booking dataset](https://www.sciencedirect.com/science/article/pii/S2352340918315191), using data manipulation techniques to query the dataset and demonstrate the huge execution time of this simple approach.

### View Project
[Click here to view project output](https://nbviewer.jupyter.org/github/danieltpham/hotel-booking-optimisation/blob/master/Optimisation_Stage2.ipynb)

### Methodologies
* Python
* Pandas, jupyter
* Network theory, networkx

## File Descriptions
* [Jupyter Notebook](https://github.com/danieltpham/hotel-booking-optimisation/blob/master/Optimisation_Stage2.ipynb)
* [Hotel booking dataset](https://github.com/danieltpham/hotel-booking-optimisation/blob/master/H1.csv)
* [Dataset description](https://github.com/danieltpham/hotel-booking-optimisation/blob/master/1-s2.0-S2352340918315191-main.pdf)

## Usage Notes
* Input a date between 1/7/2015 and 24/8/2017 as a starting date in `2. Select a week to analyse`
* The code only optimises stays for 1 week (7 days) starting from the starting date, due to large runtime of the algorithm


