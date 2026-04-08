# Lift Algorithm Optimisation

A Python simulation that models elevator operations in multi-lift buildings. Compares scheduling algorithms (FCFS, SCAN, LOOK, and two custom strategies) with real-time visualisation and performance analytics.

## Features

- Multi-lift simulation with configurable speed, acceleration, and capacity
- 5 scheduling algorithms: FCFS, SCAN, LOOK, MYLIFT, PATHFINDER (custom)
- Real-time GUI visualisation (Tkinter) and monitoring dashboard (wxPython)
- Performance analytics with Matplotlib (wait times, turnaround times, efficiency)
- Realistic passenger request generation with weight modelling

## Tech Stack

- **Language:** Python 3.9+
- **Visualisation:** Tkinter, wxPython, Matplotlib
- **Computation:** NumPy, SciPy

## How to Run

```bash
git clone https://github.com/NoeBouchard/Lift_algorithm-optimisation.git
cd Lift_algorithm-optimisation
pip install wxPython matplotlib numpy scipy
python simulation.py
```

## Project Structure

```
├── simulation.py       # Main entry point
├── algorithms.py       # Scheduling strategies (FCFS, SCAN, LOOK, custom)
├── lift.py             # Core elevator logic
├── liftmanager.py      # Multi-lift coordination
├── generator.py        # Passenger request generation
├── request.py          # Request data model
├── gui.py              # Tkinter real-time visualisation
├── monitoring.py       # wxPython monitoring dashboard
└── graph.py            # Matplotlib analytics and reporting
```

## Algorithms

| Algorithm | Strategy |
|-----------|----------|
| FCFS | First-come, first-served — serves requests in arrival order |
| SCAN | Elevator sweeps up and down, serving requests in path |
| LOOK | Like SCAN but reverses at the last request, not the top/bottom floor |
| MYLIFT | Custom heuristic-based scheduling |
| PATHFINDER | Custom optimised routing algorithm |

## License

MIT
