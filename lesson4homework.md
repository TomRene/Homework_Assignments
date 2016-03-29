## Lesson 4 Homework - Chipotle (Tom Pichard)

1. Describe the dataset
  1. Order is the order ID
  2. Quantity is the nbr of items in the order
  3. Item_Name is the name of the product for sale
  4. Choice_Description is the description of elements selected for the order
  5. Item_Price is the final price charged to the customer accounting for elements chosen and nbr of items
  
2. How many orders are there in the file?
  1. There are 4623 rows in the file so figuring 4622 orders (to account for the header row
  2. I used the wc -l chipotle.tsv command line prompt

3. How many lines are there in the file?  4623.

4. Which burrito is more popular - Steak or Chicken?
  1. Chicken is more popular at a 553 count versus 368 for Steak burritos
  2. I used the grep -c "Steak Burrito" chipotle.tsv command

5.  
  

