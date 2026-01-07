# GPU_Scheduling_Optimization
This project develops a multi-objective optimization model for scheduling jobs on heterogeneous GPU clusters using real workload data from the Alibaba cluster trace 

The objective is to balance fairness, efficiency, and operational cost when assigning jobs to GPU nodes.
Specifically, the model minimizes latency penalty to prioritize older jobs, maximizes GPU utilization, and minimizes communication overhead caused by job splitting across nodes.

The framework is implemented in GAMSPy using mixed-integer programming with constraints on CPU/GPU capacity, worker requirements, and GPU compatibility.
Three optimization approaches are explored: lexicographic (three-stage) optimization, weighted multi-objective optimization, and a scenario-based stochastic model to capture runtime uncertainty.

Pareto analysis is used to visualize trade-offs among objectives and guide decision-making.
Results show that no single scheduling policy is optimal under all conditions, highlighting the need for flexible, context-aware scheduling strategies.

## License Requirements to run this project:
Need a GAMS license to make sure the install the required solvers. The current project is run using an academic license. 

## Dataset
https://github.com/alibaba/clusterdata/tree/master/cluster-trace-v2026-spot-gpu


