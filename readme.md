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
````
Clone the repository :
```bash
git clone https://github.com/yasdev08/planets-simulator.git
cd planets-simulator
````
Run the simulation:
```bash
python planet_orbit.py
```
Controls:
```bash
Press Z to toggle zoom mode.
```
Close the window to quit.

**How It Works**

- Each planet is represented as a Body object with properties:

- Position (x, y)

- Velocity (vx, vy)

- Mass

- Radius (for display)

- Color

The simulation calculates the gravitational force between every pair of bodies using the formula:
```bash
F = G * (m1 * m2) / r^2
```
Where:

- G is the gravitational constant

- m1 and m2 are the masses of the two bodies

- r is the distance between them

Acceleration is calculated as:
```bash
a = F / m
```
Velocity and position are updated using Euler integration.

Trails are stored to show the path of each body.

Zooming changes the scale factor to give a closer look at the inner planets.

**Notes**
This is a 2D simplified simulation. It ignores relativistic effects and assumes all motion is in a single plane.

Units used:

- Distance in meters

- Mass in kilograms

- Time step: 1 day (DT = 86400 seconds)

Visual radius is for display purposes only and does not affect calculations.

Example Screenshot

<img width="1000" height="749" alt="Capture d&#39;écran 2025-12-06 080545" src="https://github.com/user-attachments/assets/76db21e4-a30e-4c18-bf94-98bc9e8b3752" />

Orbits of planets around the Sun.

