# AlcyonRegistry

Julia package registry that contains all the Alcyon packages.

## Development

To add new packages to this registry, follow these steps:

1. open julia repl, pkg mode
2. make sure to activate global environment: `activate`
3. add this registry if not already added: `registry add git@github.com:alcyon-lab/AlcyonRegistry.git`
4. install LocalRegistry.jl package if not installed: `add LocalRegistry`
5. activate the package to be added to the registry: `activate /path/to/package`
6. run: 
```julia
using LocalRegistry
register(registry="AlcyonRegistry")
```
