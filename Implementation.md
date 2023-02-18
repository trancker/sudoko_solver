## Implementation Details

The basic idea is that using OpenCV we can find the contour with the largest area. This mostly will give us the sudoku grid but it may not be in the correct perspective. We can use perpsective transform after finding out the corner points using a line sweep method. This transform would give us the sudoku cropped and transformed to a square grid. Now we can simply iterate over the 81 blocks and after processing it to remove noise pass the pixel data to a neural network to recognise the digit. Then we can easily solve the sudoku using a heuristic c++ sudoku solver.


### A portal has been created in Flask to provide a user friendly GUI front end for the sudoku solver: