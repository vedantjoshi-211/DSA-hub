![day3](https://github.com/user-attachments/assets/b04ab615-addc-4a94-8c9a-1827edf85fd7)

<h1>Arrays :-</h1>
    <p>In Data Structures and Algorithms (DSA) using C++, an array is a collection of elements, all of the same type, stored in contiguous memory locations. Arrays are one of the simplest and most widely used data structures. Here are the key points about arrays in C++:</p>   
    <h1>Characteristics of Arrays:-</h1>
    <ul>
        <li><strong>Fixed Size</strong>: The size of an array is determined at the time of declaration and cannot be changed dynamically.</li>
        <li><strong>Same Data Type</strong>: All elements in an array are of the same type.</li>
        <li><strong>Contiguous Memory Locations</strong>: Elements are stored in contiguous memory locations, which allows efficient indexing.</li>
        <li><strong>Indexing</strong>: Array elements can be accessed randomly using indices, which start at 0.</li>
    </ul>
    <h1>Declaration and Initialization:-</h1>
    <h3>Declaration:</h3>
    <pre><code>int arr[10]; // declares an array of 10 integers</code></pre>
    <h3>Initialization:</h3>
    <pre><code>int arr[5] = {1, 2, 3, 4, 5}; // declares and initializes an array</code></pre>
    <h3>Accessing Elements:</h3>
    <pre><code>int value = arr[2]; // accesses the third element (index 2)
arr[4] = 10;        // sets the fifth element (index 4) to 10</code></pre>
    <h1>Multidimensional Arrays:-</h1>
    <p>C++ also supports multidimensional arrays, such as 2D arrays, which are essentially arrays of arrays.</p>
    <h3>Declaration and Initialization of a 2D Array:</h3>
    <pre><code>int matrix[3][4] = {
    {1, 2, 3, 4},
    {5, 6, 7, 8},
    {9, 10, 11, 12}
};</code></pre>
    <h3>Accessing Elements in a 2D Array:</h3>
    <pre><code>int value = matrix[1][2]; // accesses the element in the second row and third column
matrix[2][3] = 15;        // sets the element in the third row and fourth column to 15</code></pre>
    <h1>Advantages of Arrays:-</h1>
    <ul>
        <li><strong>Efficiency</strong>: Fast access to elements using indices.</li>
        <li><strong>Simplicity</strong>: Easy to declare and use.</li>
    </ul>
    <h1>Limitations of Arrays:-</h1>
    <ul>
        <li><strong>Fixed Size</strong>: Cannot change the size once declared.</li>
        <li><strong>Memory Allocation</strong>: May waste memory if the array size is overestimated, or may run out of space if underestimated.</li>
        <li><strong>Insertion and Deletion</strong>: Inserting or deleting elements can be inefficient, as it may require shifting elements.</li>
    </ul>
    <h1>Use Cases:-</h1>
    <p>Arrays are used in various applications such as:</p>
    <ul>
        <li>Storing a collection of elements like scores, names, etc.</li>
        <li>Implementing other data structures like stacks, queues, and matrices.</li>
        <li>Algorithms that require quick access to elements using indices.</li>
    </ul>
    <h1>Declaration and Initialization Examples:-</h1>
    <h3>Default Initialization</h3>
    <pre><code>int arr[5]; // Declares an array of 5 integers. Values are undefined (may contain garbage values).</code></pre>
    <h3>Static Initialization</h3>
    <pre><code>int arr[5] = {1, 2, 3, 4, 5}; // Declares and initializes an array with 5 elements.</code></pre>
    <h3>Partial Initialization</h3>
    <pre><code>int arr[5] = {1, 2}; // First two elements are initialized to 1 and 2, rest are 0.</code></pre>
    <h3>Initialization with Default Values</h3>
    <pre><code>int arr[5] = {0}; // All elements are initialized to 0.</code></pre>
    <h3>Automatic Size Determination</h3>
    <pre><code>int arr[] = {1, 2, 3, 4, 5}; // Compiler determines the size of the array (5 in this case).</code></pre>
