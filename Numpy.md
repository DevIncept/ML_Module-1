<p align="center">
   <img src="https://th.bing.com/th/id/OIP.lOUjzO-NYYFws-ftVf9glAHaDt?w=328&h=175&c=7&o=5&pid=1.7" alt="Numpy">
   <br />
   
</p>

# :bulb: Numpy :computer:

<b><font color=green>```Table of Contents``` </font></b>


1. ***Introduction to Numpy***
2. ***Prerequisites***
3. ***Basic features of Numpy***
4. ***Python Lists and Arrays***
5. ***Why NumPy over Python Lists?***
6. ***Installating and Importing*** 
7. ***Creating Numpy array*** 
8. ***NdArray(N-Dimensional Array)***
9. ***Array Indexing and Slicing***
10. ***Numpy Array Shape and reshape***
11. ***Broadcasting***
12. ***Performing arithmetic operations on NumPy Arrays***
13. ***How To Insert And Delete Array Elements***
14. ***Some mathematical functions***
15. ***Numpy Sorting, searching, and Counting***
16. ***Joining Numpy Arrays***
17. ***Comparision and Copying*** 
18. ***Visual Representation***
19. ***Conclusion***

# <b>1.Introduction to Numpy :memo:</b>
  NumPy also known as ***Numerical Python*** is an open source library that is used for mainly working with numerical data. It provides a high-performance multidimensional array  object, and tools for working with these arrays. It also has functions for working in the domain of linear algebra, fourier transform, and matrices.
# <b>2.Prerequisites :arrow_backward:</b>
* Basic knowledge about python
* Jupyter notebook or any editor for practising.
# <b>3.Basic features of Numpy :diamond_shape_with_a_dot_inside:</b>
  * NumPy aims to provide an array object that is up to 50x faster than traditional Python lists.
  * The array object in NumPy is called ndarray which provides a lot of supporting functions that make working with ndarray very easy.
  * NumPy arrays are stored at one continuous place in memory unlike lists, so processes can access and manipulate them very efficiently.
  
# <b>4.Python Lists and Arrays :ballot_box_with_check:</b>
NumPy is something which deals with arrays, so let’s have a look at what Arrays are.
## Array
* An array is a special variable, which can hold more than one value at a time.
* All the stored items should be of the same type.
<p align="center">
   <img src="https://vrzkj25a871bpq7t1ugcgmn9-wpengine.netdna-ssl.com/wp-content/uploads/2018/09/numpy-array-with-index-and-value.png" alt="Numpy" ,height = 300, width=500>
   <br />
   
</p>
   
* Arrays are basically divided into two types:
  * One-Dimensional Array 
  * Multi-Dimensional Array
* ### One-Dimensional Array 
  One Dimensional array is a simple data structure that stores a collection of similar type data in a contiguous block of memory. 
    Example:- 
    ```An Integer array in C/C++/Javaint ar[] = {1,4,67,3,64}```
    
    To access the elements of a one-dimensional Array you can use the indexeslike : <br>
    
    ```
    ar[0] #gives us 1
    ar[2] #gives us 67
    ```
       
    <br>
   An array of characters is called a string.
* ### Multi-Dimensional Array
    The Multi dimensional array is a type of array that stores multiple data elements of the same type in matrix or table like format with a number of rows and columns.
   <p align="center">
   <img src="https://iq.opengenus.org/content/images/2020/04/index.png" alt="1-D Array">
   <br />
   
</p> 
    
## List
Now lets learn about a bit of python Lists.
* A List is used to store the sequence of various types of data. 
* These are a kind of arrays. Data are inclosed inside [ ] brackets seprated by commas(,). 
* Lists are mutable in nature it means data which can be changed when required. 
* Duplicate entries are allowed in list. 
* A list can also have another list as an item. Such list is called a nested list.
* Basically a bit more easier and handy.
* A Python list may contain different types! Indeed, you can store a number, a string, and even another list within a single list.
<br>

```
my_list = [] #create empty list
print(my_list)
my_list = [1, 2, 3, 'example', 3.132] #creating list with data
print(my_list)
```

<br>

```
Output:
[]
[1, 2, 3, ‘example’, 3.132]
```

<br>

# 5.Why NumPy over Python Lists :question:
* NumPy can provide an array object that is up to 50x faster than traditional Python lists.
* Arrays are very frequently used in data science, where speed and resources are very important.
* In Python we have lists that serve the purpose of arrays, but they are slow to process.
* It provides various mathematical functions which can be carried on easily.<br>
<p align="center">
<img src = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRYn72i3qeOmxjt5Th24PEiBr08_jSyHhOTJA&usqp=CAU", height = 400, width = 550>
</p><br>

# 6.Installating and Importing Numpy :computer:
## Installation
If you have Python and pip already installed on a system, then installation of NumPy is very easy.<br>
Install it using this command:<br>
```pip install numpy``` <br>
Or if you are using anaconda prompt then you can use this command-<br>
```conda install numpy```<br>
## Importing
If you want to use numpy in your program, first you have to import it. You can import the Numpy library by-<br>
```Import numpy as np```<br>
# 7.Creating Numpy array :bookmark_tabs:
To create a basic NumPy Array you can use the function np.array() The array object in NumPy is called ndarray.<br>
```
import numpy as np
arr1=np.array([1,2,3])
arr2=np.array(['a','b','c','d','e'])
```
<br>


```
Output:
[1 2 3]
['a' 'b' 'c' 'd' 'e']
```

<br>

## Creating numpy arrays from python lists
Say we have a Python list: <br>

```
my_list = [1, 2, 3, 4, 5]
```
<br>

We can simply create a NumPy array called my_numpy_list and display the result: <br>

```
my_numpy_list = np.array(my_list)
my_numpy_list  #This line show the result of the array generated
```

<br>


## Create some Arrays using builtin functions
* To create an Array of Zeroes use ```np.zeros()```.
* To create an Array of Ones use ```np.ones()```.
* To create an Array with a range of elements use ```np.arange()```. <br>


```
arr1 = np.zeros(3)
arr2 = np.ones(5)
arr3 = np.arange(5)
arr4 = np.arange(1,4)    # To specify start and stop
arr4 = np.arange(1,4,2)  # To specify start, stop and step size
```

<br>

```
Output:
[0. 0. 0.]
[1. 1. 1. 1. 1.]
[0 1 2 3 4]
[1 2 3]
[1 3]
```

<br>


## Generating an array of random numbers in NumPy
* We can generate an array of random numbers using ```rand()```, ```randn()``` or ```randint()``` functions.
* Using ```random.rand()```, we can generate an array of random numbers of the shape we pass to it from uniform distribution over 0 to 1.
* For example, say we want a one-dimensional array of 4 objects that are uniformly distributed from 0 to 1, we can do this: <br>

```
random_arr = np.random.rand(4)
```
<br>

It will return array of some random values between 0 and 1. Like : <br>

```
Output:
[0.72424238 0.36030484 0.3686609  0.20998672]
```
<br>


# 8.Nd Array(N-Dimensional Array) :arrow_up:
* An array class in Numpy is called an ndarray.
* Number of dimensions of the array is called the rank of the array<br>
<p align="center"><img src = "https://cdn.educba.com/academy/wp-content/uploads/2019/12/numpy-ndarray.png", height = 400 width = 700></p><br>

* Lets understand by creating Nd array:

<br>

 ```
 import numpy as np
 arr1=np.array([[1,2,3],[4,5,6]])
 arr2=np.array([[1,2,3],[4,5,6],[7,8,9]])
 arr3=np.array([['a','b','c'],['d','e','f']])

 #creates a 3X3 array with all zeros
 zeros=np.zeros((3,3))

 #creates a 2X2 array with all ones
 ones=np.ones((2,2),dtype='int64')  #specify the type with (dtype) parameter 

 print(arr1)
 print(arr2)
 print(arr3)
 print(zeros)
 print(ones)
 ```
 
 <br>
 
 ```
 Output:
 [[1 2 3]
  [4 5 6]]

 [[1 2 3]
  [4 5 6]
  [7 8 9]] 

 [['a' 'b' 'c']
  ['d' 'e' 'f']]

 # 3X3 Matrix
 [[ 0.  0.  0.]
  [ 0.  0.  0.]
  [ 0.  0.  0.]]

 # 2X2 Matrix
 [[1 1]
  [1 1]]
 ```
 
 <br>
 
# 9.Array Indexing and Slicing :pushpin:
## Indexing
Indexing NumPy arrays is similar to that of Python lists. You can simply pass in the index you want.
Still, a detail explanation:
* You use square brackets [] as the index operator
* Generally, you pass integers to these square brackets, from 0 to n-1(where n is the length of array) to get the desired element. 
```
#indexing
import numpy as np
arr1= np.array([9,10,11,12])
print(arr1[0]) #prints element on 0th index
print(arr1[1]) #prints element on 1st index
print(arr1[-1]) #prints element on last index 
print(arr1[-4]) #print element on last 4th index
```
<br>

```
Output:
9
10
12
9
```
<br>
Similarly, we can select elements in a 2-d array using either the double bracket [][] notation or the single bracket [,] notation.
<br>
<br>

```
#indexing in 2-d array
two_d_array = np.array([[10,20,30], [40,50,60], [70,80,90]])
print(two_d_array[1][2])   #prints the element in row index 1, and column index 2
print(two_d_array[0,1])    #prints the elemnt in row index 0, and column index 1
```
<br>

```
Output:
60
20
```
## Slicing-
Slicing means to get the elements from one given index to another given index.
You can put a colon : or a combination of the colon with integers in it to  designate the elements/rows/columns you want to select.
```arr[start:end]``` - returns the subarray from starting index till end index(but the end is not included).
```arr[start:end:step]``` - we can also provide step size
```arr[start:]``` - returns the rest of subarray from this starting index  
```arr[:end]```  - returns the subarray from beginning till this “end” index (but the end is not included)
<br>

```
#slicing
arr2 = np.array([10,20,30,40,50,60,70,80])
print(arr2[2:5])    #returns everything from index 2 to 5(exclusive) 
print(arr2[1:6:2])  #returns subarray with step size 2, from index 1 to 6(exclusive)
print(arr2[3:])     #returns everything from index 3 to the end of the array.
print(arr2[:5])     #returns everything from index 0 to 5(exclusive)
print(arr2[-2:])    #returns everything from last 2nd second element to the end of array
```
<br>

```
Output:
[30 40 50]
[20 40 60]
[40 50 60 70 80]
[10 20 30 40 50]
```
<br>

# 10.Numpy Array Shape and reshape :triangular_ruler:
## Shaping
It is possible to know the no. of  dimensions in the array and no.of elements present in these dimensions respectively.
Lets see these numpy functions-

* ```arr.shape``` - returns tuple of integers that indicate the number of elements stored along each dimension of the array.
* ```arr.ndim``` - returns no. of dimensions present in array.
* ```arr.size``` - returns total no of elements of the array.
<br>

```
#Shaping
arr = np.array([[[0, 1, 2, 3],
                 [4, 5, 6, 7]],

                [[0, 1, 2, 3],
                 [4, 5, 6, 7]],

                 [[0 ,1 ,2, 3],
                  [4, 5, 6, 7]]])

print('Shape of the array:',arr.shape)              
print('No of dimensions of the array:',arr.ndim)     
print('Total no of elements of the array:',arr.size) 
```


<br>


```
Output:
Shape of the array: (3, 2, 4)
No of dimensions of the array: 3
Total no of elements of the array: 24
```

<br>

## Reshaping
We can reshape an array in numpy by using ``` .reshape()``` function.
<br>

```
#Reshaping
arr1 = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
reshaped_arr1 = arr1.reshape(4, 3) #from 1-d to 2-d
print(reshaped_arr1)

```


<br>


```
Output:
[[ 1  2  3]
 [ 4  5  6]
 [ 7  8  9]
 [10 11 12]]
```


<br>


```
#Reshaping
arr2 = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
reshaped_arr2 = arr2.reshape(2,3,2) #from 1-d to 3-d
print(reshaped_arr2)
```


<br>

```
Output:
[[[ 1  2]
  [ 3  4]
  [ 5  6]]

 [[ 7  8]
  [ 9 10]
  [11 12]]]
```
<br>

We can use reshape(-1) to convert mult-dimensional array into 1-D array.<br>


```
#reshaping - from multi-dimension to 1-D
arr = np.array([[9,8,7], [4, 5, 6]])
reshaped_arr = arr.reshape(-1)
print(reshaped_arr)
```

<br>

```
Output:
[9 8 7 4 5 6]
```

<br>

<b>Note</b> - We can only reshape the array if the elements required for reshaping are equal in both shapes.
<b>For example</b> - We can reshape an 8 elements 1D array into 4 elements in 2 rows 2D array but we cannot reshape it into a 3 elements 3 rows 2D array as that would require 3x3 = 9 elements.
# 11.Broadcasting :white_square_button:
Broadcasting is a quick way to change the values of a NumPy array.<br>

```
#Broadcasting
arr = np.array([1, 2, 3, 4, 5, 6])
arr[0:3] = 50    #changes of value elements from index 0 to 3(exclusive) 
print(arr)
```


<br>

```
[50 50 50  4  5  6]
```
<br>

# 12.Performing arithmetic operations on NumPy Arrays :heavy_division_sign:
<p align = "center"><img src = "https://th.bing.com/th/id/OIP.PYUzdjvi8d_XoOm6C0WnmQHaGK?w=182&h=151&c=7&o=5&pid=1.7", height = 300, width = 400></p>
You can also do basic arithmetic operations with arrays. <br>


```
#arithmetic operations
arr1=np.array([4,4,4,4])
arr2=np.array([2,2,2,2])
print(arr1+arr2)       #adding each element of arr1 with its respective(same indexed) element of arr2
print(arr1-arr2)       #substracting 
print(arr1/arr2)       #division
print(arr1*arr2)       #multiplication

print(arr1+1)          #Adding one to all elements
print(arr2-1)          #Subtracting one from all elements
print(arr1*3)          #multiplying 3 to all elements
```


<br>


```
Output:
[6 6 6 6]
[2 2 2 2]
[2. 2. 2. 2.]
[8 8 8 8]
[5 5 5 5]
[1 1 1 1]
```
<br>


# 13.How To Insert And Delete Array Elements :scissors:
* We can insert and delete an element at particular index in NumPy array with the use of ```numpy.insert()``` and ```numpy.delete()``` function.
* We can also use ```numpy.append()``` function to append any element at the end of array.
* Parameters for these functions:
  * ```numpy.insert(array, index, value,axis=None)``` , where axis is optional
  * ```numpy.delete(array,index,axis=None)```,  where axis is optional
  * ```numpy.append(array, value, axis = None)```where axis is optional
```
#Insert element in array
arr = np.array([1, 2, 3, 4])
print(np.insert(arr, 1, 5))

#delete element in array
print(np.delete(arr,1))

#append element in array
print(np.append(arr,9))
```


<br>


```
Output:
[1 5 2 3 4]
[1 3 4]
[1 2 3 4 9]
```


<br>

# 14.Some mathematical function :heavy_plus_sign:
You can use these functions on large data sets and find the answers in just seconds. 

```numpy.sum()``` - use it to get sum of all elements in array
```numpy.max()``` - use it to find maximum element in array
```numpy.min()```  - use it to find minimum element in array
<br>


```
arr = np.array([1, 2, 3, 4, 5, 6])
print(np.sum(arr))  #sum

print(np.max(arr))  #max value

print(np.min(arr))  #min value
```



<br>


```
Output:
21
6
1
```

<br>


```numpy.mean()```  - use it to find mean of all elements in array
Mean is the average value.
To calculate the mean, we find the sum of all values, and divide the sum by the number of values.

```numpy.median()```  - use it to find median of all elements in array
Median is the mid point valueThe median value is the value in the middle, after you have sorted all the values.

<br>

```
arr=np.array([19,13,18,21,44,17,12,31,37,8,12,27])

x=np.mean(arr)
print("mean of the given array : ",x)

y = np.median(arr)
print("median of the given array : ", y)
```


<br>


```
Output:
mean of the given array :  21.583333333333332
median of the given array :  18.5
```

<br>


If you are wondering about the mode function, then numpy doesn’t have mode function.
# 15.Numpy Sorting, searching, and Counting :mag_right:
## Sorting:
Sorting is the arranging data in a particular format. Sorting algorithm specifies the way to arrange data in a particular order. A variety of sorting related functions are available in NumPy. These sorting functions implement different sorting algorithms.
```numpy.sort()```:This function returns a sorted copy of an input array.

<br>


```
# sort along the first axis
narr1 = np.array([[12, 15], [10, 1]])
arr1 = np.sort(narr1, axis = 0)        
print ("Along first axis : \n", arr1) 

# sort along the last axis
narr2 = np.array([[10, 15], [12, 1]])
arr2 = np.sort(narr2, axis = -1)        
print ("\nAlong first axis : \n", arr2)

narr3 = np.array([[12, 15], [10, 1]])
arr1 = np.sort(narr3, axis = None)        
print ("\nAlong none axis : \n", arr1)
```


<br>


```
Output:
Along first axis : 
[[10  1] 
 [12 15]]
Along first axis : 
[[10 15] 
 [ 1 12]]
Along none axis :  
[ 1 10 12 15]
```

<br>



## Searching:
Searching is an operation or a technique that helps finds the place of a given element or value in the list. Any search is said to be successful or unsuccessful depending upon whether the element that is being searched is found or not.
<br>


```where()``` : Returns the indices of searched value.
<br>


```
arr1 = np.array([1, 2, 3, 4, 5, 4, 4])
x = np.where(arr1 == 4)
y = np.where(arr1%2 == 0)
z = np.where(arr1%2 == 1)
print(x)
print(y)
print(z)
```


<br>


```
Output:
(array([3, 5, 6], dtype=int64),)
(array([1, 3, 5, 6], dtype=int64),)
(array([0, 2, 4], dtype=int64),)
```

<br>


```searchsorted()```: Performs a binary search in the array, and returns the index where the specified value would be inserted to maintain the search order.
<br>


```
# input array
in_arr = [2, 3, 4, 5, 6]
print ("Input array : ", in_arr)
# the number which we want to insert
num = 4
print("The number which we want to insert : ", num) 
out_ind = search.searchsorted(in_arr, num) 
print ("Output indices to maintain sorted array : ", out_ind)
```


<br>


```
Output:
Input array :  [2, 3, 4, 5, 6]
The number which we want to insert :  4
Output indices to maintain sorted array :  2
```

<br>

## Counting 
```numpy.count_nonzero()```: Counts the number of non-zero values in the array.<br>



```
# Counting a number of non-zero values
a = np.count_nonzero([[0,1,7,0,0],[3,0,0,2,19]])
b = np.count_nonzero([[0,1,7,0,0],[3,0,0,2,19]],axis=0)
print("Number of nonzero values is :",a)
print("Number of nonzero values is :",b)
```


<br>


```
Output :
Number of nonzero values is : 5
Number of nonzero values is : [1 1 1 1 1]
```

<br>


# 16.Joining Numpy Arrays :loop:
<p align = "center"><img src = "https://th.bing.com/th/id/OIP.v-zGrQgQslRlrLhl_RPpnAAAAA?w=284&h=78&c=7&o=5&pid=1.7"></p>
* Joining means putting contents of two or more arrays in a single array.
* In SQL we join tables based on a key, whereas in NumPy we join arrays by axes.
* We pass a sequence of arrays that we want to join to the ```concatenate()``` function, along with the axis. If axis is not explicitly passed, it is taken as 0.
<br>


```
#Join two arrays
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])
arr = np.concatenate((arr1, arr2))
print(arr)
```


<br>


```
Output:
[1 2 3 4 5 6]
```



<br>


```
#Join two 2-D arrays along rows (axis=1)
arr1 = np.array([[1, 2], [3, 4]])
arr2 = np.array([[5, 6], [7, 8]])
arr = np.concatenate((arr1, arr2), axis=1)
print(arr)
```


<br>



```
Output:
[[1 2 5 6] 
 [3 4 7 8]]
```

<br>



## Joining  Arrays using stack function:
* Stacking is same as concatenation, the only difference is that stacking is done along a new axis.
* We can concatenate two 1-D arrays along the second axis which would result in putting them one over the other, ie. stacking.
* We pass a sequence of arrays that we want to join to the ``stack()`` method along with the axis. If axis is not explicitly passed it is taken as 0.

<br>


```
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])
arr = np.stack((arr1, arr2), axis=1)
print(arr)
```


<br>


```
Output:
[[1 4] 
 [2 5] 
 [3 6]]
```

<br>


# 17.Comparison and Copying :books:
## Comparing two numpy arrays
Comparing two NumPy arrays determines whether they are equivalent by checking if every element at each corresponding index are the same.
## Method 1:
We generally use the ```==``` operator to compare two NumPy arrays to generate a new array object. 
Call ```ndarray.all()``` with the new array object as ndarray to return True if the two NumPy arrays are equivalent.
<br>


```
an_array = np.array([[1, 2], [3, 4]])
another_array = np.array([[1, 2], [3, 4]])
comparison = an_array == another_array
equal_arrays = comparison.all()
print(equal_arrays)
```


<br>


```
Output:
True
```


<br>

## Method 2:
We can also use greater than, less than and equal to operators to compare. <br>


```
Syntax : numpy.greater(x1, x2[, out])
Syntax : numpy.greater_equal(x1, x2[, out])
Syntax : numpy.less(x1, x2[, out])
Syntax : numpy.less_equal(x1, x2[, out])
```

<br>


## Copying 
```numpy.copy()```returns a copy of the array.<br>


```
arr = np.array([1, 2, 3, 4, 5])
x = arr.copy()
arr[0] = 42
print(arr)print(x)
```


<br>


```
Output:
[42  2  3  4  5]
[1 2 3 4 5]
```

<br>


# 18.Visual Representation :chart:
NumPy has a ```numpy.histogram()``` function that is a graphical representation of the frequency distribution of data. Rectangles of equal horizontal size corresponding to class interval called <b>bin</b> and <b>variable height</b> corresponding to frequency.
```numpy.histogram()``` : function takes the input array and bins as two parameters.The successive elements in bin array act as the boundary of each bin. <br>


```
a = np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27]) 
np.histogram(a,bins = [0,20,40,60,80,100]) 
hist,bins = np.histogram(a,bins = [0,20,40,60,80,100]) 
print(hist) 
print(bins)
```


<br>


```
Output:
[3 4 5 2 1]
[  0  20  40  60  80 100]
```

<br>


```plt()``` :Matplotlib can convert this numeric representation of histogram into a graph. 
The ```plt()``` function of pyplot submodule takes the array containing the data and binarray as parameters and converts into a histogram. <br>


```
from matplotlib import pyplot as plt 
a = np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27])
plt.hist(a, bins = [0,20,40,60,80,100]) 
plt.title("histogram") 
plt.show()
```


<br>



<img  src = "https://www.pythonpool.com/wp-content/uploads/2020/11/histogram_plot.jpg">








# 19.Conclusion :lock:
* NumPy is one of the most fundamental libraries in Machine Learning and Data Science. 
* It’s coded in Python and it uses vectorized forms to perform calculations at an incredible speed. 
* It supports various built-in functions that come in handy for many programmers.<br>

So, as we are done with the Numpy basics, you can now practise in your jupyter notebook. 
<br>


```EXPLORE, LEARN, PRACTISE!``` <br><br>
<b>By: Samiksha Bhavsar, Kusupati Deekshitha, Subham Nanda <b>
