# JOURN 124  Final Project
By: Yara Hassan - UC Berkeley 2027, 
B.A. Data Science, B.S. Environmental Economics and Policy

# SNAP or Not - The Same Foods In Every American Grocery Cart

## The United States' Supplemental Nutrition Assistance Program (SNAP)

A commonly debated topic in United States politics is the Supplemental Nutrition Assistance Program, also known as SNAP. SNAP is a federal food-assistance program that helps low-income households buy groceries. Households under the SNAP program receive monthly funds that are loaded onto an Electronic Benefits Transfer (EBT) card, and can be used at authorized merchants to purchase select food items. Currently, SNAP prohibits purchases of hot prepared foods, alcohol, tobacco, and non-food items. However, many Americans believe the program does not do enough to ensure that funds are used toward foods with nutritional value, and there is a stigma that individuals under the program use funds for unhealthy food choices. 

In 2025, a poll from the Center for Excellence in Polling showed that 58% of likely voters in the U.S. supported limiting the types of foods that can be purchased with food stamps to foods with high nutritional value. This would add items such as sugary beverages, candy, and pre-packaged desserts to the list of restricted foods (Taylor, PhD).

## Data Acquisition:

The dataset used in this analysis comes from a 2016 USDA study, which examined food purchases made in 2011 by 26.5 million different households receiving SNAP benefits, compared to non-SNAP households. The purchase data was collected at points of sale from a leading grocery retailer. According to the USDA, the data came from supermarkets, grocery stores, and food-and-drug stores; however, warehouse club stores, specialized food stores, and convenience stores were not included.

For this study, a transaction was considered to be associated with a SNAP household if SNAP was used to pay for at least half of the total purchase. This definition creates some limitations. For example, it does not include transactions where SNAP was used for less than half of the purchase, and it does not show which specific items were paid for using SNAP versus other payment methods such as cash or debit/credit cards. 

The USDA can generally be viewed as a trustworthy source because it is a government agency, but the dataset still has some significant limitations. First, the data comes from only one retailer group, so it does not represent all SNAP-authorized stores in the United States. Second, the data is from 2011, meaning it is likely outdated, since shopping behaviors may have changed over the past decade. Third, because SNAP is a politically controversial program, the way the data is interpreted can be influenced by debates over whether taxpayer money should fund the program and certain types of foods.


## Data Analysis: 

See the full analysis in my notebook, which includes code and markdown text cells: [JOURN_124_Final_Project_Notebook.ipynb](./JOURN_124_Final_Project_Notebook.ipynb)

## Two Data Visualizations:

### Chart 1: Top 10 Commodities — SNAP Households
![Top 10 SNAP commodities](./chart%201.png)

This visualization shows the top 10 commodities in SNAP households. Soft drinks are the single largest category at 5.44% of all SNAP spending, followed by fluid milk products (3.85%) and beef:grinds (3.05%).

### Chart 2: Top 10 Commodities — Non-SNAP Households
![Top 10 non-SNAP commodities](./chart%202.png)

This visualization shows the top 10 commodities in non-SNAP households. Fluid milk products lead at 4.03%, with soft drinks close behind at 4.01%. 7 of the top 10 commodities are identical between groups.


## Ending Summary, Ethical Concerns, Reporting Process:

The key finding for both the original USDA study and my own analysis is that there are minimal differences between SNAP and non-SNAP households when it comes to grocery purchases. The top commodities are largely the same for both groups, and staples like soft drinks and fluid milk products dominate spending regardless of SNAP status. Even where the two groups diverge the most, which I identified through the rank_gap column, the differences show up in categories that represent a small share of total spending, not in the commodities that drive most of spending.

The results of this study are ethically relevant as a significant portion of the ongoing political debate over SNAP assumes that recipients disproportionately use benefits on unhealthy foods. This belief is significant enough that some states have begun implementing policies for restricting SNAP purchases to items with clear nutritional value, with bans on items like soda and candy. Yet this dataset challenges this argument because it shows that non-SNAP households' top 10 commodities actually included more lower-nutrition items, such as ice cream, coffee creamer, and packaged candy, than SNAP households' top 10 did. While fluid milk narrowly tops soft drinks as the top commodity for non-SNAP households, the difference is minimal, at 4.03% versus 4.01% of total spending. 

If a broad statement were to be made using this data, it can continue to stigmatize SNAP recipients. For example, someone could argue that SNAP recipients' top purchase is soft drinks while non-SNAP households' top purchase is milk, and then use that to support bans with the argument that SNAP recipients make worse food choices than everyone else. Yet, that ignores how small the difference actually is and how similar the overall spending patterns are between the two groups.

It is also still important to note that any conclusions derived from this dataset must acknowledge the limitations mentioned earlier. The data only reflects purchases from a single retailer, so it is not a nationally representative sample of all SNAP-authorized stores. It also classifies a transaction as “SNAP household” spending only when SNAP covers at least half of the purchase total. Additionally, the data is from 2011, which is over a decade old, so it may not reflect current shopping behaviors.

To make this a more complete and current piece of journalism, I would want to redo the study using more modern purchase data, from multiple retailers across different regions. I would also want to interview SNAP recipients about their shopping decisions and constraints, to understand the reasoning behind their purchases. Lastly, I would look at outcomes in the states that have already implemented soda and candy restrictions to see how policy impacts purchase data. 


## Works Cited

“Foods Typically Purchased by Supplemental Nutrition Assistance Program (SNAP) Households.” Food and Nutrition Administration, United States Department of Agriculture, 24 January 2025, https://www.fna.usda.gov/research/snap/foods-typically-purchased-supplemental-nutrition-assistance-program-snap-households.

Taylor PHD, Travis N. “Voters Support Banning Junk Food Purchases with Food Stamps.” A project of the Foundation for Government Accountability, Center for Excellence in Polling, 24 March 2025, https://excellenceinpolling.com/poll/voters-support-banning-junk-food-purchases-with-food-stamps/.

“USDA SNAP Spending Study.” Data Is Plural, Data Is Plural, 18 January 2017, https://github.com/data-is-plural/usda-snap-spending-study/tree/master.


