# Mathematical Principles I (CES/RWTH Aachen)
This is a repository for the course *Mathematische Grundlagen I*
("Mathematical Principles I") for the Computational Engineering Science
bachelor program at RWTH Aachen University (winter term 2022/2023).

## Pluto notebooks
Notebooks available in this repository:
* **Notebook 1: Taylor series approximation**
  ([Pluto link](https://raw.githubusercontent.com/sloede/ces-math-1/main/notebooks/taylor_series_approximation.jl),
   [HTML preview](https://ces-math-1.lakemper.eu/notebooks/html/taylor_series_approximation.jl.html))
* **Notebook 2: Riemann integral**
  ([Pluto link](https://raw.githubusercontent.com/sloede/ces-math-1/main/notebooks/riemann_integral.jl),
   [HTML preview](https://ces-math-1.lakemper.eu/notebooks/html/riemann_integral.jl.html))
* **Notebook 3: Function approximation with orthonormal bases**
  ([Pluto link](https://raw.githubusercontent.com/sloede/ces-math-1/main/notebooks/orthonormal_basis.jl),
   [HTML preview](https://ces-math-1.lakemper.eu/notebooks/html/orthonormal_basis.jl.html))

If you are new to [Julia](https://julialang.org) and [Pluto.jl](https://github.com/fonsp/Pluto.jl),
follow the instructions [below](#getting-started-with-julia-and-pluto) to get started.

## Getting started with Julia and Pluto
The following description is roughly based on the excellent instructions
[here](https://computationalthinking.mit.edu/Spring21/installation/).

### Get Julia
To get Julia, go to
[https://julialang.org/downloads/](https://ces-math-1.lakemper.eu/)
and download the *current stable release*
of Julia (not the LTS version, no pre-releases etc.). Check out the
platform-specific instructions for more information, e.g., for
[Windows](https://julialang.org/downloads/platform/#windows),
[macOS](https://julialang.org/downloads/platform/#macos), or
[Linux](https://julialang.org/downloads/platform/#linux_and_freebsd).

### Get Pluto
Once Julia is installed, run the Julia executable
(`julia` on Linux/macOS, `julia.exe` on Windows) to start the Julia REPL. Then
execute the following commands (you can copy & paste them to the REPL prompt and
then hit *Enter*):
```julia
using Pkg
Pkg.add("Pluto")
```
This will install the Pluto package. Note that this step is only required once,
i.e., the second time you want to use Pluto you can directly proceed to
[running Pluto](#run-pluto).

### Run Pluto
After Julia and Pluto have been installed, you can run Pluto by starting the
Julia REPL and executing the following commands:
```julia
using Pluto
Pluto.run()
```
This should automatically open Pluto in your default browser. If not, find the
link in the Julia REPL that looks something like
`http://localhost:1234/?secret=1234abcd` and open it manually in your browser.

On the Pluto.jl landing page you will find a section titled "Open a notebook".
Copy one of the `Pluto link`s from the notebooks [above](#pluto-notebooks) into
the field and click "Open" to start the notebook.

*Note:* When a notebook is opened, its Julia code is executed once. Depending on
the notebook, this can take a few seconds. Once the notebook has been loaded
completely, everything should be snappy. When a notebook is opened for the *very
first time*, this delay can be even longer (tens of seconds), since Pluto might
have to install additional Julia packages.

## Author
This repository was initiated by [Michael Schlottke-Lakemper](https://lakemper.eu),
who is also its principal maintainer.

## License
The contents of this repository are licensed under the MIT license (see
[LICENSE.md](LICENSE.md)).
