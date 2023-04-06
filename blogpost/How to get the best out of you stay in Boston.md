
# What makes the AirBnb's in Boston so expensive and how can you avoid paying that much?
![source: https://www.appsverse.com/blog/rent-out-your-house-on-airbnb/](https://www.appsverse.com/blog/content/images/size/w2000/2019/07/airbnb-visual-.png)
With more than 22 million tourists per year (22.7 in 2019), Boston is a frequently visited touristic city, therefore owners of an apartment in Boston can rent out their apartments and profit from the visits. But what makes an asset actually valuable and what if you could profit even more? This is going to be answered in this article.

If you don't own an apartment in Boston and and think that this article is just about rich people getting even richer, you are wrong. This analysis can be seen the other way round as well. I will show you the things, that makes an asset valuable, but as a tenant, you can simply avoid these things and save your self some money. In addition, I am going to show you, which time will be the best to visit Boston and spend less money on your stay but more money on Boston baked beans.

## The data
We analysed data from AirBnb from September 2016 to 2017 provided by AirBnB and Kaggle. The data set contained different data reaching from the number of rooms, to the location and other data for each listing, listed in the mentioned years. The following correlation matrix gives an impression of the numerical data that was available and how they correlate with each other.
![Correlationmatrix](https://raw.githubusercontent.com/KaanDrn/udacity_data_science_project1/main/blogpost/correlation.png)

As we can see, reviews correlate with each other, same goes for the prices, which seems not too surprising.
But now to the reason you made it until here:

## What makes the apartments so expensive?
As stated before, we want to know, what makes an asset valuable. To find that out a machine learning method was used to determine which data predicts the price the best. That leads to a set of data, that shows, what determines the price for an asset the best.
The method used here is Recursive Feature Elimination (RFE), where the features (input data) is used to predict the prices and with each iteration, a specific number of features are dropped. The feature that had the least impact on the prediction is dropped afterwards and the iteratuion begins again.
The results can be seen below.
![Most important features to predict the price](https://raw.githubusercontent.com/KaanDrn/udacity_data_science_project1/main/blogpost/images/value_of_properties%20.png)
We can see here that essentially the size (number of bedrooms, bed, bathrooms, etc.) and the location (latitude/logitude) have the highest impact on the price. 
As a homeowner, this may not be surprising. It seems like there is nothing to do, if you have a small apartment in a certain area of Boston it seems like the price is predetermined. But the truth lies in the next question.

## What can I do if I can't add more bedrooms?
The features detected in the previous chapter show, that the location and certain construction related aspects have an impact on the price. So what if you have no influence on the number of rooms or can't move your apartment to a more popular area? I got you covered.

To answer that, we split up the apartments into two subgroups, small apartments with 1-2 Bedrooms and bigger apartments with at least 3 Bedrooms and performed another RFE. In comparison to the previous analysis, we are going to include the amenities in the apartments as well. with these restrictions, we get the following feature set for small apartments.
![Feature set small apartments](https://raw.githubusercontent.com/KaanDrn/udacity_data_science_project1/main/blogpost/images/enhance_small_apartment.png)
And for bigger apartments we get the following:
![Feature set bigger apartments](https://raw.githubusercontent.com/KaanDrn/udacity_data_science_project1/main/blogpost/images/enhance_big_apartment.png)
This shows, that there are a few things you can influence to make your apartment more popular.
For small apartments it is appreciated if you provide some essentials and some small goodies, like a hair dryer, a smoke detector or if you simply allow pets. This can be implemented pretty easily.
For bigger apartments, it is a bit more complicated and cost intensive. Tenants of bigger apartments are looking for more luxury, like a dryer, an indoor fireplace or animals on the property. But you can still enhance your apartment if you provide Internet, a fire extinguisher or a first aid kit. 

In summary, even though construction related factors have the highest impact on the price, you can add some small goodies for you guests to make them pay for more. Or in other words, if you are willing to pass on some goodies, you can get your apartment for a better price.

## When to go?
So, now that you know on what you have to pass on, in order to get a great price, the remaining question is: When should you visit Boston? To answer that we analysed almost 3000 listings and found that the best time to go is in autumn. That's the reason why the prices are the highest here. If you want to save you some moey, you better visit Boston fro January to April. The prices are usually the lowest here.
The plot below shows how the prices differ in time. 
![Prices of apartments in Boston](https://raw.githubusercontent.com/KaanDrn/udacity_data_science_project1/main/blogpost/images/prices_year.png)
The plot also shows, that for pretty low priced apartments (about 100\$-150\$) it does not make a hughe difference.

## Conclusion
In conclusion, we can say that if you want to have a great time in Boston but do not have a lot of money, you should visit Boston from January to April. For your apartment, you should skip on some of the goodies provided by the owner and bring your own hair dryer. 
As a home owner, the opposite applies, if you provide some of the amenities mentioned above, you can simply get more money out of the same asset.

You now know what you have to look for in an apartment in Boston to save you some money. The only thing left for me to say is: enjoy your beans!