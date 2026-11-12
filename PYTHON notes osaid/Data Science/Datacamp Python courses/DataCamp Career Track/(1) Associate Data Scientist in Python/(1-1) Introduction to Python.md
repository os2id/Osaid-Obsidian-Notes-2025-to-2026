Study sections (**In every section we have a practice for it**):
1- [Print()]

2- Variable and [type()]

3- Lists (list slicing, list manipulation, Lists behind the scene)

4- Functions ([max()], [round()], [help()], How to find functions if you do know it, and Practice functions)

5- Methods [.function] sub-sections of methods: ([.index()] method, [.count()] method, [.capitalize()] method, [.replace()] method)

6- Packages (How to Install packages from the internet)

7- Numpy (Lists recap, Numpy solution to a list, Numpy: remarks, Numpy: Subsetting )

8- 2D Numpy arrays (To see how many columns and rows in the array [<,array name>.shape], What happens if you changed one index from a number to a string?, Subsetting a 2D Numpy)

9- NumPy: Basic Statistics (Mean & Median, Check for Correlation,  Standard deviation)

10- Generate data



## ==## [type()] Function==
![[Pasted image 20260427132613.png]]Here it shows us the type of the value inside it, so (y) is a string and (z) is a Boolean (T/F) function


Types of Data![[Pasted image 20260428005719.png]]


## ==## [Lists()]==
let us say we have our family members height, we can store them in list rather than listing them individually
![[Pasted image 20260428005823.png]]
![[Pasted image 20260428010143.png]]

We can put strings and integers or floats in the same list:
![[Pasted image 20260428010246.png]]

We can put a list inside a list. Here we are dividing each list to know who's height belongs to whom:
![[Pasted image 20260428010326.png]]

Here we printed(fam2):
![[Pasted image 20260428010746.png]]
we see that fam2 has sub lists inside a list

Here we are seeing the type of fam and fam2:
![[Pasted image 20260428010845.png]]

Here we can see the list has the string with its value:
![[Pasted image 20260428011256.png]]

Here we made sub-lists inside a list, which makes it easier if you want to take a specific information:
![[Pasted image 20260428011708.png]]


he did [print(fam[3])] to print the height of emma, the formula is (Index-1): 
![[Pasted image 20260428012024.png]]
The white color is the values and the print function, while the blue is the result


he did [print(fam[6])] to print the string of dad, the formula is (Index-1): 
![[Pasted image 20260428012133.png]]


![[Pasted image 20260428012325.png]]

### ### Lists slicing

Here the start point is 3 and the end point is 4, so the fifth index is excluded:
![[Pasted image 20260428012547.png]]

Here the start point 1 is and the end point is 3, so the fourth index is excluded:
![[Pasted image 20260428012612.png]]

Start is index zero to index 3, so the fourth index is excluded:
![[Pasted image 20260428012805.png]]

Starting from point 5  to the last point with including the last index as well:
![[Pasted image 20260428012854.png]]


#### Practice slice indexing:
Datacamp exercise 1 explanation:
![[Pasted image 20260428013141.png]]

My solution exercise 1:
![[Pasted image 20260428013421.png]]

Datacamp exercise 2 explanation:
![[Pasted image 20260428013627.png]]

My solution exercise 2:
![[Pasted image 20260428013849.png]]
![[Pasted image 20260428013952.png]]
The two answers are correct


Datacamp exercise 3 explanation:
![[Pasted image 20260428014512.png]]

My solution exercise 3:
![[Pasted image 20260428014447.png]]


### ### Lists manipulation
![[Pasted image 20260428014800.png]]

#### #### Changing lists elements
Here for example we want to update dad height because his height is shrinking due to growing in age:
![[Pasted image 20260428014835.png]]

Updating lisa height:
![[Pasted image 20260428015000.png]]

#### #### Adding elements in lists
![[Pasted image 20260428015120.png]]



#### #### Removing elements in lists
fam list:
![[Pasted image 20260428015430.png]]
We are deleting emma from the list(fam):
![[Pasted image 20260428015329.png]]

### ### Lists behind the scene (how lists work)
Here we can see that y changing list(y) index it also changed the list(x) index:
![[Pasted image 20260428015559.png]]
![[Pasted image 20260428015927.png]]
The update is visible to all y and x

Here we are making y list a copy of x list, so when we change list(y) index the old list(x) will not change because it is another separated list:
![[Pasted image 20260428020042.png]]


#### #### Practice lists manipulation and how it works:
Datacamp exercise 1 explanation:
![[Pasted image 20260428021201.png]]

My solution exercise 3:
![[Pasted image 20260428021320.png]]

Datacamp exercise 2 explanation:
![[Pasted image 20260428021513.png]]

My solution exercise 2:
![[Pasted image 20260428021717.png]]



Datacamp exercise 3 explanation:
![[Pasted image 20260428022649.png]]

My solution exercise 3:
![[Pasted image 20260428022616.png]]
Done! correct answer

Datacamp exercise 4 explanation:
![[Pasted image 20260428022806.png]]
![[Pasted image 20260428022920.png]]
So here we can see that all areas and areas_copy changed because we didn't create a copied list of list(areas)

My solution exercise 4:
Here because we created a copy of the list(areas) in areas_copy we can see that the old list(areas) is kept constant:
![[Pasted image 20260428023126.png]]
Done! correct answer



## ==## Functions==
![[Pasted image 20260428023931.png]]

### ### [max()] function
Here we used [max()] function
![[Pasted image 20260428024028.png]]

### ### [round()] function
Here we used [round()] function. It rounds the number to the closest integer, for example, [round(1.68)] here the closest number to it is 7 but if we rounded 4.5 I think it is near to 4 so it will be 4 
![[Pasted image 20260428024158.png]]

We can also use:
![[Pasted image 20260428024729.png]]


### ### [help()] function
Here we used [help()] function:
![[Pasted image 20260428024654.png]]

we can also use [?] :
![[Pasted image 20260428031451.png]]
### ### How to find functions if you do know it
Simple way is to use the internet:
![[Pasted image 20260428024910.png]]
[You can search here](https://docs.python.org/3/library/functions.html)

### ### Practice Functions

Datacamp exercise 1 explanation:
![[Pasted image 20260428025357.png]]

My solution exercise 1:
![[Pasted image 20260428030001.png]]
Done! correct answer


Datacamp exercise 2 explanation:
![[Pasted image 20260428030049.png]]

My solution exercise 2:
![[Pasted image 20260428031951.png]]
![[Pasted image 20260428032000.png]]
Done! correct answer


Datacamp exercise 3 explanation:
![[Pasted image 20260428032337.png]]

My solution exercise 3:
![[Pasted image 20260428033005.png]]
Done! correct answer


## ==## Methods [.function]==
![[Pasted image 20260428033155.png]]
![[Pasted image 20260428033247.png]]
![[Pasted image 20260428034649.png]]

#### ChatGPT explanation to what is methods:

Question: is it under functions?

Answer:
Great question! Methods are related to functions, but they are a specific type of function that belongs to Python objects.

While functions like `max()` or `len()` are called directly and are not tied to a particular object, methods are functions that are called on an object using dot notation, like `fam.index('mom')`.

So, methods are a kind of function, but they are associated with objects, which makes them different from standalone functions.

### ### [.index()] method
Here we are calling the index(mom) in the list(fam):
![[Pasted image 20260428033342.png]]
it shows us that the index number of mom is 4


#### two other uses for [.index()]
Sister is a string here, sister = "liz":
![[Pasted image 20260428034826.png]]
Here we are seeing that "z" is in index 2 inside the string
![[Pasted image 20260428034808.png]]



list(fam):
![[Pasted image 20260428033907.png]]
Here we can see that it is showing the index of mom string is the fourth inside list(fam):
![[Pasted image 20260428034816.png]]

### ### [.count()] method
list(fam):
![[Pasted image 20260428033907.png]]

Here we are counting how many times (1.73) is in the list(fam):
![[Pasted image 20260428033637.png]]
only one time it is in the list(fam)

### ### [.capitalize()] method
![[Pasted image 20260428034352.png]]

### ### [.replace()] method
![[Pasted image 20260428034516.png]]



### ### [.append()] method
![[Pasted image 20260428035358.png]]
==From instructor: "This is pretty cool, because you can write very concise code to update your data structures on the fly, but it can also be pretty dangerous. Some method calls don't change the object they're called on, while others do, so watch out. Again, the fam list was extended."==




### ### practice methods

Datacamp exercise 1 explanation:
![[Pasted image 20260428053128.png]]

My solution exercise 1:
![[Pasted image 20260428053322.png]]
Done! correct answer




Datacamp exercise 2 explanation:
![[Pasted image 20260428053716.png]]

My solution exercise 2:
![[Pasted image 20260428053633.png]]
![[Pasted image 20260428053741.png]]
Done! correct answer




Datacamp exercise 3 explanation:
![[Pasted image 20260428054020.png]]

My solution exercise 3:
![[Pasted image 20260428054054.png]]
Done! correct answer


## ==## Packages==

Why we use packages:
![[Pasted image 20260428075832.png]]

What is packages:
![[Pasted image 20260428075913.png]]

### ### How to Install packages from the internet
![[Pasted image 20260428080118.png]]

### ### Import Pacakge
![[Pasted image 20260428080315.png]]


==From the instructor "this is not clear to another programmer if he read your code":==
![[Pasted image 20260428080635.png]]

==From the instructor "this is better use":==
![[Pasted image 20260428080703.png]]


### ### Practice packages

Datacamp exercise 1 explanation:
![[Pasted image 20260428080945.png]]

My solution exercise 1:
![[Pasted image 20260428081044.png]]
Done! correct answer



Datacamp exercise 2 explanation:
![[Pasted image 20260428100253.png]]

My solution exercise 2:
![[Pasted image 20260428100416.png]]
Done! correct answer


Datacamp exercise 3 explanation & Answer:
![[Pasted image 20260428100823.png]]
Done! correct answer

## ==## Numpy==

### ### Lists recap
![[Pasted image 20260429134711.png]]


Here lists cannot calculate inside lists unless you call an index, so to solve this problem because with huge data it is hard to deal with is to use Numpy:
![[Pasted image 20260429134756.png]]


### ### Numpy solution to a list
![[Pasted image 20260429150522.png]]


Here we put the two lists in an array and then we can calculate each index inside the array:
![[Pasted image 20260429150654.png]]


Here he is showing the two ways, the first is wrong but the first is right:
![[Pasted image 20260429150816.png]]


### ### Numpy: remarks
Here all inputs inside the array list will be (strings):
![[Pasted image 20260429150944.png]]
so by putting different types list indexes in an array they will all be dealt as  a strings even though they are not strings

#### #### Another explanation to Numpy: remarks
`numpy` is great for doing vector arithmetic. If you compare its functionality with regular Python lists, however, some things are different.

First, `numpy` arrays cannot contain elements with different types. If you mix types, like booleans and integers, `numpy` automatically converts them to a common type. Booleans like `True` and `False` are treated as `1` and `0` when combined with numbers, so the array ends up as integers.

Second, the typical arithmetic operators, such as `+`, `-`, `*` and `/` have a different meaning for regular Python lists and `numpy` arrays.





![[Pasted image 20260429151203.png]]


We can also use (sum) and (sort) functions in Numpy 
![[Pasted image 20260429184121.png]]





### ### Numpy: Subsetting
![[Pasted image 20260429150654.png]]
![[Pasted image 20260429151814.png]]





### ### Practice (Numpy)
Datacamp exercise 1 explanation:
![[Pasted image 20260429152450.png]]

My solution exercise 1:
![[Pasted image 20260429152734.png]]
Done! correct answer



Datacamp exercise 2 explanation:
![[Pasted image 20260429153403.png]]

My solution exercise 2:
![[Pasted image 20260429153427.png]]
Done! correct answer


Datacamp exercise 3 explanation:
![[Pasted image 20260429161103.png]]

My solution exercise 3:
![[Pasted image 20260429161114.png]]
![[Pasted image 20260429161122.png]]
Done! correct answer



Datacamp exercise 4 explanation:
![[Pasted image 20260429170502.png]]

My solution exercise 4:
![[Pasted image 20260429170453.png]]
Done! correct answer




## ==## 2D Numpy arrays==

![[Pasted image 20260429171123.png]]


### ### To see how many columns and rows in the array [<,array name>.shape]
![[Pasted image 20260429171318.png]]


### ### What happens if you changed one index from a number to a string?
So here we can see that all indexes changed to be a strings because we changed one index to be a string in the array
![[Pasted image 20260429171430.png]]
![[Pasted image 20260429171438.png]]

### ### Subsetting a 2D Numpy 
![[Pasted image 20260429171655.png]]
 [<,array name>[<, number of the Row you need>]]





[<, number of the Row you need>, <,number of number of the column you need>] or [. <,array name>[<, number of Rows>][<,number of the column you need>] ]  :![[Pasted image 20260429171745.png]]




Here he wants all rows (the height and weight) of the second and third family member:
![[Pasted image 20260429172333.png]]
[:, <,the number of the column you need] (:) this sign means ALL, and here it means print all rows




Here he wants only the second row and all columns:
![[Pasted image 20260429172620.png]]
![[Pasted image 20260429172629.png]]
[<,The number of the row you need>, :] (:) this sign means ALL, and here it means print all columns

### ### practice (2D Numpy)
Datacamp exercise 1 explanation:
![[Pasted image 20260429173542.png]]

My solution exercise 1:
![[Pasted image 20260429173619.png]]
Done! correct answer






Datacamp exercise 2 explanation:
![[Pasted image 20260429174029.png]]

My solution exercise 2:
![[Pasted image 20260429174010.png]]
Here we can see that (1015, 2) because we printed [.shape] function which gave us 1015 = rows and 2 = columns
Done! correct answer




Datacamp exercise 3 explanation:
![[Pasted image 20260429182635.png]]

My solution exercise 3:
![[Pasted image 20260429175409.png]]
Because Python starts counting from **0**, not from 1 in the indexes, thats why we wrote 49 indicating we want the row (50) and row(124) in the next part.
Done! correct answer






Datacamp exercise 4 explanation:
![[Pasted image 20260429182657.png]]

My solution exercise 4:
![[Pasted image 20260429182619.png]]
Done! correct answer


## ==## NumPy: Basic Statistics==
![[Pasted image 20260429182904.png]]

Here with big data we will see (...) sign which means we cannot know what are the data or numbers inside
![[Pasted image 20260429183006.png]]


### ### Mean & Median
Here (mean) means the average, and (median) means the middle number let us say for example we have 5 numbers from 1 to 5 then the median is 3 because it is the middle number: 
![[Pasted image 20260429183518.png]]
[np.mean(<,name of the array>)]
[np.median(<,name of the array>)]

OR if you need specific row or column:
[np.mean(<,name of the array>[:, <,put the column you need>)]] Here it will give us all rows but we should specify what column we need for example [np.mean(np_city[:, 1)]] means here we want all rows of the array(np_city) but we need only the second column. This applies with all (mean, median, and standard deviation)

[np.mean(np_city[0, :)]] Here it means we want the (mean) of the first row and we want as well to print all columns using (:) sign 

Example of mean and median use:
![[Pasted image 20260429194910.png]]

### ### Check for Correlation 
![[Pasted image 20260429183837.png]]


### ### Standard deviation
![[Pasted image 20260429183935.png]]
[np.std(<,name of the array>)]

OR if you need specific row or column:
[np.mean(<,name of the array>[:, <,put the column you need>)]] Here it will give us all rows but we should specify what column we need for example [np.mean(np_city[:, 1)]] means here we want all rows of the array(np_city) but we need only the second column. This applies with all (mean, median, standard deviation)

[np.std(np_city[:, 1)]] It will be like that for the standard deviation


[np.std(np_city[0, :)]] Here it means we want the (standard deviation) of the first row and we want as well to print all columns using (:) sign 

### ### Practice (NumPy: Basic Statistics)

Datacamp exercise 1 explanation:
![[Pasted image 20260429194459.png]]

My solution exercise 1:
![[Pasted image 20260429194948.png]]
Done! correct answer






Datacamp exercise 2 explanation:
![[Pasted image 20260429200034.png]]

My solution exercise 2:
![[Pasted image 20260429200608.png]]
Done! correct answer






## ==## Generate data==
![[Pasted image 20260429184252.png]]

