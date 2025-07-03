# 🧠 A* Pathfinding Visualizer in Python

An interactive visualization tool for the A* (A-star) pathfinding algorithm, built using Python and Pygame. This project combines algorithmic logic with intuitive design to help learners and developers explore how A* efficiently finds the shortest path in a grid-based environment.

![A* Visualization Demo](https://upload.wikimedia.org/wikipedia/commons/5/5d/Astar_progress_animation.gif)  


---

## 🚀 Features

- 🧭 **A* Algorithm Implementation**  
  Real-time visualization of the A* pathfinding algorithm with `g`, `h`, and `f` score computations and priority queue management.

- 🎨 **Interactive Grid-Based UI**  
  Use mouse and keyboard to place:
  - Start and End points  
  - Barriers (walls)  
  - Erasers for removing nodes

- 🖱️ **Intuitive Controls**
  - Left-click to place start, end, or walls
  - Right-click to erase
  - Press **Space** to start the algorithm
  - Press **C** to clear the grid

- 🧱 **Grid Representation with Color Coding**
  - White: Unvisited node  
  - Black: Barrier  
  - Orange: Start  
  - Turquoise: End  
  - Red: Already evaluated nodes  
  - Green: Nodes currently in open set  
  - Purple: Final path  

- ♻️ **Reset and Replay**  
  Clear and re-run the algorithm without restarting the program.

---


## 📦 Installation & Setup

### Requirements
- Python 3.x
- `pygame`

### Installation

```bash
git clone https://github.com/YOUR_USERNAME/AStar-Visualizer.git
cd AStar-Visualizer
pip install -r requirements.txt
```
---

## Run the Program

```bash
python main.py
```
---

## 🧠 How It Works

-**Grid Creation**
  Initializes a 2D grid where each cell is a Spot object with position, color, and neighbor      tracking.

-**User Interaction**

  -Left‑click: place start, end, or walls

  -Right‑click: erase

  -Spacebar: run A*

  -C: clear grid

-**A* Algorithm Execution**

  -Maintain g_score, h_score (Manhattan), and f_score = g + h.

  -Use a priority queue to pick the lowest‑f node each step.

  -Update neighbor scores and track predecessors in came_from.

-**Path Reconstruction**
  Backtrack from the end node via the came_from map to draw the shortest path.

---

##📐 Heuristic Function

```python
Copy
Edit
def h(p1, p2):
    return abs(p1.x - p2.x) + abs(p1.y - p2.y)
```
##🙋 Author
Vivek C K
