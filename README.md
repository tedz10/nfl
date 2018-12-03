CS 171 Project

Team Title: What’s it take to make the playoffs?

Team Name: Scott’s Tots

Team Members:

Curtis Hsu, Ted Zhu, Ray An, Kelly Mcdougal

Code: 
The html file that is our webpage is index.html. 
The CSS code is found in “style.css”.
All our visualizations are initialized in “main.js” except for “mainupdate.js” which is linked in the website to another page.
All our other code for the visualizations are in the following .js files which is located in the “js” folder, and the names refer to the visualization in main: barchart.js, linegraph.js, main.js, rushing.js, StackedAreaChart.js, tree.js, and turnover.js. 
The files animation_controllupdate.js, color-labels.js, fade.js, focus_point.js, focus_point.js, focus_pointupdate.js, generate_visupdate.js, mainupdate.js, newinitialisation.js, and tracesupdate.js are all used to make the scatterplot that transitions over time work.
The remaining .js files in the “js” folder are libraries.

Data: 
Our data consists of play by play data, which is scraped from NFLScrapR. We processed this data source to create .csvs to be used for each visualization. The data is saved in the “raw_data” folder. Any data that we processed and then uploaded into javascript can be found in “data”.

Data Mining / Machine Learning:
All code pertaining to the decision tree is in the ‘dt’ folder
With the question of our project being “What’s it take to make the playoffs,” we run a decision tree where we include features such as points per game, rushing yards per game, passing yards per game, offensive yards let up, turnover differential, red zone percentage, and sacks. To achieve this data, we first process it using python. To create this decision tree, we use the sklearn package. We then visualize our decision tree. 

URL:  https://tedz10.github.io/nfl/

Screencast URL: https://www.youtube.com/watch?v=JYbIBKaKRpI&feature=youtu.be

Features:
Our main visualization consists of a decision tree. After fitting a decision tree on all 32 playoff teams from 2010 to 2017 (for a total of 256 teams and 96 playoff teams), we created a json file that matches the nodes and children structure of a tree. By clicking on a node, we can expand its children. By hovering over the node, we can see statistics such as the number of samples in this node, the playoff non-playoff breakdown, and the gini impurity. 

For our supplementary visualizations, we start with a stacked area chart, where hovering over the area gives the type of method the points were scored. For the offensive yards let up visual, we click on the start button to see transitions over time and click to also stop the animation. For the rushing bar chart, the drop down menu allows the user to parse the data, and a tool tip activates upon hovering. Finally, on the turnover differential visualization, clicking on a bar gives more information about the team’s turnovers for the year. 

