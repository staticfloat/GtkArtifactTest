# Testing GTK artifacts

To test, using Julia 1.3-rc4 or later, run the following:

```
julia --project=. -e 'import Pkg; Pkg.instantiate()'
julia --project=. -i imageview_test.jl
```

Installation and Precompilation can take a while, but eventually you should then see an image viewer pop up showcasing "The Face of Victory".

## Using these versions in your projects:

To use these JLL package versions of dependencies in your projects, open up the `pkg>` repl and add the following versions:

```julia
add https://github.com/staticfloat/Cairo.jl#sf/jll_packages
add https://github.com/JuliaMath/FFTW.jl#sf/jll_packages
add https://github.com/staticfloat/Gtk.jl#sf/jll_packages
add https://github.com/JuliaIO/ImageMagick.jl#sf/jll_packages
add https://github.com/JuliaMath/SpecialFunctions.jl#sf/jll_packages
add https://github.com/staticfloat/ZipFile.jl#sf/jll_packages
```

These versions will eventually be merged into their main packages, but as we are still testing Julia 1.3, the changes are still held on separate branches.
