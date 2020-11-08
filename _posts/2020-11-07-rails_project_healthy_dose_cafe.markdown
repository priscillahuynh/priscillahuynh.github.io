---
layout: post
title:      "Rails Project: Healthy Dose Cafe"
date:       2020-11-08 03:21:38 +0000
permalink:  rails_project_healthy_dose_cafe
---

For my third Rails project, I decided to incorporate my passion for health concious food. I'll admit I'm a sucker for that  overpriced Matcha latte and the unconventional gluten free/dairy free pastry. So it was only natural for me to create an online shop where users could purchase their own favorites from the comfort of home.

The project has 6 models outlined below:

```
class User < ApplicationRecord
    has_many :orders
    has_one :cart
		
	class Product < ApplicationRecord
  belongs_to :category
  has_many :line_items
  has_many :carts, through: :line_items
  has_one_attached :image
	
	class Order < ApplicationRecord
  belongs_to :user
  has_one :cart
  has_many :line_items, through: :cart
	
	class LineItem < ApplicationRecord
  belongs_to :product
  belongs_to :cart, optional:true
	
	class Category < ApplicationRecord
  has_many :products, :dependent => :destroy
		
	class Cart < ApplicationRecord
  belongs_to :user
  belongs_to :order, optional: true
  has_many :line_items, dependent: :destroy
  has_many :products, through: :line_items
```

From the main page a user can login, signup, or signup with facebook. Once logged in the user will be redirected to the home page listing the available menu categories. 

Each category name is a link to view all the products within that category. From there the user is able to add that item to the cart. When the user is finished shopping they can view their cart, and increase or decrease each item if they wish. They also have the option to add any special requests to their order. After completing their purchase they are redirected to the main page. If they view their profile, they can view a list of links to their previous orders. 

An admin has access to all of the same views but with additional links to add, edit, or delete categories and products on the menu. The admin profile will also show the top 3 most popular products and 3 highest paying customers.



