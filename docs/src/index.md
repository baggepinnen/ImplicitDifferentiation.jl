```@meta
CurrentModule = ImplicitDifferentiation
```

# ImplicitDifferentiation.jl

[ImplicitDifferentiation.jl](https://github.com/gdalle/ImplicitDifferentiation.jl) is a package for automatic differentiation of functions defined implicitly.

## Background

Implicit differentiation is useful to differentiate through two types of functions:

- Those for which automatic differentiation fails. Reasons can vary depending on your backend, but the most common include calls to external solvers, mutating operations or type restrictions.
- Those for which automatic differentiation is very slow. A common example is iterative procedures like fixed point equations or optimization algorithms.

Please refer to [_Efficient and modular implicit differentiation_](https://arxiv.org/abs/2105.15183) for an introduction to the underlying theory.

## Getting started

To install the stable version, open a Julia REPL and run:

```julia
julia> using Pkg; Pkg.add("ImplicitDifferentiation")
```

For the latest version, run this instead:

```julia
julia> using Pkg; Pkg.add(url="https://github.com/gdalle/ImplicitDifferentiation.jl")
```

Check out the API reference to know more about the main object defined here, [`ImplicitFunction`](@ref).
The tutorials give you some ideas of real-life applications for our package.

## Related projects

- [DiffOpt.jl](https://github.com/jump-dev/DiffOpt.jl): differentiation of convex optimization problems
- [InferOpt.jl](https://github.com/axelparmentier/InferOpt.jl): differentiation of combinatorial optimization problems
- [NonconvexUtils.jl](https://github.com/JuliaNonconvex/NonconvexUtils.jl): contains the original implementation from which this package drew inspiration