# Presentation
Miao Bosen, Riley Andreachuk

CCID:bmiao1, randreac


# Introduction
When it comes to agricultural products, eggs must be one of those things that come to your mind. It is undoubtedly one of the most popular food worldwide due to its high nutritional value, delicious taste and affordable price. In this project, we will work on the price of eggs and discover its correlation with countries’ GDP.


# Analysis
Here is our work on the [Google Colab](Presentation.ipynb)

![IMG_0169](IMG_0169.jpeg)

We create a BeautifulSoup object first. Then the second line allows us to search for a table within the link provided within beautiful soup. Finally the census_table finds the specific table we are looking for.


![IMG_0170](IMG_0170.jpeg)

We only need 10 countries for this project, this line picks 10 from the table, including Canada.

![IMG_0171](IMG_0171.jpeg)

 Here we list all the curencys we need for our table (Made the array in order), then we make another column with the currency symbols.

![IMG_0172](IMG_0172.jpeg)

![IMG_0173](IMG_0173.jpeg)

![IMG_0174](IMG_0174.jpeg)

![IMG_0181](IMG_0181.jpeg)

![IMG_0175](IMG_0175.jpeg)

![IMG_0176](IMG_0176.jpeg)

![IMG_0177](IMG_0177.jpeg)

![IMG_0178](IMG_0178.jpeg)

![IMG_0179](IMG_0179.jpeg)

![IMG_0180](IMG_0180.jpeg)





# The reason why we choose GDP as the external factor
A high GDP often means higher productivity and demand, which can affect egg prices. GDP is also related to several concepts like inflation and international trade. We believe that GDP is not a direct factor in determining egg prices, but it can indirectly affect it through various mechanisms such as supply and demand, production costs, and policies.




# Conclusion
The main difficulty in this project is converting the price to each countries' local price.
According to the research, among the ten countries we selected, Costa Rica has the lowest price and Ghana has the highest price.
-0.2 indicates that there is a very weak negative linear relationship between countries' GDP and egg prices,which means GDP may not have an impact on the price.
