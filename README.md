# 🧭 BFS Maze Traversal 🗺️

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🔍 Overview

BFS Maze Traversal is a visual maze-solving application that demonstrates the breadth-first search (BFS) algorithm in action. Watch in real-time as the algorithm explores the maze and finds the optimal path from start to finish!

## ✨ Features

- 🎮 Terminal-based visual interface using the curses library
- 🔄 Real-time visualization of the search algorithm
- ⚡ Breadth-first search implementation for finding the shortest path
- 🎨 Color-coded display for better visibility
- 🧩 Customizable maze layouts

## 🚀 Getting Started

### Prerequisites

- Python 3.6+
- curses library (built-in for Unix systems, requires `windows-curses` package for Windows)

### Installation

1. Clone this repository:
   ```
   git clone https://github.com/qusai-Kagalwala/bfs-maze-traversal.git
   cd bfs-maze-traversal
   ```

2. For Windows users only:
   ```
   pip install windows-curses
   ```

3. Run the program:
   ```
   python path-finder.py
   ```

## 🎮 How It Works

- **O**: Starting point
- **X**: Target destination
- **#**: Wall
- **[Space]**: Open path

The algorithm starts at the **O** position and explores all possible paths using breadth-first search until it finds the target **X**. The path is visualized in real-time, showing exactly how BFS explores the maze.

## 🛠️ Customizing the Maze

You can customize the maze by editing the `maze` array in `path-finder.py`. Follow these guidelines:

```python
maze = [
    ["#", "O", "#", "#", "#", "#", "#", "#", "#"],  # O is the starting point
    ["#", " ", " ", " ", " ", " ", " ", " ", "#"],  # Space represents open paths
    ["#", " ", "#", "#", " ", "#", "#", " ", "#"],  # # represents walls
    ["#", " ", "#", " ", " ", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", "#", "#"],
    ["#", " ", " ", " ", " ", " ", " ", " ", "#"],
    ["#", "#", "#", "#", "#", "#", "#", "X", "#"]   # X is the target
]
```

## 🧠 Algorithm Details

The project implements the **Breadth-First Search (BFS)** algorithm, which guarantees finding the shortest path in an unweighted graph. Key aspects include:

- Uses a queue data structure to track exploration
- Maintains a visited set to avoid cycles
- Builds the path incrementally as it explores
- Visualizes the exploration process with a time delay

## 📝 Future Enhancements

- [ ] Add support for Dijkstra's and A* algorithms
- [ ] Implement maze generation algorithms
- [ ] Add ability to load mazes from files
- [ ] Create difficulty levels with increasingly complex mazes
- [ ] Add stats display (path length, exploration coverage, etc.)

## 🤝 Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add some amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a pull request

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Inspired by pathfinding visualizers
- Built with Python and curses
- Special thanks to all maze algorithm enthusiasts!

---

⭐ If you found this project interesting, please consider giving it a star! ⭐

Made with ❤️ by Qusai Kagalwala
