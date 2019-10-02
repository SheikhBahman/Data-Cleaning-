# Data-Cleaning-
Theory and Practice of Data Cleaning Course Project

- This is my course project submitted for ***CS-513: Theory and Practice of Data Cleaning*** at UIUC.

# Languages used
- To accomplish this project following languages/programs are empoyed:
  - OpenRefine
  - SQLite
  - YesWorkFlow
  - Python/Jython
  
# Introduction
In this project I used the techniques and tools I have learned for data cleaning and wrangling in the class: “CS513 Theory and practice of data cleaning” to clean a raw and messy data set. I have chosen the New York Public Library’s crowd-sourced historical menus called “What's on the Menu?” as the messy data to be cleaned. The tools I employed in this project are: OpenRefine, Python/Jython, SQLite and YesWorkFlow.

# Dataset
The New York Public Library’s data set is a crowd-sourced digitized data with approximately 45,000 historical menus. This data set originated through effort of Miss Frank E. Buttolph (1850-1924) is one of the largest in the world. Miss Buttolph added more than 25,000 menus to the collection, until 1924 before leaving the Library. After that the collection has continued to grow through additional voluntary added gifts of graphic, gastronomic, topical, or sociological interest, especially but not exclusively New York related (http://menus.nypl.org/about). Hence, this broad crowd-sourced data set requires to be cleaned. This data set contains four dataset files: Menu, MenuItem, MenPage and Dish.
  1. Menu data file
In the Menu data file each menu has an ID and may be provided with name for the menu, sponsor, event, place, address, occasion, call number, currency, note, date, page count, dish count. It contains 17,545 rows of data. Many cells are null/blank, names of the column seem to be not consistent.
  2. MenuPage data file
The data in the MenuPage file refers to each menu ID in the Menu file provides details about a page in a menu. Also each data row in the MenuPage companions with number of MenuItam values. It contains 66,937 rows of data. Should be check each referred menu ID and MenuItem ID are correctly exist in the Menu and MenuItem datasets.
  3. MenuItem data file
Each row of the data in MenuItem data file provides information, price and date, about an item and refers to a MenuPage and a Dish in the Dish data file. It contains 1,332,726 rows of data.
  4. Dish data file
Each row data in Dish data file contains information about a kind of food dish with a specified ID number. The information contains: range of price, and number of times the dish appeared in the MenuItems data file and the range of date of the appearance. It contains 423397 rows of data.
