# User Profiling and Segmentation Project

## Project Overview
This project focuses on user profiling and segmentation to enhance targeted ad campaigns, personalized marketing strategies, and improved customer service. By analyzing user data, we can identify distinct user segments and understand their characteristics, behaviors, and preferences. This information is crucial for tailoring strategies that meet diverse user needs.

## Objectives
The primary objectives of this project are:
1. **Improving Customer Service**: By understanding user segments, we can provide more personalized and efficient customer service.
2. **Personalized Marketing**: Tailoring marketing campaigns to align with the preferences and behaviors of different user segments.
3. **Product Recommendations**: Recommending products that match the interests and behaviors of specific user groups.

## Data Collection and Preprocessing
We utilized a dataset named `user_profiles_for_ads.csv`, which includes various demographic, behavioral, and interest-based features of users. The key columns in the dataset are:

- **Demographic**: Age, Gender, Location, Language, Education Level, Income Level
- **Behavioral**: Time Spent Online (hrs/weekday), Time Spent Online (hrs/weekend), Likes and Reactions, Followed Accounts, Click-Through Rates (CTR), Conversion Rates, Ad Interaction Time (sec)
- **Interests**: Top Interests

The dataset was preprocessed to handle categorical and numerical data, ensuring it was ready for analysis and clustering.

## Exploratory Data Analysis (EDA)
We began the EDA by visualizing the distribution of key demographic variables (Age, Gender, Education Level, Income Level) and behavioral patterns (Device Usage). The visualizations helped us understand the overall distribution and trends within the user data.

## Clustering for User Segmentation
To segment the users into distinct groups, we selected a subset of features that were most indicative of user preferences and behaviors. These included both demographic and behavioral features. We then applied the K-Means clustering algorithm to create user segments. The preprocessing involved one-hot encoding of categorical features and standardization of numerical features.

## Cluster Analysis and Naming
After clustering, we computed the mean values of numerical features and the mode for categorical features within each cluster to understand their defining characteristics. Based on these characteristics, we assigned meaningful names to each cluster:

1. **Weekend Warriors**: High weekend online activity, moderate likes and reactions, predominantly male, age group 25-34, income level 80k-100k.
2. **Engaged Professionals**: Balanced online activity, high likes and reactions, predominantly male, age group 25-34, high income (100k+).
3. **Low-Key Users**: Moderate to high weekend online activity, moderate likes and reactions, predominantly male, age group 25-34, income level 60k-80k, lower CTR.
4. **Active Explorers**: High overall online activity, lower likes and reactions, predominantly female, age group 25-34, income level 60k-80k.
5. **Budget Browsers**: Moderate online activity, lowest likes and reactions, predominantly female, age group 25-34, lowest income level (0-20k), lower CTR.

## Visualization of User Segments
To provide a visual representation of each segment's profile, we created a radar chart. This chart compares the mean values of selected features (Time Spent Online, Likes and Reactions, CTR, Conversion Rates) across the clusters, highlighting the distinctive characteristics of each segment.

## Findings and Insights
1. **Weekend Warriors** tend to be highly active online during weekends and have moderate engagement with content.
2. **Engaged Professionals** are highly engaged throughout the week, showing high levels of interaction and reactions, indicative of a well-engaged user base with substantial spending power.
3. **Low-Key Users** exhibit moderate online activity with lower engagement rates, possibly indicating a more reserved user group.
4. **Active Explorers** are predominantly female, with high overall online activity but lower interaction rates, suggesting they might be browsing more than engaging.
5. **Budget Browsers** show the least engagement and lowest income levels, which might indicate limited spending power but consistent browsing activity.

These insights can be used to tailor specific strategies for each user segment, ensuring that marketing efforts are efficient and effective.
