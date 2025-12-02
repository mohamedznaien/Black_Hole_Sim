# Black Hole Gravitational Lensing Simulator

A real-time 2D visualization of light bending near a Schwarzschild black hole, built with C++ and OpenGL.



## Physics

This simulation models photon trajectories near a non-rotating black hole using:

- **Schwarzschild metric** for spacetime geometry
- **Geodesic equations** for light path calculation
- **4th-order Runge-Kutta** numerical integration
- **Conserved quantities** (energy E, angular momentum L) from metric symmetries

The black hole is modeled after Sagittarius A* (~4 million solar masses).

## Controls

- **Space** - Pause/Resume
- **R** - Restart simulation

## Build (macOS)
```bash
brew install glew glfw glm
g++ bh.cpp -o bh $(pkg-config --cflags --libs glew glfw3) -I$(brew --prefix glm)/include -framework OpenGL
./bh
```

## Next Steps

- 3D visualization with accretion disk
- Kerr metric (rotating black holes)
- GPU acceleration (CUDA/OpenCL)

