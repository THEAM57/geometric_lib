
# How to use calculator:
1. Run `python calculate.py`
2. Enter the figure name. Available are Circle, Square.
3. Enter the function: Area or Perimeter.
4. Enter figure sizes. Radius for circle, one side for square.
5. Get the answer!

# Math formulas
## Area
- Circle: `S = πR²`
- Rectangle: `S = ab`
- Square: `S = a²`
- Triangle: `S = sqrt(p * (p-a) * (p-b) * (p-c))` where p is semiperimeter

## Perimeter
- Circle: `P = 2πR`
- Rectangle: `P = 2a + 2b`
- Square: `P = 4a`
- Triangle: `P = a + b + c`


# Description

1. Import Modules: The program assumes the existence of `circle` and `square` modules, which contain functions for calculating the perimeter and area of the respective shapes.

2. Lists of Shapes and Functions: 
   - `figs` — a list of available shapes: `'circle'` and `'square'`.
   - `funcs` — a list of available functions: `'perimeter'` and `'area'`.

3. Sizes Dictionary: - `sizes` — a dictionary that can be used to store information about the required dimensions for each combination of shape and function. In the current code, it is not populated.

4. Function `calc`:
   - Takes as input the name of the shape (`fig`), the name of the function (`func`), and a list of dimensions (`size`).
   - Checks that the shape and function are in the respective lists.
   - Calculates the result using the `eval` function, calling the appropriate function from the imported module (`circle` or `square`).
   - Prints the result in the format: `"{func} of {fig} is {result}"`.

5. Main Program Block:
   - Prompts the user to input the shape, function, and dimensions until they are correct.
   - Uses a `while` loop to ensure valid input.
   - Once valid data is obtained, it calls the `calc` function to compute and display the result.

# Example of Operation:

- The user inputs the name of the shape.
- The user selects a function.
- The user inputs the necessary dimensions.
- The program calculates and displays the area of the circle with the given radius.


# Functions
## Calc
### Appointment
- Calculates and outputs the result of a function for a given shape.
### Parameters
- `fig (str)`: Name of the shape (`circle` or `square`)
- `size (list)`: The size of the figure.
### Example
- `calc('circle', 'area', [5])` - Returns the area of a circle with a radius of 5.


## Square - area
### Appointment
- Calculates the area of a square on a given side.
### Parameters
- `a (float)` is the length of the side of the square.
### Example
- `area(4)` - Returns the area of the square with side 4.



## Square - perimeter 
### Appointment
- Calculates the perimeter of a square on a given side.
### Parameters
- `a (float)` - The length of the side of the square.
### Example
- `perimeter(4)` - Returns the perimeter of the square with side 4.



## Circle - area
### Appointment
- Calculates the perimeter (circumference) of a circle by a given radius.
### Parameters
- `r (float)` - The radius of the circle.
### Example
- `perimeter(5)` - Returns the perimeter of a circle with a radius of 5.



## Circle - perimeter
### Appointment
- Calculates the perimeter (circumference) of a circle by a given radius.
### Parameters
- `float` - The perimeter of the circle.
### Example
- `perimeter(5)` - Returns the perimeter of a circle with a radius of 5.



## Triangle - area
### Appointment
- Calculates the half-diameter of a triangle based on the specified lengths of its sides.
### Parameters
- `a (float)` - The length of the first side of the triangle.
- `b (float)` - The length of the second side of the triangle.
- `c (float)` - The length of the third side of the triangle.
### Example
- `perimeter(3, 4, 5)` - Returns the perimeter of the triangle with sides 3, 4 and 5.



## Triangle - perimeter
### Appointment
-   Calculates the perimeter of a triangle based on the specified lengths of its sides.
### Parameters
-   `a (float)`: The length of the first side of the triangle.
-   `b (float)`: The length of the second side of the triangle.
-   `c (float)`: The length of the third side of the triangle.
### Example
-   `perimeter(3, 4, 5)` - Returns the perimeter of the triangle with sides 3, 4 and 5.

# History of changes and hashes of the commits
### commit d76db2ac7f69cc920ae2e6f669fb0671a7fa7d71  
Author: Daniil.K `<dlkay@yandex.ru>`  
Date:   Tue Mar 30 17:57:42 2021 +0300  
L-04: Add calculate.py

### commit 51c40ebfd0e0b65f52fe5e54740cbb038e492db3
Author: smartiqa `<info@smartiqa.ru>`  
Date:   Fri Mar 26 14:52:26 2021 +0300  
L-04: Doc updated for triangle

### commit d080c7888b81955bad2ed78d58ad910526b5132a  
Author: smartiqa `<info@smartiqa.ru>`  
Date:   Fri Mar 26 14:48:39 2021 +0300  
L-04: Triangle added

### commit d078c8d9ee6155f3cb0e577d28d337b791de28e2 (upstream/main, upstream/HEAD, origin/main, origin/HEAD, main)  
Author: smartiqa `<info@smartiqa.ru>`  
Date:   Thu Mar 4 14:55:29 2021 +0300
L-03: Docs added

### commit 8ba9aeb3cea847b63a91ac378a2a6db758682460  
Author: smartiqa `<info@smartiqa.ru>`  
Date:   Thu Mar 4 14:54:08 2021 +0300  
L-03: Circle and square added