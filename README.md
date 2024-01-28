# Hi everyone :wave:

I'm a researcher in scientific computing, developing software and algorithms for simulating complex
physical systems (fluids, bubbles, drops, and particles) on
supercomputers, and now blending them with machine learning tools to solve
inverse and control problems.
Currently working at [Harvard SEAS](https://cse-lab.seas.harvard.edu/people/petr-karnakov) in Cambridge, MA, United States.

You can see highlights of my work at [pkarnakov.com](https://pkarnakov.com),
reach me on social media [LinkedIn](https://www.linkedin.com/in/pkarnakov), [Twitter/X](https://twitter.com/pkarnakov),
and watch some of my simulation videos on [YouTube](https://www.youtube.com/@pkarnakov).

## Skills

The field of scientific computing is multidisciplinary and highly collaborative.

<details>
<summary>
Skills related to each aspect of my research work
</summary>

* mathematical model (mechanics, calculus, differential equations)
* discretization (numerical methods, linear algebra)
* software implementation (C++, Python)
* high-performance computing (MPI, OpenMP, OpenCL, vectorization, x86 assembly)
* project tools (CMake, CI/CD, Docker)
* inverse and control problems (optimization, machine learning, TensorFlow, Bayesian inference)
* publishing and communication (LaTeX, scientific writing, oral presentation)
* visualization, slides, and demos (ParaView, Keynote, reveal.js, JavaScript, HTML)

I have collaborated with over 20 fellow researchers from several institutions around the globe (US, Switzerland, Germany, France, Russia)
and presented my work at 8 international conferences.
</details>

## Research projects
<details open>
<summary>
Projects done as part of my research work
</summary>

### [ODIL](https://github.com/cselab/odil)

ODIL (Optimizing a DIscrete Loss) is a method for solving inverse problems for partial differential equations,
which is orders of magnitude faster than PINN (physics-informed neural networks).

| Body from flow | Poisson | Wave | Heat |
|:---:|:---:|:---:|:---:|
| [<img src="https://pkarnakov.com/media/tile_bodyinfer.jpg" width=100>](https://academic.oup.com/pnasnexus/article/3/1/pgae005/7516080#437357793) | [<img src="https://pkarnakov.com/media/wasm_poisson.png" width=100>](https://pkarnakov.github.io/autodiff/demos/poisson.html) | [<img src="https://pkarnakov.com/media/wasm_wave.png" width=100>](https://pkarnakov.github.io/autodiff/demos/wave.html) | [<img src="https://pkarnakov.com/media/wasm_heat.png" width=100>](https://pkarnakov.github.io/autodiff/demos/heat.html) |

### [Aphros](https://github.com/cselab/aphros)

Aphros is a distributed multiphysics solver for simulating multiphase
flow with bubbles and electrochemical reactors.
The solver performed first-ever simulations
of foaming by breakup and mixing of air in water.

| Foaming | Electrolysis | Drops | Gallery |
|:---:|:---:|:---:|:---:|
| [<img src="https://pkarnakov.com/media/tile_waterfall.jpg" width=100>](https://www.youtube.com/watch?v=0Cj8pPYNJGY) | [<img src="https://pkarnakov.com/media/tile_reactor.jpg" width=100>](https://www.youtube.com/watch?v=Rm-xDGpIEJA) | [<img src="https://pkarnakov.com/media/wasm_hydro.png" width=100>](https://cselab.github.io/aphros/wasm/hydro.html) | [<img src="https://pkarnakov.com/media/wasm_gallery.png" width=100>](https://github.com/cselab/aphros/wiki/Aphros-Explorer) |

</details>

## Hobby projects
<details open>
<summary>
Spare-time projects to learn something or have fun
</summary>

### [ptoy](https://github.com/pkarnakov/ptoy)

Particle toy with bonds and portals. You can connect particles to create ropes,
run them through portals, and manipulate with the mouse.
Written in C++ with OpenGL and SDL2. The web version uses WebAssembly.

| Native | [Web](https://pkarnakov.github.io/ptoy/ptoy.html) |
|:---:|:---:|
|<img src="https://pkarnakov.github.io/ptoy/images/ptoy_native.png" height="120">|<img src="https://pkarnakov.github.io/ptoy/images/ptoy_web.png" height="120"> |

### [autodiff](https://github.com/pkarnakov/autodiff)

Automatic differentiation in C++ with GPU support through OpenCL.

This project has certainly made automatic differentiation frameworks less
intimidating for me. I've realized that some machine learning tasks that would
normally rely on TensorFlow/JAX/PyTorch can actually be solved in pure C++
from scratch in a reasonable amount of time (Christmas holidays).
And for small problems on a CPU it also works 10x times faster
than the corresponding Python+TensorFlow implementation.
The ODIL demos above (and [here](https://github.com/pkarnakov/autodiff#interactive-demos))
use this code to run through WebAssembly.

Examples of constructed computational graphs:

<img src="https://pkarnakov.github.io/autodiff/media/reverse_scal1.svg" height="150"><img src="https://pkarnakov.github.io/autodiff/media/poisson/poisson.svg" height="150">

</details>
