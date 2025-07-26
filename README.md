Algorithm Visualizer
This project is a web-based interactive tool designed to help users understand fundamental searching and sorting algorithms through visual representation. It allows you to generate a dataset, select an algorithm, and watch as the algorithm processes the data step-by-step, highlighting key operations and providing a trace log of its execution.

Features
Algorithm Selection: Choose from a variety of common searching and sorting algorithms.

Dynamic Data Generation: Generate random datasets of customizable sizes (10 to 200 elements).

Interactive Visualization: Observe the algorithms in action with a dynamic bar chart representation of the data array.

Step-by-Step Trace Log: A detailed log explains each operation performed by the algorithm, providing insights into its logic.

Pause/Resume/Reset Controls: Full control over the visualization playback.

Responsive Design: Adapts to different screen sizes for a consistent user experience.

Supported Algorithms
The following algorithms are currently implemented and visualized:

Linear Search: A simple search algorithm that sequentially checks each element of the list until a match is found or the whole list has been searched.

Binary Search: An efficient algorithm for finding an item from a sorted list of items. It works by repeatedly dividing in half the portion of the list that could contain the item, until you've narrowed down the possible locations to just one.

Bubble Sort: A simple sorting algorithm that repeatedly steps through the list, compares adjacent elements and swaps them if they are in the wrong order.

Insertion Sort: A simple sorting algorithm that builds the final sorted array (or list) one item at a time. It iterates through the input elements and removes one element per iteration, finds the place within the sorted array and inserts it there.

Visualization Details
The primary visualization uses a bar chart where each bar represents an element in the dataset. The height of the bar corresponds to its value.

Color Coding:
Default Blue: Elements that are part of the active dataset but not currently involved in an operation.

Amber (Orange-500): checking - The element currently being examined (e.g., in Linear Search).

Emerald (Green-500): found / sorted - The target element has been found (in search algorithms) or an element is confirmed to be in its final sorted position.

Red (Red-500): low - Used in Binary Search to highlight the 'low' pointer.

Purple (Purple-500): high - Used in Binary Search to highlight the 'high' pointer.

Pink (Pink-500): mid - Used in Binary Search to highlight the 'mid' pointer.

Violet (Violet-400): comparing - Elements currently being compared (e.g., in Insertion Sort, Bubble Sort).

Orange (Orange-400): inserting - The element being moved or inserted (in Insertion Sort).

Pink (Pink-400): swapping - Elements actively being swapped (in Bubble Sort).

Grey Shades (Gray-200 to Gray-900): discarded-level-X - Used in Binary Search to progressively grey out portions of the array that have been eliminated from the search space. Darker shades indicate earlier discards.

How to Use
Generate Data:

Set the desired "Data Size" (between 10 and 200).

Click the "Generate Data" button. A new random array will be displayed and visualized.

(For Binary Search, the data will be automatically sorted upon generation as it requires a sorted input.)

Choose Algorithm:

Select an algorithm from the "Choose Algorithm" dropdown.

If you select Linear Search or Binary Search, an input field for "Target Value" will appear. Enter the number you wish to search for.

Start Visualization:

Click the "Start Visualization" button. The algorithm will begin executing step-by-step, updating the visualization and the trace log.

Control Playback:

Pause/Resume: Click the "Pause" button to temporarily halt the animation. Click it again (it will change to "Resume") to continue.

Reset: Click the "Reset" button to return the visualization to its initial state (original data or initially sorted data for Binary Search).

Observe Trace Log:

The "Trace" box at the bottom provides a textual description of each step the algorithm takes, offering a deeper understanding of its operations.

Technologies Used
HTML5: For the basic structure of the web page.

Tailwind CSS: A utility-first CSS framework for rapid and responsive styling.

JavaScript (ES6+): For implementing the algorithms, controlling the visualization logic, and handling user interactions.
