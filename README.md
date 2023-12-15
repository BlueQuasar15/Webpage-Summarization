# Webpage-Summarization
Follow this colaboratory link to [view the code](https://colab.research.google.com/drive/1Hm7aGFJ7raPZkofA0KbA4l7f9Kknq_HA?usp=sharing).<br>
This program takes a search query from the user and compiles the textual information of all the webpages that appear on the first page of the SERPs (Search Engine Result Pages). The application utilizes BART which is an abstractive summarization model, which is capable of understanding the information in the compiled text as a human would, and summarizes it in short.

## Background
When making a search on Google or any other search engine, we often find that the information is fragmented and spread across many different webpages. Or we may find ourselves in a situation where after reading through a whole web page we realize that it did not have the content we are looking for. Thus having a solution that automatically compiles different webpages and summarizes them would reduce human effort and save time, while filtering out filler text, ads and other irrelevant tokens from the actual information.

## Workflow
We used Selenium to automate the process of calling the top 'n' webpages for a given query and load all HTML documents in python. Then the HTML is parsed, cleaned and compiled into one single document.
We tried multiple summarization techniques and models, including algorithmic approaches like SVD, and Deep Learning approaches using Transformers, before finding the right fit.
The process of collecting text data from a user query is same for every approach, but the pre-processing steps as well as output differ for each method.
The link given at the top uses BART for summarization. [Click here](https://colab.research.google.com/drive/16893PRDLy3QbFXf4fqHPBWO2t1QDLbcv?usp=sharing) to check the result for an extractive summarization that was performed using Singular Value Decomposition and see how an Extractive model performs.
The links given contains the code for every step described above (From Information extraction to Summarization).
The outputs given by both the Extractive and Abstractive approaches can be compared manually. 
