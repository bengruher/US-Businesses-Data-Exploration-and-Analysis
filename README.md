# US-Businesses-Analysis

This project originated from a graduate Data Science course at Seattle University. My notebook as well as the original dataset are located in this repository. This README contains the original assignment. My answers to the below questions are located in my notebook. 


For this exercise you will pull together data from threedifferent sources, and use that data to do some analysis about the relationships between businesses, the kind of business, where the business is located, and the population and income of where it is located. Your data comes in threefiles The first file businesses.tsv gives you some information about some of the businesses the companyknows about.  This is a sample of approximately 100K business;  there are approximately 18M businesses in the full data set.  Also, the full data set has rich informationabout each business.  

For this exercise all we are giving you is 
a.A unique ID for the business (a UUID) 
b.The NAICS codes for the business (there can be more than one code per business) 
c.The zip code in which the business is located 

This is a sample of 100000businesses that are claimed to have been sampled from the 50 US states and the District of Columbia. The NAICS code is a classification of what a business does.  A business might have more than one code, and if it does,that will appear as more than one line in the file with the same business ID.  There are records with a business ID, a zip code, but no NAICS code.  Those recordsshould be interpreted as a real business located in the zip code, but for which we have no NAICS codes. Any NAICS code appearing in the businesses file that has a missing or unrecognized NAICS code should be considered as being in the category UNKNOWN.

NAICS codes also have a descriptive name, and that mapping from code to name appears in the second file,naics_codes.txt.This is a CSV file downloaded directly from the web.  You will notice that the codes in the businesses files are generally longer than two characters, wheras the codes in this file are all exactly two characters.  That is because we are focusing only on the24 top-level codes(also called two-character or sector codes) 
http://www.census.gov/cgi-bin/sssd/naics/naicsrch?chart=2012.For a longer (full)code in the businesses file, the sectorcode is the first two characters in the full codeThe third file zip_demographics.txt contains demographic data about postal codes, in particular the median and mean income for the zip code, the zip code’s population, and the state in which the zip code is located. 

A big part of this exercise is understanding, interpreting, and cleaning the data.  Consider the description above what the data set is supposed to be like.  You have to think hard about whether or not the data in the files conforms to thedescription, and if not, what you should do about it in the cleaning and EDA phases.Use data in these files to do the following: 

1.What kind of data cleaning and error checking did you do in processing the files, what challenges did you find, and what did you do about those challenges? What assumptions did you make about the data attributes?  Please address these issues in some detail.  

2.Considering only the top-level NAICS categories, produce a graphic of your choiceshowing the number of businesses per category and also showing the percentage of businesses in each category. 

3.Consider now aggregating data up to the state level.   Which states have the most and least number of businesses per capita? Show this in a graphic that communicates the information for all states, but also indicates to the viewer the states with the most and least number of businesses per capita.

4.Staying at the state level, look more carefully at the Health Care category.  What state has the most and what state has the least concentration of health-care businesses, where concentration is defined as the percentage of total businesses in the state that are in the health-care category? Show a table with the information about all states that highlights the stateswith the most and least concentration.

5.Does the data support the claim that the state of New Hampshire has a lower concentration of health-care businesses than the country as a whole? Why or why not?6.Do an analysis on the quantity mean per capita income per state.  What does the distribution of this attribute look like?  Is it skewed?  Are there outliers?
