# Mercari Price Suggestion Challenge
## Business Problem

Mercari is a safe and easy online marketplace for buying and selling clothing, electronics, household goods, specialty items, and more. Mercari would like to offer pricing suggestions to sellers, but this is tough because their sellers are enabled to put just about anything, or any bundle of things, on Mercari's marketplace.

This is very important because optimal prices attract more customers to their website and result in faster transactions. Hence, Mercari wanted an algorithm that automatically suggests the right product prices. 


## Data Overview

<b>Source</b>: https://www.kaggle.com/c/mercari-price-suggestion-challenge

The files consist of a list of product listings. These files are tab-delimited. The training set have ~1.5 million entries (1,482,535) and the test set have ~3.5 million entries (3,460,725). The attributes (i.e. columns) contained in both datasets are the following:

<b>train_id or test_id</b> - the id of the listing

<b>name</b> - the title of the listing. Note that we have cleaned the data to remove text that look like prices (e.g. $20) to avoid leakage. These removed prices are represented as [rm]

<b>item_condition_id</b> - the condition of the items provided by the seller

<b>category_name</b> - category of the listing

<b>brand_name</b> - name of the “brand” the product is sold under

<b>price</b> - the price that the item was sold for. This is the target variable that you will predict. The unit is USD. This column doesn't exist in test.tsv since that is what you will predict.

<b>shipping</b> - 1 if shipping fee is paid by seller and 0 by buyer

<b>item_description</b> - the full description of the item.
