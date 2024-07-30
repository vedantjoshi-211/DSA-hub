
![day6](https://github.com/user-attachments/assets/ddacf2e6-c5bb-4ec6-b5a4-027db3fbb45d)



<h1>2D Arrays in Data Structures and Algorithms (DSA) using C++</h1>
    <p>In data structures and algorithms (DSA), a 2D array is a fundamental concept that extends the idea of a one-dimensional array. A 2D array can be thought of as a grid or a table, consisting of rows and columns, where each element is accessed using two indices. This structure is particularly useful for representing matrices, game boards, images, and other grid-based data.</p>

  <h2>Definition and Declaration</h2>
    <p>A 2D array in C++ is essentially an array of arrays. It can be declared in various ways depending on the requirements. Here's a basic declaration:</p>
    <pre><code>type arrayName[rows][columns];</code></pre>
    <p>For example, to declare a 2D array of integers with 3 rows and 4 columns, you can write:</p>
    <pre><code>int arr[3][4];</code></pre>

  <h2>Initialization</h2>
    <p>A 2D array can be initialized at the time of declaration. Here are a few ways to do this:</p>
    <h3>1. Initializing with specific values:</h3>
    <pre><code>int arr[3][4] = {
    {1, 2, 3, 4},
    {5, 6, 7, 8},
    {9, 10, 11, 12}
};</code></pre>
    <h3>2. Partially initializing:</h3>
    <pre><code>int arr[3][4] = { 
    {1, 2}, 
    {3, 4}, 
    {5, 6} 
}; // Remaining elements will be initialized to 0.</code></pre>
    <h3>3. Default initialization (all elements to zero):</h3>
    <pre><code>int arr[3][4] = {0};</code></pre>

  <h2>Accessing Elements</h2>
    <p>Elements in a 2D array are accessed using two indices: one for the row and one for the column. The syntax is:</p>
    <pre><code>arrayName[row][column]</code></pre>
    <p>For instance, to access the element in the second row and third column of the array <code>arr</code>, you would write:</p>
    <pre><code>int value = arr[1][2]; // Remember, indices start from 0.</code></pre>

  <h2>Iterating through a 2D Array</h2>
    <p>A common operation with 2D arrays is iterating through all elements. This can be done using nested loops:</p>
    <pre><code>for(int i = 0; i < 3; i++) {
    for(int j = 0; j < 4; j++) {
        std::cout << arr[i][j] << " ";
    }
    std::cout << std::endl;
}</code></pre>

  <h2>Common Applications</h2>
    <ul>
        <li><strong>Matrices:</strong> 2D arrays are used to represent matrices in mathematical computations.</li>
        <li><strong>Grids:</strong> Games like Tic-Tac-Toe, Sudoku, and Minesweeper use 2D arrays to represent the playing field.</li>
        <li><strong>Images:</strong> In image processing, a 2D array can represent a grayscale image where each element corresponds to a pixel's intensity.</li>
  </ul>

  <h2>Advantages and Disadvantages</h2>
    <h3>Advantages:</h3>
   <ul>
        <li>Simple representation of matrix-like data structures.</li>
        <li>Easy to access and manipulate individual elements using row and column indices.</li>
  </ul>
    <h3>Disadvantages:</h3>
    <ul>
        <li>Fixed size: The size of a 2D array must be known at compile-time and cannot be changed dynamically.</li>
        <li>Memory consumption: Large 2D arrays can consume a significant amount of memory.</li>
  </ul>
<h3>HANDWRITTEN NOTES</h3>
<a href = "https://drive.google.com/file/d/19caUgOnQyzLYBiTMdA9UBrgrGd07atMm/view?usp=sharing"> NOTES </a>
