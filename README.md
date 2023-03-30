# SIR model
## Repository Title
### About This Project

This is a test SIR modelt hat is based on Ottar's book code from chapter 2. It is a simple SIR model with births and deaths.
It uses fractional populations.

```math
\begin{align}
\frac{dS}{dt} &= \mu (N - S) -\beta S \frac{I}{N} \\
\frac{dI}{dt} &= \beta S \frac{I}{N} - \gamma I - \mu I \\
\frac{dR}{dt} &= \gamma I - \mu R
\end{align}
```

```math
\begin{align}
\mu &= \frac{1}{50*52} \\
\beta &= 2 \\
\gamma &= \frac{1}{2} \\\\

N &= 1000 \\
S_0 &= 999.0 \\
I_0 &= 1.0 \\
R_0 &= 0.0
\end{align}
```

### Repository Structure

```
.
├── data/
├── figs/
├── funs/
├── out/
└── src/
```

- `data/` contains ...
- `figs/` contains ...
- `funs/` contains ...
- `out/` contains ...
- `src/` contains ...

### Built With

- [R version 4.2.1 (2022-06-23)](https://cran.r-project.org/bin/macosx/)
- [`{renv}`](https://rstudio.github.io/renv/articles/renv.html) for package management
- [`{deSolve}`](https://cran.r-project.org/web/packages/deSolve/index.html) for solving differential equations

### Getting Started
I've used the `{renv}` package to manage the R environment for this project.
For more details on how to use `{renv}`, see [this article](https://rstudio.github.io/renv/articles/renv.html), but in brief, it creates a snapshot of the installed packages and their versions.

To get started, you will need to install `{renv}` as usual (i.e., `install.packages("renv")`), and then run `renv::restore()` to install the packages that are used in this project (the record in the ***renv.lock*** file).

### Usage
To run the SIR model, you can open the ***src/sir_model.R*** file and run the code as usual.

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

### Contact
tsb5404@psu.edu

### Acknowledgements
Ottar's book
