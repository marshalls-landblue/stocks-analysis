# VBA Unit

## Overview of Project

### Purpose

This analysis is designed to help quickly look at large amounts of stock information for a given company in a given year. This is something that can take a long time to look up individually so we employ the use of macros to get the job done. 

### Background

Previously, we designed a script that can collect the data for a specific year based on data entry. This code was working fine but it required havin static values inserted into the script, the goal of this tool is to improve upon that by making a more extendable script that can work for many different inputs in faster manner.

## Results

I successfully refactored the script to be able to process these results very quickly. See these screenshots for detailed statistics on these 12 tickers for the years 2017 and 2018, respectively.

![image](https://user-images.githubusercontent.com/17416097/149719473-d2c43635-bc0f-483f-87d4-3032f7c3484c.png)

![image](https://user-images.githubusercontent.com/17416097/149719684-6f4444c9-7c7c-430b-b6b3-71a4a1a6f4d2.png)

Based on the data, you can notice that these stocks had much better returns in the year 2017. Most of the them went down in 2018, except for ENPH and RUN which had substantially more volume than the other stocks. The volume also changed very little, but was allocated to the tickers differently

The refactored code ran over 10x more quickly than the original script, this is because it utilizes the for loops and the iterator to save a lot of complexity and stores a lot less information.

![image](https://user-images.githubusercontent.com/17416097/149720906-54ccb183-518b-4a9f-882f-42a580370d24.png)


## Summary

Refactoring code has advantages and disadvantages. It is extremely helpful to expand on an existing codebase to save time and energy of starting from scratch. it is a great tool to aide colaboration between teammates working on the same project. It is also always good to keep in mind what can be changed about your code to make it solve a different problem or operate more efficiently. Sometimes refactoring can make your project difficult, because you find yourself locked in to a certain structure or method of solving the problem, when you would have gone about it in a different way. For me, I found it really refreshing to be able to start on our existing code and not have to redo some of the formatting and variable declaration we had already set up earlier. I did however, feel a little trapped to write the script in a certain way, for example hardcoding the tickers in, instead of dynamically adding them to the array when found in the loop.
