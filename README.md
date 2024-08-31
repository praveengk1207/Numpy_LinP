# NumPy: Creating Arrays

1. **What is NumPy?**
   > NumPy is a popular Python library used for working with arrays and performing numerical computations.

2. **What is an ndarray?**
   > The array object in NumPy is called an `ndarray` (N-dimensional array).
   >
   > It is used to store collections of numbers in a grid-like format (1D, 2D, 3D, etc.).

3. **Creating an ndarray:**
   > You can create a NumPy `ndarray` object by using the `array()` function.
   >
   > ```python
   > import numpy as np
   >
   > arr = np.array([50, 60, 70, 80, 100])
   >
   > print(f"ndarray: {arr}")
   > ```
   >
   > **Output:**
   > ```
   > ndarray: [ 50  60  70  80 100]
   > ```

4. **Understanding the `type()` Function in Python**
   - **Purpose**: The `type()` function is a built-in Python function that returns the type of an object.
   - **Syntax**: 
     ```python
     type(object)
     ```
   - **Example**:
     ```python
     print(type(arr))
     ```
     **Output:**
     ```
     <class 'numpy.ndarray'>
     ```

5. **Creating a NumPy Array from a Tuple**
   > You can easily create a NumPy array from a `tuple`.
   >
   > ```python
   > import numpy as np
   >
   > arr = np.array((10, 20, 30, 40, 50))
   >
   > print(f"ndarray created using tuple: {arr}")
   > ```
   >
   > **Output:**
   > ```
   > ndarray created using tuple: [10 20 30 40 50]
   > ```

-----------------------------------------------------------------------------------------------------------------------------------------------------

# Array Dimensions

1. **What is a Dimension in Arrays?**
   > A **dimension** in arrays refers to one level of array depth, indicating how many indices are needed to access an element. Nested arrays are arrays that have other arrays as their elements.

2. **Types of Arrays:**
   > - **0-D Array**: A scalar value with no dimensions (e.g., `5`).
   > - **1-D Array**: A single level of depth, like a list of values (e.g., `[1, 2, 3]`).
   > - **2-D Array**: An array of arrays, resembling a matrix (e.g., `[[1, 2, 3], [4, 5, 6]]`).
   > - **3-D Array**: An array of 2-D arrays, similar to a collection of matrices (e.g., `[[[1, 2, 3], [4, 5, 6]]]`).

3. **Key Points:**
   > - Each additional dimension increases the level of complexity and data representation.
   > - The number of dimensions determines how data is structured and accessed.

4. **Interesting Facts:**
   > - **Higher Dimensions**: Arrays can have more than three dimensions, such as 4-D arrays, which are used in advanced applications like video data processing.
   > - **Memory Layout**: The way arrays are stored in memory can differ based on their dimensions, affecting performance in computations.
   > - **Applications**: Multi-dimensional arrays are widely used in data analysis, machine learning, and scientific computing, making them essential in these fields.

5. **0-D Arrays**

   - **Definition:**
     > 0-D arrays, also known as scalars, are the simplest form of arrays. They contain only a single element. Each value in an array is considered a 0-D array.

   - **Example:**
     > Create a 0-D array with the value `55`:
     >
     > ```python
     > import numpy as np
     >
     > arr = np.array(55)
     >
     > print(arr)
     > ```
     >
     > **Output:**
     > ```
     > 55
     > ```

6. **1-D Arrays**

   - **Definition:**
     > A 1-D array, also known as a uni-dimensional array, is an array where each element is a 0-D array (a single value). This is the most common and basic type of array.

   - **Key Points:**
     > - 1-D arrays are like lists or sequences of numbers, making them easy to understand and use.
     > - They are ideal for storing simple data, like a list of numbers or a series of measurements.

   - **Interesting Fact:**
     > Did you know? In Python, a 1-D array can be seen as a row of values, which is why it’s often used to represent vectors in mathematics.

   - **Example:**
     > Create a 1-D array containing the values `20, 45, 22, 41, 96`:
     >
     > ```python
     > import numpy as np
     >
     > arr = np.array([20, 45, 22, 41, 96])
     >
     > print(arr)
     > ```
     >
     > **Output:**
     > ```
     > [20 45 22 41 96]
     > ```

7. **2-D Arrays in NumPy**

   - **Definition:**
     > A 2-D array contains 1-D arrays as elements, resembling a table with rows and columns.

   - **Usage:**
     > Used to represent matrices or second-order tensors.

   - **NumPy Matrix Operations:**
     > The submodule `numpy.mat` is designed for matrix manipulations.

   - **Interesting Facts:**
     > - **Shape**: Use `arr.shape` to get the number of rows and columns.
     > - **Element Access**: Access elements with two indices, e.g., `arr[0, 1]` (value `2`).
     > - **Matrix Operations**: Perform addition, multiplication, and inversion with NumPy functions.
     > - **Visualization**: Use libraries like Matplotlib to visualize 2-D arrays as images or heatmaps.

   - **Example:**
     > Create a 2-D array:
     >
     > ```python
     > import numpy as np
     >
     > arr = np.array([[1, 2, 3], [4, 5, 6]])
     >
     > print(arr)
     > ```
     >
     > **Output:**
     > ```
     > [[1 2 3]
     >  [4 5 6]]
     > ```

8. **3-D Arrays in NumPy**

   - **Definition:**
     > A 3-D array is an array that has 2-D arrays (matrices) as its elements. It can be visualized as a collection of matrices stacked together.

   - **Usage:**
     > 3-D arrays are often used to represent third-order tensors, which are useful in various applications, including computer graphics and data science.

   - **Interesting Facts:**
     > - **Shape**: You can use `arr.shape` to get the dimensions of the 3-D array, which shows the number of matrices, rows, and columns.
     > - **Element Access**: Access elements with three indices, e.g., `arr[0, 1, 2]` to get the value in the first matrix, second row, and third column.
     > - **Applications**: 3-D arrays are widely used in machine learning and deep learning to represent data such as images (height, width, channels).
     > - **Visualization**: Libraries like Matplotlib can be used to visualize 3-D data in various ways, including 3-D plots and surface plots.

   - **Example:**
     > Create a 3-D array:
     >
     > ```python
     > import numpy as np
     >
     > arr = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])
     >
     > print(arr)
     > ```
     >
     > **Output:**
     > ```
     > [[[1 2 3]
     >   [4 5 6]]
     >
     >  [[1 2 3]
     >   [4 5 6]]]
     > ```


