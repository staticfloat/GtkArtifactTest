# Testing GTK artifacts

To test, using Julia 1.3-rc4 or later, run the following:

```
julia --project=. -e 'import Pkg; Pkg.instantiate()'
julia --project=. -i imageview_test.jl
```

Installation and Precompilation can take a while, but eventually you should then see an image viewer pop up showcasing "The Face of Victory".
