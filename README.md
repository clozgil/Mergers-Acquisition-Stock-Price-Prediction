*The Notebook contains links that don't operate on Github. It is recommended to view the project below:*
https://nbviewer.org/github/clozgil/Mergers-Acquisition-Stock-Price-Prediction/blob/main/Mergers%20%26%20Acquisition%20-%20Stock%20Price%20Prediction.ipynb

# Introduction

This project looks at the mergers and acquisitions of 30 publicly traded companies and attempts to determine the stock price at closing. M&As are incredibly difficult to assess, and while the company's instrinsic value and fundamentals play a significant role in predicting whether a merger will be "successful", public sentiment from Wall Street investors is another commonly referenced topic. 

Brainstorming for this project prompted two notable observations; data on M&As are often incomplete and highly inconsistent given the confidentiality behind these deals, and determining an appropriate dependent variable y for analysis presents a significant challenge (would most likely require an additional project on its own). The success of a merger could be measured various ways, but often times the unpredictability of management makes all the more challenging. Culture, reorganization, and leadership shake-up are all attributes that play an important role in the success of an M&A but are difficult to quantify. 

Although I do build and run a model in this proejct, the complexity around this subject urged me to focus primarily on data gathering and manipulation. Since one would most likely need to compose a dataframe with the attributes necessary to run an a useful analysis on Mergers and Acquisition, I believe this is a valuable first step.

For a more balanced notebook between EDA, data manipulation, and models, I have a project that focuses on COVID19's impact on Post-Secondary Education below titled **COVID19 Effects on Post-Secondary Education**

https://nbviewer.org/github/clozgil/COVID19-Effects-on-Post-Secondary-Education/blob/main/COVID-19%20Effects%20on%20Post-Secondary%20Education.ipynb

## The Process

My objective was to build a dataframe with useful attribtues from scratch. I found that three reports per company would have sufficient information to get started.
- Acquistion data (any and all information on the company's M&A)
- Financial ratios (data to determine the company's fundamentals)
- Stock information (data to gain insight into Wall Street sentiment)

Since downloading, importanting, and cleaning each one of those files for each of the 30 companies would be cumbersome, I looped on all the data files using the `OS` module, simulteanously cleaning and merging each one of the files.

However, for the purpose of this presentation, I will feature each one of my data cleaning techniques for one company - **Apple**.

## Data Sources

**For reference only. All necessary data for this project can be found in the `data` dictionary**

Acquisition data: https://www.capitaliq.com/CIQDotNet/my/dashboard.aspx
*

Financial ratios:
https://www-mergentonline-com.pitt.idm.oclc.org/companyfinancials.php?pagetype=ratios&compnumber=46247&period=Quarters&range=50&Submit=Refresh&csrf_token_mol=3680683535
*

Stock info:
https://www-mergentonline-com.pitt.idm.oclc.org/equitypricing.php?pagetype=report&compnumber=46247
*

(*) = Account required. University of Pittsburgh account used for access
