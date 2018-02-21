---
layout : post
title : Grocery Basket Analytics Case Study
---

In this case study, we will explore real life sales dataset of a grocery retailer and try to quickly generate insights and answer several questions without asking. The case study is in two parts: first, we will do rapid visual analysis and then we will demonstrate how machine learning models can help us generate not so obvious insights.

 

Without much further ado, let's begin. 

 

Review the Input Dataset:

First step is to load and quickly understand the input data set files. The input dataset is provided as text files of anonymized transaction records of around 200k customers stored in comma separated vector format. The dataset contains of following files:

1. Transaction Orders (3.4 million records) - Order ID, Customer ID, Date, Hour timestamp

2. Order Products (~35 million records): Order ID, Product ID, Add to Cart Order

3. Products (50,000 records): Product ID, Product Name, Aisle ID, Department ID

4. Aisles (134 records): Aisle ID, Aisle Name

5. Departments (14 records): Department ID, Department Name

 

There are no names of the customers or any personal details which reveal the identity. For our quick analysis below, we took a stratified sample dataset of about 1.5 million records. 

 

So let's begin answering:

 

How is the Store Organized?
Let's first quickly make a visual tour of the store. We map the store as per departments and aisles within the departments. The size of each aisle is the number of SKUs or unique products stored. We find that Snacks, Personal Care and Pantry departments together account for almost one-third of total products. This is followed by Beverages, Frozen and Dairy/Eggs departments. 
![blog2](https://user-images.githubusercontent.com/35987843/36478371-7413ae76-172a-11e8-9f45-6cc6ebadc51e.png)
