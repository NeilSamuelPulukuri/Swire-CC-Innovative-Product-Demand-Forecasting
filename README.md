# Swire-CC-Innovative-Product-Demand-Forecasting

<img width="182" alt="image" src="https://github.com/NeilSamuelPulukuri/Swire-CC-Innovative-Product-Demand-Forecasting/assets/141296161/0cbfefb3-2093-471c-8c98-418ca003a22e">


## Business Problem & Problem Objective

Swire Coca-Cola faces a business challenge in optimizing production planning and inventory management for its innovative beverage products segment. The innovative products that Swire plans to launch differ from historical sales. This is a similar kind of problem Swire Coca-Cola has faced in the past, where for one product, they had overproduced, leaving their inventory overstocked, and in another instance, they produced too few products, resulting in a lack of supply to meet the demand, and this incurred a loss. Now, they are introducing seven innovative products and want to know how many units to produce, as well as the best times of the year and regions to launch them. The project aims to build a robust machine-learning model that can predict the best 13 weeks of the year and the forecasted sales for those weeks.

## Group Solution
The products we were dealing with were innovative and did not have an exact match with the historical sales data. To solve this problem, we decided to filter the data by the products attributes (Flavor/category/caloric segment/package/manufacturer/brand). It was not possible to apply all the filters. Hence, we decided to go with the order of Flavor, Manufacturer, caloric segment, and category. Again, for some products, the maximum filter was three. The order of priority was flavor, which is crucial for any soft drink company, followed by the manufacturer, since the project is about Swire products, then by the caloric segment to know the consumer preferences. Healthy customers choose diet while other customers select primarily regular, and the last filter is the category to know whether the consumer is more inclined towards energy or sparkling water or SSD category. We assumed that we would be considering the best 13 consecutive weeks to know which season the product has to be launched and we also assumed unit sales over dollar sales since the problem is about forecast demand of products. Our goal was to build at least two machine learning models for each question so that we can validate the performance based on evaluating the error metric and then picking the best model for prediction.

## Personal Contribution
As the project was complicated, task distribution was essential. I was tasked with solving two out of seven questions and performing an exploratory data analysis for a specific question. The strategy I followed involved filtering the data based on innovative product attributes. The first question I solved was by filtering the data based on flavor, manufacturer, and caloric segment. There was a negative spike in the forecasted unit sales. Further analysis suggested that Swire had not experimented sufficiently with this flavor, hence there was a negative peak that was carried forward to the forecasted sales. The second question I solved followed a similar pattern but considered regions. For both questions, I developed three machine learning models: SARIMA, Exponential Smoothing, and Prophet. The Prophet model proved to be the most effective for both questions. Since it is time series data, the error metric I considered was Mean Absolute Percentage Error (MAPE). In addition, I took the initiative to combine all the notebooks of my teammates, made the final edits to the consolidated modeling notebook, and also prepared the content for the presentation.

## Business Value
The solutions provided by our team will help Swire make the right decisions on innovative products. All seven questions about the innovative products were answered. We built a robust machine-learning model that can be reused. We went further by calculating the overage and underage cost of the forecasted sales, which would help the Swire team get the full picture of the innovative products. Additionally, we suggested the best season of the year and regions for product launches. Overall, the results provided by our team would directly impact on Swire's product sales and help them make the right decisions. We structured the project in such a way that the data team could understand the trend of the forecasted sales, management could understand the effects of excess and shortage for the innovative products. In addition to this, we also did a sentimental analysis of the historical products to understand the consumer preference. My team believes that this sentimental analysis can be implemented for innovative products in the future.

## Challenges Encountered
One of the main challenges we encountered as a team was dealing with large amounts of data. We had to work on nearly 4GB of data. We tried to work with parquet files, but we observed that there was a data loss; we also tried pyspark, but it was way too expensive. To tackle this problem, there was no other way than to filter the data and also pivot the consumer demographics dataset to avoid complications while joining the datasets. The second biggest challenge was how to validate the models and which error metric to use. We decided to follow an 80-20 train test split and validate the models. The model with the least error was then picked and used to forecast the unit sales. The third biggest hurdle for me personally was time because I believe that this is a complicated data science problem that actually requires data experts to solve the problem, and my team took the extra initiative of doing research and working out late nights to get the job done.

## Learnings
Throughout the capstone project, I acquired the skillset of handling time series data, validating forecast models, and using them to predict forecasted sales. Apart from this, I gained hands-on knowledge of the concepts of overage and underage costs and how they help the business grow and make accurate decisions. From visualizing in Python and Power BI to building complex machine learning models and converting these results into business value information, this has been a step up in my career path. Apart from the technical skills, I also learned the importance of communication, and to my surprise, this non-technical skill was a game-changer for our team. Through communicating, we ensured our objectives were clear and all team members were on the same page.








