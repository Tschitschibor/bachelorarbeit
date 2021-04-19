# Bachelor thesis CatReps

[LaTeX](https://en.wikipedia.org/wiki/LaTeX) source files for my Bachelor thesis with title 
"The category of representations of a concrete category
as a functor category." 
The result of this thesis is the [Gap](https://github.com/gap-system/gap) package [CatReps](https://github.com/homalg-project/CatReps).

I have also given a talk on this subject, the slides and an example in form of a jupyter worksheet can be found in the sub-repository `catreps-seminar`.

## Build

The directory `3_Ausarbeitung/` contains the LaTeX source code.

There are two .tex files that can be compiled into .pdf files using the LaTeX compiler of your choice, e.g. [MiKTeX](https://miktex.org/).

The main file is `Bachelorarbeit_Tibor_Gruen.tex`.

The other file is `Nur_Algorithmen.tex` which only shows the code listings. It is also included in the Appendix A of the Bachelor thesis.

### Installing gap and some homalg-project packages

Both .tex files rely on specific versions of the following `Gap` packages in order to read the algorithm listings:

| Package name        | Version           | Sha  | Link |
| ------------- |:-------------| :-----| :-----------:|
| CatReps      | 2020.10-07 | ac2124f392067d30 | [CatReps](https://github.com/homalg-project/CatReps/commit/ac2124f392067d308570d16b4335d2c5b6d1d49f) |
| Algebroids      | 2020.10-12      |   4b47253d82f557c6 | [Algebroids](https://github.com/homalg-project/Algebroids/commit/4b47253d82f557c6f225d394d93671e1c7aceaf0) |
| FunctorCategories | 2020.10-04      | 2a57bc4cf1c81784 | [FunctorCategories](https://github.com/homalg-project/FunctorCategories/commit/2a57bc4cf1c8178431e827396bff94505b3f7bbd) |
| CategoryConstructor | 2020.10-02      | c0352cf43691044c | [CategoryConstructor](https://github.com/homalg-project/CategoryConstructor/commit/c0352cf43691044c7af3516ec4f51c3d148be1c4) |

They should be installed into your gap/pkg folder after installing `Gap`.

For instructions to install gap, see https://github.com/gap-system/gap

### Customize Pfad.tex

Edit the file `Pfad.tex.sample` to point towards
the `gap/pkg` directory and then rename it to `Pfad.tex`.

Now the LaTeX compiler will find the source files to include the algorithm listings in the appendix and the Nur_Algorithmen file.

## Dependencies

All used LaTeX packages and commands are in the file `definitions_packages.tex`

