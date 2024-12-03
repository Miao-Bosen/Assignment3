# Assignment3 Presentation
Miao Bosen, Riley Andreachuk



# Introduction
When it comes to agricultural products, eggs must be one of those things that come to your mind. It is undoubtedly one of the most popular food worldwide due to its high nutritional value, delicious taste and affordable price. In this project, we will work on the price of eggs and discover its correlation with countries’ GDP.


# Analysis
def scrape_table(table):
    df = pd.read_html(str(table))
    df = pd.DataFrame(df[0])
    return Table.from_df(df)


# The reason why we choose GDP as the external factor
A high GDP often means higher productivity and demand, which can affect egg prices. GDP is also related to several concepts like inflation and international trade. We believe that GDP is not a direct factor in determining egg prices, but it can indirectly affect it through various mechanisms such as supply and demand, production costs, and policies.


![IMG_0153](IMG_0153.png)


![IMG_0154](IMG_0154.png)


![IMG_0152](IMG_0152.png)


![IMG_0155](IMG_0155.png)
