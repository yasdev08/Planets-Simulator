# Planet Simulation

A simple **planetary simulation** using **Python** and **Pygame**, demonstrating gravitational interactions between celestial bodies in a 2D space. The simulation models the Sun, planets of the Solar System, and Pluto, showing their orbits and trails.

---

## Features

- Simulates gravitational forces between celestial bodies using **Newton's law of universal gravitation**.
- Realistic orbital motion of planets.
- **Trails** for visualizing the paths of the bodies.
- **Zoom toggle** to switch between normal and zoomed-in scales.
- Adjustable **time step** for orbital calculations.

---

## Requirements

- Python 3.8+
- [Pygame](https://www.pygame.org/news)

Install Pygame via pip:

```bash
pip install pygame
How to Run
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/planet-simulation.git
cd planet-simulation
Run the simulation:

bash
Copy code
python simulation.py
Controls:

Press Z to toggle zoom mode.

Close the window to quit.

How It Works
Each planet (and the Sun) is represented as a Body object with properties:

Position (x, y)

Velocity (vx, vy)

Mass

Radius (for display)

Color

The simulation calculates the gravitational force between every pair of bodies using the formula:

ini
Copy code
F = G * (m1 * m2) / r^2
Where:

G is the gravitational constant

m1 and m2 are the masses of the two bodies

r is the distance between them

Acceleration is calculated as:

ini
Copy code
a = F / m
Velocity and position are updated using Euler integration.

Trails are stored to show the path of each body.

Zooming changes the scale factor to give a closer look at the inner planets.

Notes
This is a 2D simplified simulation. It ignores relativistic effects and assumes all motion is in a single plane.

Units used:

Distance in meters

Mass in kilograms

Time step: 1 day (DT = 86400 seconds)

Visual radius is for display purposes only and does not affect calculations.

Example Screenshot

Orbits of planets around the Sun.
