# Evolutionary Community Detection

Bachelor’s thesis by Felix Fröschl, University of Passau.

## Abstract

Community detection based on modularity optimization is widely used for identifying structural organization in complex networks. However, classical scalar modularity maximization imposes a fixed trade-off between intra-community density and null-model expectation, potentially obscuring alternative yet structurally meaningful partitions.

This work reformulates modularity as a multiobjective optimization problem by decomposing it into its constitutive components. Instead of aggregating these competing terms into a single scalar objective, both are optimized simultaneously. To solve the resulting problem, a locus-based genetic algorithm combined with NSGA-II selection and a portfolio of complementary mutation operators is proposed. The mutation design integrates local node relocation, community merge operations and a restricted Louvain-based refinement step to enable structural adaptation at multiple scales.

The algorithm is evaluated on standard benchmark graphs, including Zachary’s Karate Club and the American College Football network. The results demonstrate robust convergence behaviour and a high probability of reaching the global modularity optimum under moderate computational budgets. Moreover, the multiobjective formulation exposes a structured Pareto front that reveals alternative community configurations beyond the scalar optimum.

Overall, the study indicates that multiobjective evolutionary optimization provides additional structural transparency while maintaining competitive convergence properties compared to classical modularity maximization.
