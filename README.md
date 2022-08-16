
# H&M_Personalized_Fashion_Recommendations_Project
Provide product recommendations based on previous purchases

Dataset: https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/overview/description

Team: Ecenur Özütrk , Barış Cengiz , Mert Yüksek

PDF File: 

Streamlit App: 


*******Business Problem *********

H&M Group is a family of brands and businesses with 53 online markets and approximately 4,850 stores. 
Our online store offers shoppers an extensive selection of products to browse through. 
But with too many choices, customers might not quickly find what interests them or what they are looking for, and ultimately, 
they might not make a purchase. To enhance the shopping experience, product recommendations are key. 
More importantly, helping customers make the right choices also has a positive implications for sustainability, as it reduces returns, 
and thereby minimizes emissions from transportation.

In this competition, H&M Group invites you to develop product recommendations based on data from previous transactions, 
as well as from customer and product meta data. The available meta data spans from simple data, such as garment type and customer age, 
to text data from product descriptions, to image data from garment images.

There are no preconceptions on what information that may be useful – that is for you to find out. If you want to investigate 
a categorical data type algorithm, or dive into NLP and image processing deep learning, that is up to you.

Submission File
For each customer_id observed in the training data, you may predict up to 12 labels for the article_id, which is the predicted items 
a customer will buy in the next 7-day period after the training time period. 

*******Datasets************

The dataset contains 4 csv files and one folder with several subfolders, each with a different number of images.

📸 images - images of every article_id
🙋 articles - detailed metadata of every article_id
👔 customers - detailed metadata of every customer_id
🧾 transactions_train - purchases with details

🙋 articles : 

article_id : A unique identifier of every article.
product_code, prod_name : A unique identifier of every product and its name (not the same).
product_type, product_type_name : The group of product_code and its name
graphical_appearance_no, graphical_appearance_name : The group of graphics and its name
colour_group_code, colour_group_name : The group of color and its name
perceived_colour_value_id, perceived_colour_value_name, perceived_colour_master_id, perceived_colour_master_name : The added color info
department_no, department_name: : A unique identifier of every dep and its name
index_code, index_name: : A unique identifier of every index and its name
index_group_no, index_group_name: : A group of indeces and its name
section_no, section_name: : A unique identifier of every section and its name
garment_group_no, garment_group_name: : A unique identifier of every garment and its name
detail_desc: : Details

👔 customers :

customer_id : A unique identifier of every customer
FN : 1 or missed
Active : 1 or missed
club_member_status : Status in club
fashion_news_frequency : How often H&M may send news to customer
age : The current age
postal_code : Postal code of customer

🧾 transactions_train : 

t_dat : A unique identifier of every customer
customer_id : A unique identifier of every customer (in customers table)
article_id : A unique identifier of every article (in articles table)
price : Price of purchase
sales_channel_id : 1 or 2
