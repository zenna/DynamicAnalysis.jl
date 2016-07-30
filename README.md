# DynamicAnalysis

Benchmark and compare your algorithms.

# Usage

DynamicAnalysis exports two important types `Problem` and `Algorithm` and two important functions `benchmark` and `record`.

Subtype Problem and Algorithm

```julia

OptimizationProblem <: Problem
  obj_function::Function
  captures::Vector{Symbol}
end

x_squared = OptimizationProblem(x->x^2, [:optimal_cost])
```

```julia

OptimizationAlgo <: Algorithm
  solver::
end


```

