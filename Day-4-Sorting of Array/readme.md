![day 4](https://github.com/user-attachments/assets/bc29cabf-b34f-40e4-9aab-8e5c2ef1bb4e)
<h1>Sorting Algorithms in C++</h1>
<p>Sorting is a key operation in Data Structures and Algorithms (DSA) used to arrange elements in a specific order, usually in ascending or descending order. Sorting makes data more manageable and helps improve the efficiency of other algorithms, such as searching and merging.</p>
<h2>1. Selection Sort</h2>
<p><strong>Explanation:</strong> Selection Sort works by repeatedly finding the minimum element from the unsorted portion and placing it at the beginning of the list. It divides the list into two parts: the sorted part and the unsorted part.</p>

<p><strong>Steps:</strong></p>
<ol>
    <li>Find the minimum element in the unsorted part.</li>
    <li>Swap it with the first element of the unsorted part.</li>
    <li>Move the boundary of the sorted part one element to the right.</li>
    <li>Repeat until the entire list is sorted.</li>
</ol>

<p><strong>Code:</strong></p>
<pre><code class="cpp">
#include &lt;iostream&gt;
#include &lt;vector&gt;
using namespace std;

void selectionSort(vector&lt;int&gt;& arr) {
    int n = arr.size();
    for (int i = 0; i &lt; n - 1; ++i) {
        int min_idx = i;
        for (int j = i + 1; j &lt; n; ++j) {
            if (arr[j] &lt; arr[min_idx]) {
                min_idx = j;
            }
        }
        swap(arr[i], arr[min_idx]);
    }
}

int main() {
    vector&lt;int&gt; arr = {64, 25, 12, 22, 11};
    selectionSort(arr);
    cout &lt;&lt; "Sorted array: ";
    for (int num : arr) {
        cout &lt;&lt; num &lt;&lt; " ";
    }
    cout &lt;&lt; endl;
    return 0;
}
</code></pre>

<h2>2. Bubble Sort</h2>

<p><strong>Explanation:</strong> Bubble Sort repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. This process is repeated until the list is sorted.</p>

<p><strong>Steps:</strong></p>
<ol>
    <li>Compare each pair of adjacent elements.</li>
    <li>Swap them if they are in the wrong order.</li>
    <li>Repeat until no swaps are needed.</li>
</ol>

<p><strong>Code:</strong></p>
<pre><code class="cpp">
#include &lt;iostream&gt;
#include &lt;vector&gt;
using namespace std;

void bubbleSort(vector&lt;int&gt;& arr) {
    int n = arr.size();
    for (int i = 0; i &lt; n - 1; ++i) {
        for (int j = 0; j &lt; n - i - 1; ++j) {
            if (arr[j] &gt; arr[j + 1]) {
                swap(arr[j], arr[j + 1]);
            }
        }
    }
}

int main() {
    vector&lt;int&gt; arr = {64, 34, 25, 12, 22, 11, 90};
    bubbleSort(arr);
    cout &lt;&lt; "Sorted array: ";
    for (int num : arr) {
        cout &lt;&lt; num &lt;&lt; " ";
    }
    cout &lt;&lt; endl;
    return 0;
}
</code></pre>

<h2>3. Insertion Sort</h2>

<p><strong>Explanation:</strong> Insertion Sort builds the final sorted array one item at a time. It takes each element from the unsorted part and inserts it into the correct position in the sorted part.</p>

<p><strong>Steps:</strong></p>
<ol>
    <li>Assume the first element is sorted.</li>
    <li>Take the next element and compare it with the elements in the sorted part.</li>
    <li>Shift all the elements in the sorted part that are greater than the new element to one position to the right.</li>
    <li>Insert the new element into its correct position.</li>
    <li>Repeat until the entire array is sorted.</li>
</ol>

<p><strong>Code:</strong></p>
<pre><code class="cpp">
#include &lt;iostream&gt;
#include &lt;vector&gt;
using namespace std;

void insertionSort(vector&lt;int&gt;& arr) {
    int n = arr.size();
    for (int i = 1; i &lt; n; ++i) {
        int key = arr[i];
        int j = i - 1;
        while (j &gt;= 0 && arr[j] &gt; key) {
            arr[j + 1] = arr[j];
            j--;
        }
        arr[j + 1] = key;
    }
}

int main() {
    vector&lt;int&gt; arr = {12, 11, 13, 5, 6};
    insertionSort(arr);
    cout &lt;&lt; "Sorted array: ";
    for (int num : arr) {
        cout &lt;&lt; num &lt;&lt; " ";
    }
    cout &lt;&lt; endl;
    return 0;
}
</code></pre>

<h2>Summary</h2>
<ul>
    <li><strong>Selection Sort:</strong> Efficient for small lists but has O(n²) time complexity.</li>
    <li><strong>Bubble Sort:</strong> Simple to understand but inefficient with O(n²) time complexity.</li>
    <li><strong>Insertion Sort:</strong> More efficient for small datasets and nearly sorted data, with a best-case time complexity of O(n) and worst-case O(n²).</li>
</ul>

<p>Each of these algorithms is easy to implement and understand, making them suitable for educational purposes and small datasets.</p>
