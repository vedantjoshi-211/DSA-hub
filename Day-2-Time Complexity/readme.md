![day2](https://github.com/user-attachments/assets/a57294bf-3a27-4e4e-8a3c-78adac5cba65)

<h1>What is Time Complexity?</h1>
    <p>Time complexity is a computational concept used to describe the amount of time an algorithm takes to run as a function of the length of its input. It provides a theoretical measure of the runtime performance of an algorithm, which helps in understanding and comparing the efficiency of different algorithms.</p>
    <h1>Cases of Time Complexity</h1>
    <p>In time complexity analysis, we consider different scenarios based on the input data to understand how the algorithm's execution time behaves. There are three main cases to consider:</p>
    <h2>Best Case (Ω(n))</h2>
    <p>This refers to the minimum amount of time an algorithm takes to execute for an input of size <code>n</code>. It represents the scenario where the algorithm encounters the most favorable conditions. For example, in searching a sorted array, the best case would be the target element being present at the first position. Big Omega notation (Ω) is used to express the best case.</p>
    <h2>Average Case (Θ(n))</h2>
    <p>This represents the typical execution time the algorithm takes on average, considering all possible inputs of size <code>n</code> with equal probability. It's important to note that this can be difficult to determine for some algorithms. Big Theta notation (Θ) is used to express the average case.</p>
    <h2>Worst Case (O(n))</h2>
    <p>This refers to the maximum amount of time an algorithm takes to execute for an input of size <code>n</code>. It represents the scenario where the algorithm encounters the least favorable conditions. For example, in searching an unsorted array, the worst case would be having to compare the target element with every element in the array. Big O notation (O) is used to express the worst case, and it's the most commonly used case for analysis because it guarantees an upper bound on the execution time.</p>
    <h1>Summary Table</h1>
    <table border="1">
        <thead>
            <tr>
                <th>Case</th>
                <th>Notation</th>
                <th>Description</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Best Case</td>
                <td>Ω(n)</td>
                <td>Minimum execution time</td>
            </tr>
            <tr>
                <td>Average Case</td>
                <td>Θ(n)</td>
                <td>Typical execution time on average</td>
            </tr>
            <tr>
                <td>Worst Case</td>
                <td>O(n)</td>
                <td>Maximum execution time</td>
            </tr>
        </tbody>
    </table>
    <h1>Rules to Find Time Complexity</h1>
    <ol>
      <h2>(1) Ignore constant factors. </h2> <br>For example, 3n + 2 becomes n.
      <h2> (2) After ignoring constants, choose the term with the highest growth rate. </h2> <br>example, 2n^3 + 3n^2 + 2n becomes n^3 (because n^3 grows faster than n^2 and n as the input size increases).</li>
    </ol>
    <h1> Example (Hand written) </h1>
    <a href="https://drive.google.com/file/d/1znwQ_-lzn4nbqQmZS5vRq4Q_r1fMwc3b/view?usp=drive_link">here are all exaples</a>
    <h1>Time Complexity Practice Problems</h1>
    <p>This repository contains a collection of practice problems to help understand and analyze the time complexity of various code snippets.</p>
    <h2>Problems and Time Complexities</h2>
    <h3>1. Code:</h3>
    <pre>
for(int i=1; i&lt;=n*n; i++) 
    cout &lt;&lt; "DSA-HUB";
    </pre>
    <p><strong>Time Complexity:</strong> O(n^2)</p>
    <h3>2. Code:</h3>
    <pre>
for(int i=1; i&lt;=n*n; i=i+2) 
    cout &lt;&lt; "DSA-HUB";
    </pre>
    <p><strong>Time Complexity:</strong> O(n^2)</p>
    <h3>3. Code:</h3>
    <pre>
for(int i=1; i&lt;=n; i++) 
    for(int j=1; j&lt;=n; j=j+5)
        cout &lt;&lt; "DSA-HUB";
    </pre>
    <p><strong>Time Complexity:</strong> O(n^2/5) or O(n^2)</p>    
    <h3>4. Code:</h3>
    <pre>
for(int i=1; i&lt;=n; i++) 
    for(int j=i; j&lt;=n; j=j++)
        cout &lt;&lt; "DSA-HUB";
    </pre>
    <p><strong>Time Complexity:</strong> O(n^2)</p>    
    <h3>5. Code:</h3>
    <pre>
for(int i=1; i&lt;=n; i++) 
    for(int j=1; j&lt;=n; j=j*4)
        cout &lt;&lt; "DSA-HUB";
    </pre>
    <p><strong>Time Complexity:</strong> O(n log n)</p>   
    <h3>6. Code:</h3>
    <pre>
for(int i=1; i&lt;=n; i=i*2) 
    for(int j=1; j&lt;=i; j=j++)
        cout &lt;&lt; "DSA-HUB";
    </pre>
    <p><strong>Time Complexity:</strong> O(n)</p>    
    <h3>7. Code:</h3>
    <pre>
for(int i=1; i&lt;=n; i++) 
    for(int j=1; j&lt;=n; j=j++)
        for(int k=1; k&lt;=n; k=k*3)
            cout &lt;&lt; "DSA-HUB";
    </pre>
    <p><strong>Time Complexity:</strong> O(n^2 log n)</p> 
    <h3>8. Code:</h3>
    <pre>
for(int i=1; i&lt;=n; i++) 
    for(int j=1; j&lt;=n; j=j++)
        for(int k=1; k&lt;=n; k++)
            cout &lt;&lt; "DSA-HUB";
    </pre>
    <p><strong>Time Complexity:</strong> O(n^3)</p>
