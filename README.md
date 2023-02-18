## Visual Sudoku Solver

This is a project that uses OpenCV in Python to recognise the sudoku grid and digits which will be classified using a neural network and then a C++ utility will solve the sudoku and output the final solved state.

The front end of the site is created in Flask and can be deployed on a webserver that has Keras/Tensorflow installed on it. It is possible to use the simpler neural network implementation based on NumPy by changing the model code but it gives poorer results and for usability the convulational version is recommended.

