# urban-flooding
literatur review

1. Multi-Scale Target-Specified Sub-Model Approach for Fast
Large-Scale High-Resolution 2D Urban Flood Modelling

Urban floods are an increasing threat due to ongoing urbanization and climate change.

Effective flood forecasting systems are crucial for early warnings and require accurate, timely spatial and temporal flood predictions.
 
This research reviews two primary types of flood models: 2D hydrodynamic models and 1D static models.

The study aims to develop a complementary 1D/2D solution that maximizes the strengths of both model types while minimizing their limitations.

Improving Computational Efficiency in 2D Urban Flood Models:

This excerpt discusses various strategies employed to enhance the computational efficiency of 2D hydrodynamic urban flood models, which are often computationally expensive, especially when dealing with high-resolution data. It outlines four main approaches used to speed up these models, acknowledging that while these methods reduce computational costs, handling vast amounts of high-accuracy remote sensing data remains a challenge.

Main Idea:
To address the high computational cost of 2D urban flood models, particularly with high-resolution data, researchers have developed several speed-up approaches focusing on # parallelization, # model simplification, # grid coarsening with detail compensation, and # cellular automata.

Explanation of Details
Improving the computational efficiency of 2D hydrodynamic models is crucial for their practical application, especially in large-scale and real-time scenarios. The paper identifies four primary strategies:

Parallelization Technology
This approach leverages advanced computing hardware and software to distribute the computational load, allowing for faster processing. Technologies utilized include:

Graphics Processing Units (GPUs): These are specialized electronic circuits designed to rapidly manipulate and alter memory to accelerate the creation of images in a frame buffer intended for output to a display device. Their parallel architecture makes them highly effective for computational tasks.
Multi-core Central Processing Units (MCs): Modern CPUs often have multiple processing cores that can execute instructions simultaneously, speeding up computations.
Remotely Distributed Computers and Cloud Computing: This involves using networks of computers or cloud-based services to perform computations, such as JFLOW-GPU 
[
1
]
, OpenMP 
[
1
]
, MPI libraries 
[
1
]
, FloodMap-Paraller model 
[
1
]
, and CityCAT 
[
1
]
.
Simplified Hydrodynamic Models
These models aim to reduce computational time by solving simplified governing equations. While they may offer reasonable flood extents and depths quickly, they often place less emphasis on momentum conservation, which can affect the accuracy of flow dynamics. Examples include:

Inertial LISFLOOD-FP 
[
1
]
Quasi 2D models 
[
1
]
Coarse-Grid Approach with Detail Compensation
Computational time can be reduced by increasing the grid size (using a coarser grid) 
[
1
]
. However, this can lead to a loss of accuracy due to the smearing of details, especially around complex structures like buildings. To mitigate this, various improvements have been introduced:

Sub-grid treatment 
[
1
]
Multi-cell approach 
[
1
]
Multi-layered approach 
[
1
]
Porosity parameter approach 
[
1
]
Cellular Automata (CA) Approach
This method involves coding a universal transition rule for spatial discretization in the simulation, leading to a reduced-complexity procedure in 2D models 
[
1
]
. CA models simplify the simulation of complex systems by breaking them down into a grid of cells, each following simple rules, which can significantly reduce computational demands.

Despite these advancements, the paper notes that these technologies, while reducing costs to some extent, still struggle to handle the immense volumes of data from new, fast-approaching remote sensing technologies that offer enhanced data accuracy 
[
1
]
. The use of high-resolution modeling grids is a prerequisite for explicitly including all detailed spatial representations in 2D simulations, making the computational efficiency of 2D models a continuous challenge in the context of high-resolution data 
[
1
]
.

Key Terms Glossary
Hydrodynamic Models: Mathematical models that simulate the movement of water, including its depth, velocity, and flow patterns, often used for flood prediction.
Digital Elevation Models (DEMs): Digital representations of terrain surface, containing elevation data for a given area, crucial for accurate flood modeling.
Cellular Automata (CA): A discrete model that consists of a grid of cells, each in one of a finite number of states, with the state of each cell evolving over time according to a set of rules based on the states of its neighbors.
