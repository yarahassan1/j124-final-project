# JOURN124 - Final - Project
### By: Yara Hassan, UC Berkeley 2027 
### B.A. Data Science, B.S. Environmental Economics and Policy

## The Same Foods In Every American Grocery Cart, SNAP or Not

## Data Acquisition and Summary:

A commonly debated topic in the United States is access to the Supplemental Nutrition Assistance Program, also known as SNAP. SNAP is a federal food-assistance program that helps low-income households buy groceries using monthly funds loaded onto an Electronic Benefits Transfer card. Currently, SNAP restricts purchases of hot prepared foods, alcohol, tobacco, and non-food items. However, many Americans believe the program does not do enough to ensure that benefits are used for foods with nutritional value.

In 2025, a poll from the Center for Excellence in Polling showed that 58% of likely voters in the U.S. supported limiting the types of foods that can be purchased with food stamps to foods with high nutritional value. This would add items such as sugary beverages, candy, and pre-packaged desserts to the list of restricted foods (Taylor, PhD).

The dataset used in this analysis comes from a 2016 USDA study that examined food purchases made by households receiving SNAP benefits compared to non-SNAP households. The purchase data was collected at the point of sale in 2011 from a leading grocery retailer. According to the USDA, the data came from supermarkets, grocery stores, and food-and-drug stores. However, warehouse club stores, specialized food stores, and convenience stores were not included.

For this study, a transaction was considered to be associated with a SNAP household if SNAP was used to pay for at least half of the total purchase. This definition creates some limitations. For example, it does not include transactions where SNAP was used for less than half of the purchase, and it does not show which specific items were paid for using SNAP versus another payment method such as cash, debit, or credit.

The USDA can generally be viewed as a trustworthy source because it is a government agency, but the dataset still has important limitations. First, the data comes from only one retailer group, so it does not represent all SNAP-authorized stores in the United States. Second, the data is from 2011, meaning it is likely outdated, since shopping behaviors may have changed over the past decade. Third, because SNAP is a politically controversial program, the way the data is interpreted could be influenced by debates over whether taxpayer money should fund certain types of food purchases.


## Data Analysis: 

See the full analysis in my notebook: [JOURN_124_Final_Project.ipynb](./JOURN_124_Final_Project.ipynb)

## Two Data Visualizations:

### Chart 1: Top 10 Commodities — SNAP Households
![Top 10 SNAP commodities](./chart%201.png)
Soft drinks are the single largest category at 5.44% of all SNAP spending, followed by fluid milk products (3.85%) and beef:grinds (3.05%).

### Chart 2: Top 10 Commodities — Non-SNAP Households
![Top 10 non-SNAP commodities](./chart%202.png)
Fluid milk products lead at 4.03%, with soft drinks close behind at 4.01%. 7 of the top 10 commodities are identical between groups.


## Ending summary, ethical concerns, reporting process:

The key finding of both the original USDA study and my own analysis is that there are minimal differences between SNAP and non-SNAP households when it comes to grocery purchases. The top commodities are largely the same for both groups, and staples like soft drinks and fluid milk products dominate spending regardless of SNAP status. Even where the two groups diverge the most, which I identified through the rank_gap, the differences show up in categories that represent a small share of total spending, not in the commodities that actually drive most grocery spending overall.

This has real ethical relevance. A significant portion of the ongoing political debate over SNAP assumes that recipients disproportionately use benefits on unhealthy food. This belief is significant enough that some polling has found majority support for restricting SNAP purchases to items with clear nutritional value, and several states have already begun implementing bans on soda and candy SNAP purchases. Yet this dataset complicates that assumption by showing that non-SNAP households' top 10 commodities actually included more less-nutritional items, such as ice cream, coffee creamer, and packaged candy, than SNAP households' top 10 did. While fluid milk narrowly tops soft drinks as the top commodity for non-SNAP households, the margin is minimal, at 4.03% versus 4.01% of total spending. This means both groups spend about the same amount on soft drinks.
Taken blindly, this data could risk being used to stigmatize SNAP recipients based on assumptions that are not well supported by the purchase data itself. For example, someone could argue that SNAP recipients' top purchase is soft drinks while non-SNAP households' top purchase is milk, and then use that to support the argument that SNAP recipients make worse food choices than everyone else. However, that ignores how small the difference actually is and how similar the overall spending patterns are between the two groups.

As noted earlier, this dataset has constraints on what it can tell us. It reflects purchases from a single retailer, so it is not a nationally representative sample of all SNAP-authorized stores. It also classifies a transaction as “SNAP household” spending only when SNAP covers at least half of the purchase total. Additionally, the data is from 2011, which is over a decade old, so it may not reflect current shopping patterns.
To make this a more complete and current piece of journalism, I would want to reconduct the study using more modern purchase data, ideally from multiple retailers across different regions, to check whether this “minimal difference” finding still holds today. I would also want to interview SNAP recipients directly about their shopping decisions and constraints, rather than relying only on purchase data, which cannot capture the reasoning behind a purchase. Lastly, I would look at outcomes in the states that have already implemented soda and candy restrictions, since real-world data on those policies would meaningfully contribute to this debate.

## Works Cited

“Foods Typically Purchased by Supplemental Nutrition Assistance Program (SNAP) Households.” Food and Nutrition Administration, United States Department of Agriculture, 24 January 2025, https://www.fna.usda.gov/research/snap/foods-typically-purchased-supplemental-nutrition-assistance-program-snap-households.

Taylor PHD, Travis N. “Voters Support Banning Junk Food Purchases with Food Stamps.” A project of the Foundation for Government Accountability, Center for Excellence in Polling, 24 March 2025, https://excellenceinpolling.com/poll/voters-support-banning-junk-food-purchases-with-food-stamps/.

“USDA SNAP Spending Study.” Data Is Plural, Data Is Plural, 18 January 2017, https://github.com/data-is-plural/usda-snap-spending-study/tree/master.


