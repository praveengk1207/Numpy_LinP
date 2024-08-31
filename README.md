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
