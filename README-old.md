# Array Sorting Visualizer

An interactive browser-based tool that visualizes 5 classic sorting algorithms **simultaneously** — the array elements physically move and slide into place in real time.

**Made by Abdulrazzak Kouwider**

---

## Live Demo

Just open `array-sort-visualizer.html` in any modern browser — no installation, no build step, no dependencies.

---

## Algorithms

| Algorithm | Time Complexity | Space |
|---|---|---|
| Bubble Sort | O(n²) | O(1) |
| Insertion Sort | O(n²) | O(1) |
| Selection Sort | O(n²) | O(1) |
| Merge Sort | O(n log n) | O(n) |
| Quick Sort | O(n log n) avg | O(log n) |

---

## Features

- **Elements physically move** — each number is a tile that slides to its new position during swaps, not a bar chart
- **All 5 algorithms run in parallel** — compare them side by side in real time
- **Custom array input** — enter your own comma-separated numbers (e.g. `12, 5, 33, 8, 21`)
- **Speed control** — 5 levels from Slowest to Turbo
- **Live stats** — comparisons, swaps, and elapsed time tracked per algorithm
- **Color-coded states** — see exactly what each algorithm is doing at every step
- **Performance comparison panel** — bar chart breakdown shown after sorting completes

## Color Legend

| Color | Meaning |
|---|---|
| Purple | Elements being compared |
| Pink / Red | Elements being swapped |
| Orange | Pivot element (Quick Sort) |
| Cyan | Current minimum (Selection Sort) |
| Green | Element in its final sorted position |

---

## How to Use

1. Clone or download the repo
2. Open `array-sort-visualizer.html` in your browser
3. *(Optional)* Type your own array in the input field
4. Adjust the speed slider to your liking
5. Click **Sort All** — watch all 5 algorithms sort at the same time
6. Check the **Performance Comparison** panel at the bottom when done

---

## Tech Stack

- Pure **HTML / CSS / JavaScript** — zero dependencies, zero frameworks
- CSS `transform: translateX()` with transitions for smooth block movement
- `async/await` + `setTimeout` for step-by-step animation control
- All algorithms run concurrently via `Promise.all`

---

## Project Structure

```
array-sort-visualizer.html   # entire app in one file
README.md
```
