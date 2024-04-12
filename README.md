## **METHODOLOGY:**

1. ***Function for matrix multiplication:***  matrix_multiply() is defined to perform matrix multiplication of two matrices (A and B) using np.dot(). It stores the answer at the specific index of result array.

2. ***Function for multiplication using threads:***  run_with_threads() is defined to perform matrix multiplication with a specified number of threads.
It first initializes a list threads to store the thread objects.
Then, it iterates over the list of matrices and creates a new thread for each matrix multiplication operation using threading.Thread() constructor.
Each thread is started using the start() method. After creating all threads, it waits for all threads to complete using the join() method. The function returns the time taken for the multiplication operations.

3. ***Matrices Definition:*** The constant matrix A of size 1000x1000 is generated using numpy.random.rand(). A list of 100 random matricesof the same size is created.

4. ***Execution:*** run_with_threads() function is called for each number of threads in the range from 1 to 10, and the time taken for each operation is recorded. The results are stored in the results_table list, along with the corresponding number of threads.

5. ***Results:*** The results are displayed in a table format using the tabulate() function.

6. ***Plotting:*** The number of threads and the corresponding time taken are plotted using matplotlib.pyplot.plot() and plot is displayed using plt.show().

### **OBSERVATIONS:**
The time taken is minimum for number of threads= 8 which is justified as there are 8 cores on my laptop.

![123](https://github.com/gleegazer16/Multi-Threading-Assignment-UCS654/assets/100419223/58dc5d63-b9ff-4f07-b2ea-710e9833fe67)

![321511686-e85868bb-acf6-4b9e-8bac-6773a634222c](https://github.com/gleegazer16/Multi-Threading-Assignment-UCS654/assets/100419223/d05fc065-93fd-41fa-8398-a9d38103bc7b)
