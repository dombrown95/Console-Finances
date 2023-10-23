# Console-Finances summary

This repository holds the HTML and JavaScript code for the Week 4 console finances challenge.

The purpose of this project is to create code to analyse the financial records of a company. A financial dataset has been provided and is composed of arrays with two fields — 'Date' and 'Profit/Losses'

The included code calculates:

* The total number of months included in the dataset.
* The net total amount of Profit/Losses over the entire period.
* The average of the changes in Profit/Losses over the entire period.

The live site can be found at the below URL:

https://dombrown95.github.io/Console-Finances/

An image of the live site and console results can be seen below: 

<img src="/images/Screenshot 2023-10-23 151209.png">


# Congifuration/Customisation

The provided code is not specific to the included dataset and can be used to calculate further results from different datasets. 

If users would like to use the code for their own dataset, it should follow a similar format of 'Date' and 'Profit/Losses' (e.g. 'Dec-2012', 359333). The first field should be a string and the second field should always be in the form of a number, as concatenation is used to append the results.

# Issues/Limitations

I initially struggled to identify the correct formulas to calculate the required results, but researching via StackOverflow/Google and separating the process into sections by commenting on my code helped.

Although my code seemed to work intially and the majorty of the values were identical to the reults provided, I did notice that one of the values (Average Change) was quite different. I eventually managed to resolve this with help from a class mate (credited in the below 'Resources' section).

# Resources used -

I used a line of code provided by a classmate (Emma Blencowe) to fix an issue with the 'Average Change' value not calculating correctly -

        sumOfChange += finances[i][k] - finances[i - 1][k];

Links Used - 

Printing to nearest 100 - 
https://stackoverflow.com/questions/19621455/how-to-round-up-to-the-nearest-100-in-javascript

Concatenation - 
https://stackoverflow.com/questions/16124032/js-strings-vs-concat-method

Calcularing average change in JS -
https://stackoverflow.com/questions/21561582/debug-javascript-code-to-calculate-average-then-assign-letter-grade?rq=1

Average rate of change in a dataset - 
https://math.stackexchange.com/questions/55913/question-about-rate-of-change-given-a-set-of-data
