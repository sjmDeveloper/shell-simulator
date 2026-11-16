# 1. What is this app?
A Physics Simulator.

# 2. Mathematics & Physics Side
$$
\begin{aligned}
V_x(t) &= V_0 \sin(\alpha) \\
V_y(t) &= V_0 \cos(\alpha) - g \cdot t \\
\text{These are the } & \text{physics velocity equations:} \\
h &= \|\overrightarrow{MM'}\| \\
M &: \text{Point of mouse} \\
M' &: \text{Point of circle} \\
V_0 &= \sqrt{2gh}
\end{aligned}
$$

# Version:
`1.0.1`

# 6. Prerequisites & Installing SFML
Before compiling the project, make sure you have **SFML** installed on your system:

* **On Linux (Ubuntu/Debian):** Install directly via terminal:
  ```bash
  sudo apt-get update && sudo apt-get install libsfml-dev
  ```
  *(Watch step-by-step video guide: [How to install SFML on Linux](https://www.youtube.com/watch?v=Z7CAWvQN8oY))*

* **On Windows:** Download the SDK from the [Official SFML Download Page](https://sfml-dev.org) and link it to your compiler.
  *(Watch step-by-step video guide: [How to Setup SFML on Windows](https://www.youtube.com/watch?v=qvg8BXXWpCE))*

# 7. How to Run
1. Open your Terminal (Linux) or CMD (Windows) and navigate to the project folder:
```bash
cd your_file_path
```

2. Compile the code with SFML libraries linked:
```bash
g++ main.cpp -o circle_fall -lsfml-graphics -lsfml-window -lsfml-system
```
