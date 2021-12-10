# User Stories:

## Researchers:
- Trends in migrant detention facilities over the last 10 years to answer questions about the impact of opening and closing detention facilities
- Visualize certain trends, pull our data and the way that we have organized it so that they can work with it
- Interacting via a webpage 
- More technical experience

## Policymakers/Advocates:
- Visualize trends in order to get summary level statistics in order to make broad policy decisions
- A way to output visualizations
- Easy drop down menus to change relevant variables (years, citizenship, various demographics)
- Less technical, make it very very clear and easy to use


## Technician/Data Scientist:
- Add to or edit data that already exists on the portal
- Add to or edit visualization formatting and displays
- Add to or edit language on the user interface
- Ability to preview what the portal looks like to other users

# Functional Design: 

## Researchers:

1. Include drop down boxes for variables for visualizing tables of data subsets
2. Include drop down boxes for variables so that users can visualize charts
3. Allow users to download the data they want:
  a. All the data
  b. Prespecified subsets of the data
  c. Data that you visualized through the interface
4. Allow users to download visualizations:
  a. Tables
  b. Interactive plots downloaded as still figures

## Policymakers/Advocates:
1. 
2. 
3.
4. 
5. be able to see most popularly created visualizations/charts on the site 


## Technician/Data Scientist:
1.
2.
3.
4.
5. 
6. Adding/Removing new data
7. Adding/Removing new visualization functionality
8. Changing the language on the website
9. Handling website traffic
10. Algorithm for choosing most often created visualizations
11. View user statistics/demographics
12. Email collection of site visitors to update them on site progress (stretch goal)

# Component Design

Name: User interface
- What it does: allows users to request tables, charts, and files 
- Inputs: drop down options for output format and data selection 
- Outputs: files, tables, and charts 

Name: Download
- what it does: it produces a file
- Inputs: type of file and data/charts to include
- Outputs: file for download

Name: Visualization
- what it does: produces a table or chart
- Inputs: data to include and format of chart or table
- outputs: chart or table

Name: Database 
- What it does: it stores spreadsheets and shape files 
- Inputs: requests from users 
- Outputs: files, tables, and charts 

## Interaction diagram
![Portal Interaction Diagrams](https://user-images.githubusercontent.com/70054008/139509645-53e18fe0-240a-4fd0-9a70-9710be34779d.png)


