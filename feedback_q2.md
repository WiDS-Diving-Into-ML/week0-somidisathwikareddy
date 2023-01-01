# Feedback for Problem 2

## Loading the data

* The standard csv way to read a file is to use the reader class in the csv module, but if you observe the data, it's almost like a text file, just that it's structured column-wise as well.
* So a nice way to read this (especially since it has no header, which csv files usually have) is to treat it like a text file and read it line by line into a list, and then split the string with the ',' character, and you get what you want.

## Grouping the Data

* For this part, your idea is correct, but you should have used one for loop with 10 iterations, instead of copying the same thing and storing it in 10 different arrays, changing the number and array name in each. You could have used a dictionary or a normal Python list, to store all the images (note that you can't use a numpy array to store it because the number of images in each category would be different, and NumPy only allows homogenous data types)
* Check these two links out as well, they talk about group by using pure NumPy : https://stackoverflow.com/questions/49372918/group-numpy-into-multiple-sub-arrays-using-an-array-of-values and https://stackoverflow.com/questions/49141969/vectorized-groupby-with-numpy?noredirect=1&lq=1

## Computing Mean Images

* Similar problem here of being neater using loops, these are all just good coding practices that will save you time and make it look neater, so if you had used a for loop for the earlier part, you would have used it here as well.
