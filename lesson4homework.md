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

5.  Do chicken burritos more often have black beans or pinto beans?
  1. Using grep "Chicken Burrito" chipotle.tsv | grep -c "Pinto Beans" returns 105
  2. Using grep "Chicken Burrito" chipotle.tsv | grep -c "Black Beans" returnss 282
  3. ...so I'd have to say Black Beans is the answer.

6. Make a list of all of the CSV or TSV files in the GA-SEA-DAT2 repo
  1. I've returned these and seen them but prefer to count them using the following command while in the GA-SEA-DAT2 directory locally...
  2. find . -name *.ipynb | grep -c ".ipynb" returns 36
  3. find . -name *.txt | grep -c ".txt" returns 2
  4. find . -name *.py | grep -c ".py" returns 28
  5. find . -name *.csv | grep -c ".csv" returns 22
  6. find . -name *.tsv | grep -c ".tsv" returns 2
  7. find . -name *.md | grep -c ".md" returns 4

7. Count the approximate number of occurrences of the word "dictionary" (regardless of case) across all files in the GA-SEA-DAT repo.
  1. Using grep -r "dictionary" . | grep -c "dictionary" returns 81.
  2. Using grep -r "dictionary" . | grep -c "dictionary\|Dictionary" which apparently incorporates an OR condition also returns 81.

  



  
  
  

