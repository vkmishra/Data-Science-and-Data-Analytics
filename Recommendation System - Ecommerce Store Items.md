# Data-Science-and-Data-Analytics

#Recommendation System - Ecommerce Store Items

IN this project we have import a dataset (vendor product distribute data set)
nvoiceNo	StockCode	Description	Quantity	InvoiceDate	UnitPrice	CustomerID	Country

1st check description of data set:
Note the negative values in Unit price and quantity, it could have likely been an error or perhaps a return. It's not overly critical for our application that we clean it up, for low let's assume we can remove anything negative.
# Lets see how these records with missing customer ID look

# Number of records and shape before dropping our missing values
# Let's drop these records since we can't build our required matrixes 
Building a customer-item matrix
Something like this:

# We need a create a matrix that contains the customer IDs as the index, and each invidividual item as a column
# We use the pivot function to use the CustomerID as the index and use the StockCode as columns
# Then we using the Quantity value as the values we display, and finally use the aggfunc to sum up these values
# Creating out Colaborative Filter
# Let's use the sklearn cosine_similarity function to compute the pairwise cosine similarities between the cusomters 
# Let's find the customers most similar to our test customer, '12358'
# Finding Items to Recommend to a Customer
