# 🧠 A* Pathfinding Visualizer in Python

An interactive visualization tool for the A* (A-star) pathfinding algorithm, built using Python and Pygame. This project combines algorithmic logic with intuitive design to help learners and developers explore how A* efficiently finds the shortest path in a grid-based environment.

 
![Screenshot 2025-07-04 013049](https://github.com/user-attachments/assets/b3de8cc4-a019-4ebe-8c50-fe070c69a6d3)

![image](https://github.com/user-attachments/assets/759cb506-5591-442f-9ef5-0611e46bd1c8)

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

## 🧠 A* Algorithm Execution

- Maintain g_score, h_score (Manhattan), and f_score = g + h.

- Use a priority queue to pick the lowest‑f node each step.

- Update neighbor scores and track predecessors in came_from.

---

## Path Reconstruction
  Backtrack from the end node via the came_from map to draw the shortest path.

---

## 📐 Heuristic Function

```python
Copy
Edit
def h(p1, p2):
    return abs(p1.x - p2.x) + abs(p1.y - p2.y)
```
## 🙋 Author
Vivek C K
