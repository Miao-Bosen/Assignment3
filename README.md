# Presentation
Miao Bosen, Riley Andreachuk

CCID:bmiao1, randreac



# Introduction
When it comes to agricultural products, eggs must be one of those things that come to your mind. It is undoubtedly one of the most popular food worldwide due to its high nutritional value, delicious taste and affordable price. In this project, we will work on the price of eggs and discover its correlation with countries’ GDP.


# Analysis
Here is our work on the [Google Colab](Presentation.ipynb)

![image](https://github.com/user-attachments/assets/989ee7be-cd9c-4de2-9106-04252fcafba1)

We create a BeautifulSoup object first. Then the second line allows us to search for a table within the link provided within beautiful soup. Finally the census_table finds the specific table we are looking for.

This gives us the following table

![image](https://github.com/user-attachments/assets/690158b9-b901-44b9-8e93-1ac14f7ddb90)


We only need 10 countries for this project, this line picks 10 from the table, including Canada.

![image](https://github.com/user-attachments/assets/45a44b88-940c-413b-a047-ff0c84a4926d)

Which gives us this table

![image](https://github.com/user-attachments/assets/cc55c856-24dc-45bd-b5a8-591ca465fef8)

Because of the table being in USD we are tasked with converting it back into local price with currency symbols.

![IMG_0172](IMG_0172.jpeg)

First of all, we list the exchange rates for these ten counrtries.

Since the table we imported does not have "Local" prices of eggs, we need to deifine a function tp work backwards and get that information.
 
 By using the 'if', we set what would happen if a currency symbol from the table matches one from the exchange rates

The currency line here creates a list of all the converted currencys, extracts the prices in usd and currency for a row,

Then we adopt the function to convert the prices to the local currency           

Here we use a with column function to create a new column and adds it to the original.



After converting everything to local price we have to add the currency symbols, we acheive this through the following to lines of Code

![image](https://github.com/user-attachments/assets/97319b26-b25f-4e20-98db-b77d7f87f826)

After applying all the code to the original table we get this.

![IMG_0173](IMG_0173.jpeg)

Next we have to add a column with all the prices converted to CAD ( Also dropping the useless "Rank" column

![image](https://github.com/user-attachments/assets/6943f21f-7b61-4bf5-b1a8-5717ab54827f)

After applying this code we get the following table

![image](https://github.com/user-attachments/assets/2df0e3b6-fa6e-456a-af3c-e834dfb9d5fe)

This is our fully cleaned data set

Next we are going to compare the eggs prices with the price in CAD

![image](https://github.com/user-attachments/assets/74d4f0d4-3c1a-4f09-a77e-1cde9d19e561)

After running this code and plotting it we can see the diffrence between the countries in relation to Canada

![image](https://github.com/user-attachments/assets/3d1c9355-377c-49b4-9fa3-ca0a0817a6ef)

#


Next is our external factor, each countries GDP

# The reason why we choose GDP as the external factor
A high GDP often means higher productivity and demand, which can affect egg prices. GDP is also related to several concepts like inflation and international trade. We believe that GDP is not a direct factor in determining egg prices, but it can indirectly affect it through various mechanisms such as supply and demand, production costs, and policies.


First we need to import a csv with the GDPs of all of our countries
![image](https://github.com/user-attachments/assets/e0be35ab-8875-4dbb-babb-3c5c95422a3e)
![image](https://github.com/user-attachments/assets/9c07e54f-f741-4a6c-9592-e7c7ea7e2bcc)


Then after this we join this table back with our original 

![image](https://github.com/user-attachments/assets/fe5305c0-9e71-427e-ab15-cd1dd00f8cf0)

We then use this information to plot it using a scatterplot

![image](https://github.com/user-attachments/assets/738e9d94-fe93-4966-bde8-077f165a49be)


The final step in our analysis would be to find the correlation bettween GDP and price of eggs

![image](https://github.com/user-attachments/assets/0f2b8fe1-d64f-409c-a0fd-e8529a52fc56)


# Conclusion
The main difficulty in this project is converting the price to each countries' local price.
According to the research, among the ten countries we selected, Costa Rica has the lowest price and Ghana has the highest price.
-0.2 indicates that there is a very weak negative linear relationship between countries' GDP and egg prices,which means GDP may not have an impact on the price.
