# Physics Simulator

## 1. About the Project
An interactive 2D Physics Simulator built with C++ and SFML that models projectile motion and initial launch velocity based on mouse interaction.

## 2. Mathematics & Physics Formulation
The simulation calculates the initial launch velocity ($V_0$) from the Euclidean distance between the mouse cursor ($M$) and the circle center ($M'$), then updates the velocity components over time ($t$):

$$
\begin{aligned}
h &= \|\overrightarrow{MM'}\| \\
V_0 &= \sqrt{2gh} \\
V_x(t) &= V_0 \sin(\alpha) \\
V_y(t) &= V_0 \cos(\alpha) - g \cdot t
\end{aligned}
$$

Where:
* **$M$**: Position vector of the mouse cursor.
* **$M'$**: Position vector of the circle.
* **$h$**: Distance between $M$ and $M'$.
* **$V_0$**: Initial launch speed.
* **$\alpha$**: Launch angle.
* **$g$**: Gravitational acceleration.

## 3. Prerequisites & Installing SFML
Before compiling the project, ensure you have **SFML** and a C++ compiler (`g++`) installed on your system:

### Linux
*(Watch step-by-step video guide: [How to install SFML on Linux](https://www.youtube.com/watch?v=Z7CAWvQN8oY))*

* **Ubuntu / Debian / Mint:**
  ```bash
  sudo apt-get update && sudo apt-get install libsfml-dev g++
  ```
* **Fedora / RHEL / CentOS:**
  ```bash
  sudo dnf install SFML-devel gcc-c++
  ```
* **Arch Linux / Manjaro:**
  ```bash
  sudo pacman -S sfml gcc
  ```
* **openSUSE:**
  ```bash
  sudo zypper install sfml2-devel gcc-c++
  ```
* **Alpine Linux:**
  ```bash
  sudo apk add sfml-dev g++
  ```
* **Other Distributions:** Download the source or SDK from the [Official SFML Download Page](https://sfml-dev.org).

### Windows
Download the SDK from the [Official SFML Download Page](https://sfml-dev.org) and link it to your compiler (Visual Studio / MinGW).
*(Watch step-by-step video guide: [How to Setup SFML on Windows](https://www.youtube.com/watch?v=qvg8BXXWpCE))*

## 4. Build & Run

### 1. Clone & Compile
Open your Terminal (Linux) or Command Prompt (Windows) and run:
```bash
git clone https://github.com
cd YOUR_REPO_NAME
g++ main.cpp -o circle_fall -lsfml-graphics -lsfml-window -lsfml-system
```

### 2. Run the Simulation
* **On Linux:**
  ```bash
  ./circle_fall
  ```
* **On Windows (CMD):**
  ```cmd
  circle_fall.exe
  ```

## 5. Version
`1.0.1`
