## Genetic Boids:
This is my second boids simulation. It is a real time flocking simulator that in my case, uses rgb a sort of stand in for genes. The boids evolve and as they do their colors change to reflect this. Boids only flock with boids of the same genetic marker.

## What it does:
When you run the sim, a single boid named adam begins to fly in a random direction. After a while, he will die of old age, and split into n children who will all inheret his rgb genes, with some random mutation. These children will then fly on until they too die and split apart.
When a boid dies, their children are given an exact copy of the rgb values that determined the parents color. Each color channel is mutated randomly. Depending on which channel is most dominant, their color gene marker is set to r, g or b. Then, their color is biased slightly
towards that color. Boids flock with other boids of the same genetic type, and avoid others. Its very interesting to see two large flocks hit eachother and quickly repulse eachother. Its also interesting to see how sometimes in a large flock, children will mutate to a different
genetic marker and rapidly depart from the group. 

## Demo:
![giphy](https://github.com/user-attachments/assets/5dd8644e-1970-475c-b73c-a56de93756f5)
<img width="2559" height="1439" alt="Screenshot 2025-08-14 221108" src="https://github.com/user-attachments/assets/ea54332b-7ee9-4c91-bcc7-affaf72e82db" />



## Key Features
- Real-time genetic algorithm simulation
- Spatial partitioning optimization (O(n²) → mostly O(n))
- Live parameter adjustment
- Emergent flocking behavior
- Color-coded genetic traits

## Technologies Used
- Python and Pygame

## Notable Techniques 
- Spatial Data Structures like a dictionary to partition boids.
- Sampling for clamping expensive operations at high boid density.

## How to run
```bash
pip install pygame
python main.py



