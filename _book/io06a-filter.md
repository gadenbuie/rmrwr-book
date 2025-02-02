---
title: "Wrangling Rows in R with Filter"
author: "Peter Higgins"
date: "12/15/2020"
output: html_document
---


# Wrangling Rows in R with Filter
In this chapter, we will introduce you ways to wrangle rows in R. You will often want to focus your analysis on particular observations, or rows, in your dataset. This chapter will show you how to include the rows you want, and exclude the rows you don't want. 
Once your data wrangling and data validation is done, you will be ready for data analysis.

## Filtering on Numbers - Starting with A Flipbook

If you have not used a flipbook before, you can **click** on the frame below to activate it, then use **right and left arrow keys** to move forward and back through the demo. 

With each forward step in the code on the left, examine the resulting output on the right. Make sure you understand how the output was produced.

<!---FLIPBOOK EX 1-->

<iframe style="margin:0 auto; border: solid black;" id="myIframe1" width="763" height="432" src="https://higgi13425.github.io/mini_flipbooks/filter_microflip_1_num.html#1" scrolling="no">
</iframe>

<!---FLIPBOOK EX 1-->

### Your Turn - learnr exercises

<!---LEARNR TUTORIAL EX 1-->
<iframe style="margin:0 auto; border: solid black;" id="myIframe2" width="763" height="763" src="https://higginslab-rshiny.med.umich.edu/shiny-apps/learn_filter1/" scrolling="yes">
</iframe>
<!---LEARNR TUTORIAL EX 1-->


## Filtering on Multiple Criteria with Boolean Logic 

You can use multiple filters on your data, and combine these with 
AND
OR
XOR
parentheses
and combinations thereof.

<!---FLIPBOOK -->

<iframe style="margin:0 auto; border: solid black;" id="myIframe3" width="763" height="432" src="https://higgi13425.github.io/mini_flipbooks/filter_microflip_2_boolean.html#1" scrolling="no">
</iframe>

<!---FLIPBOOK  -->

### Your Turn - learnr exercises

<!---LEARNR TUTORIAL EX 2-->
<iframe style="margin:0 auto; border: solid black;" id="myIframe4" width="763" height="763" src="https://higginslab-rshiny.med.umich.edu/shiny-apps/learn_filter2/" scrolling="yes">
</iframe>
<!---LEARNR TUTORIAL EX 2-->


## Filtering Strings 

You can use == to test exact equality of strings, but you can also use str_detect from the {stringr} package, and combine it with the magic of regex to do complicated filtering on character string variables in datasets. 

<!---FLIPBOOK -->

<iframe style="margin:0 auto; border: solid black;" id="myIframe5" width="763" height="432" src="https://higgi13425.github.io/mini_flipbooks/filter_microflip_3_string.html#1" scrolling="no">
</iframe>

<!---FLIPBOOK  -->

Test the strings

### Your Turn - learnr exercises

Strings learnr here



## Filtering Dates 

You can use the {lubridate} package to format strings for logical tests, and filter your observations by date, month, year, etc. 

<!---FLIPBOOK -->

<iframe style="margin:0 auto; border: solid black;" id="myIframe7" width="763" height="432" src="https://higgi13425.github.io/mini_flipbooks/filter_microflip_4_dates.html#1" scrolling="no">
</iframe>

<!---FLIPBOOK  -->

### Your Turn - learnr exercises

Dates learnr here

## Filtering Out or Identifying Missing Data 

You can use the is.na(), drop_na() and negation with ! to help identify and filter out (or in) the missing data, or observations that are incomplete. 

<!---FLIPBOOK -->

<iframe style="margin:0 auto; border: solid black;" id="myIframe9" width="763" height="432" src="https://higgi13425.github.io/mini_flipbooks/filter_microflip_5_na.html#1" scrolling="no">
</iframe>

<!---FLIPBOOK  -->

### Your Turn - learnr exercises

NA learnr here

## Filtering Out Duplicate observations 

You can use the {janitor} package to help you find duplicated observations/rows for fixing or removal from your dataset.

<!---FLIPBOOK -->

<iframe style="margin:0 auto; border: solid black;" id="myIframe11" width="763" height="432" src="https://higgi13425.github.io/mini_flipbooks/filter_microflip_6_dupes.html#1" scrolling="no">
</iframe>

<!---FLIPBOOK  -->

### Your Turn - learnr exercises

Dupes learnr here

## Slicing Data by Row

You can use the _slice()_ family of functions to cut out a chunk of your observations/rows by position in the dataset.

<!---FLIPBOOK -->

<iframe style="margin:0 auto; border: solid black;" id="myIframe13" width="763" height="432" src="https://higgi13425.github.io/mini_flipbooks/filter_microflip_7_slice.html#1" scrolling="no">
</iframe>

<!---FLIPBOOK  -->

Slice learnr here

## Randomly Sampling Your Rows

You can use the _slice_sample()_ function to take a random subset of large datasets, or to build randomly selected training and testing sets fo modeling.

<!---FLIPBOOK -->

<iframe style="margin:0 auto; border: solid black;" id="myIframe15" width="763" height="432" src="https://higgi13425.github.io/mini_flipbooks/filter_microflip_8_sample.html#1" scrolling="no">
</iframe>

<!---FLIPBOOK  -->

### Your Turn - learnr exercises

Sample learnr here
