# Numpay
mport numpy as np
np.__version__
'1.24.3'
dir(np)
SCALAR
​
a=np.array(50)
​
print(a)
print(type(a))
print(a.ndim)
print(a.size)
50
<class 'numpy.ndarray'>
0
1
VECTOR
a =np.array([1,2,3,4,5,6,7])      
print(a)
print(type(a))
print(a.ndim)
print(a.size)
[1 2 3 4 5 6 7]
<class 'numpy.ndarray'>
1
7
Matrix
a =np.array([[1,2,3],
            [4,4,6],
            [7,8,9]])
​
print(a)
print(type(a))
print(a.ndim)
print(a.size)
[[1 2 3]
 [4 4 6]
 [7 8 9]]
<class 'numpy.ndarray'>
2
9
a =np.array([[1,2,3],
            [4,4,6],
            [7,8,9]])
a+5 # if want to sum number in array 
array([[ 6,  7,  8],
       [ 9,  9, 11],
       [12, 13, 14]])
Functions
#arange 
​
a = np.arange(1,6)
a
array([1, 2, 3, 4, 5])
#shape row, column
a = np.arange(1,6) 
a
a.shape
​
(5,)
#a =np.arange(27).reshape(3,3,3) #list of list with reshape (slide, row, column)
a =np.arange(27).reshape(3,3,3) #list of list with reshape
a
array([[[ 0,  1,  2],
        [ 3,  4,  5],
        [ 6,  7,  8]],

       [[ 9, 10, 11],
        [12, 13, 14],
        [15, 16, 17]],

       [[18, 19, 20],
        [21, 22, 23],
        [24, 25, 26]]])
a= np.arange(5*2*4).reshape(5,2,4)
a
array([[[ 0,  1,  2,  3],
        [ 4,  5,  6,  7]],

       [[ 8,  9, 10, 11],
        [12, 13, 14, 15]],

       [[16, 17, 18, 19],
        [20, 21, 22, 23]],

       [[24, 25, 26, 27],
        [28, 29, 30, 31]],

       [[32, 33, 34, 35],
        [36, 37, 38, 39]]])
a= np.zeros((2,3,4)),
             
a
(array([[[0., 0., 0., 0.],
         [0., 0., 0., 0.],
         [0., 0., 0., 0.]],
 
        [[0., 0., 0., 0.],
         [0., 0., 0., 0.],
         [0., 0., 0., 0.]]]),)
a= np.ones((2,3,4))
a
array([[[1., 1., 1., 1.],
        [1., 1., 1., 1.],
        [1., 1., 1., 1.]],

       [[1., 1., 1., 1.],
        [1., 1., 1., 1.],
        [1., 1., 1., 1.]]])
a= np.empty((2,3,4))
a
array([[[1., 1., 1., 1.],
        [1., 1., 1., 1.],
        [1., 1., 1., 1.]],

       [[1., 1., 1., 1.],
        [1., 1., 1., 1.],
        [1., 1., 1., 1.]]])
#Linspace
​
a = np.linspace(1,3,5)
a
array([1. , 1.5, 2. , 2.5, 3. ])
a= np.ones((2,3,4))
a
print(type(a))
print(a.dtype)
<class 'numpy.ndarray'>
float64
a= np.ones((2,3,4),dtype=np.int64)
           
print(a.dtype)
a
           
int64
array([[[1, 1, 1, 1],
        [1, 1, 1, 1],
        [1, 1, 1, 1]],

       [[1, 1, 1, 1],
        [1, 1, 1, 1],
        [1, 1, 1, 1]]], dtype=int64)
a= np.ones((2,3,4),dtype=str)
           
print(a.dtype)
a
<U1
array([[['1', '1', '1', '1'],
        ['1', '1', '1', '1'],
        ['1', '1', '1', '1']],

       [['1', '1', '1', '1'],
        ['1', '1', '1', '1'],
        ['1', '1', '1', '1']]], dtype='<U1')
arr = np.array([2, 1, 5, 3, 7, 4, 6, 8])
np.sort(arr)
array([1, 2, 3, 4, 5, 6, 7, 8])
#               0  1  2  3  4  5  6  7
arr = np.array([2, 1, 5, 3, 7, 4, 6, 8])
np.argsort(arr)
array([1, 0, 3, 5, 2, 6, 4, 7], dtype=int64)
