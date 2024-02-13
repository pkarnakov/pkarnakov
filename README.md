# Hi everyone :wave:

I'm a research scientist developing software and numerical algorithms
for simulation, control, and design of complex physical systems.
My interests range from classical numerical methods to data-driven techniques and machine learning,
with a focus on software engineering and high-performance computing.
List of [publications](https://pkarnakov.com/pub.html).
Currently working at [Harvard University](https://cse-lab.seas.harvard.edu/people/petr-karnakov) in Cambridge, MA, United States.

You can see examples of my work at [pkarnakov.com](https://pkarnakov.com),
reach me on social media [LinkedIn](https://www.linkedin.com/in/pkarnakov), [Twitter/X](https://twitter.com/pkarnakov),
and watch some of my simulation videos on [YouTube](https://www.youtube.com/@pkarnakov/videos).

## Research Projects

### [ODIL](https://github.com/cselab/odil)

ODIL (Optimizing a DIscrete Loss) is a method for solving inverse problems for partial differential equations,
which is orders of magnitude faster than PINN (physics-informed neural networks).

<details>
<summary>
Demos
</summary>

| Poisson | Wave | Heat |
|:---:|:---:|:---:|
| [<img src="https://pkarnakov.com/media/wasm_poisson.png" width=100>](https://pkarnakov.github.io/autodiff/demos/poisson.html) | [<img src="https://pkarnakov.com/media/wasm_wave.png" width=100>](https://pkarnakov.github.io/autodiff/demos/wave.html) | [<img src="https://pkarnakov.com/media/wasm_heat.png" width=100>](https://pkarnakov.github.io/autodiff/demos/heat.html) |
</details>

### [Aphros](https://github.com/cselab/aphros)

Distributed multiphysics solver for simulating multiphase flow with bubbles and electrochemical reactors.
The solver performed the largest simulations of foaming by breakup and mixing of air in water.

<details>
<summary>
Videos and demos
</summary>

| <img src="http://pkarnakov.com/media/icon_youtube.png" width=16> Foaming | <img src="http://pkarnakov.com/media/icon_youtube.png" width=16> Electrolysis | Drops | Gallery |
|:---:|:---:|:---:|:---:|
| [<img src="https://pkarnakov.com/media/tile_waterfall.jpg" width=100>](https://www.youtube.com/watch?v=0Cj8pPYNJGY) | [<img src="https://pkarnakov.com/media/tile_reactor.jpg" width=100>](https://www.youtube.com/watch?v=Rm-xDGpIEJA) | [<img src="https://pkarnakov.com/media/wasm_hydro.png" width=100>](https://cselab.github.io/aphros/wasm/hydro.html) | [<img src="https://pkarnakov.com/media/wasm_gallery.png" width=100>](https://github.com/cselab/aphros/wiki/Aphros-Explorer) |
</details>

## Other Projects

### [autodiff](https://github.com/pkarnakov/autodiff)

Automatic differentiation framework in C++ with GPU support through OpenCL.

<details>
<summary>
Story and examples
</summary>
This project made me realize that some machine learning applications that would
normally rely on TensorFlow/JAX/PyTorch can actually be implemented in pure C++
from scratch in a reasonable amount of time (several days).
And for small problems on a CPU it also works 10x times faster
than the corresponding Python+TensorFlow implementation.
The ODIL demos above use this code to run in WebAssembly.
Examples of constructed computational graphs:

<img src="https://pkarnakov.github.io/autodiff/media/reverse_scal1.svg" height="150"><img src="https://pkarnakov.github.io/autodiff/media/poisson/poisson.svg" height="150">
</details>

### [ptoy](https://github.com/pkarnakov/ptoy)

Game with particles and portals. Written in C++ with OpenGL and SDL2. There is a <a href="https://pkarnakov.github.io/ptoy/ptoy.html">web version</a>.

<details>
<summary>
Description and screenshots
</summary>
You can connect particles to create ropes, run them through portals, and manipulate with the mouse.
The <tt>accel</tt> button couples the gravity vector with measurements from an accelerometer (if supported).

| Native | [Web](https://pkarnakov.github.io/ptoy/ptoy.html) |
|:---:|:---:|
|<img src="https://pkarnakov.github.io/ptoy/images/ptoy_native.png" height="120">|<img src="https://pkarnakov.github.io/ptoy/images/ptoy_web.png?1" height="120"> |
</details>

### [AM205](https://github.com/pkarnakov/am205#gallery)

Visual materials for a class on numerical methods that I lectured in 2022.

<details>
<summary>
Removing day-night cycle from videos using PCA. <a href="https://github.com/pkarnakov/am205/blob/main/media/unit2/media/pcavideo/pcavideo.py">Code</a> | <a href="https://pkarnakov.github.io/am205/slides/unit2/#/167">Slides</a>
</summary>

<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_paris.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_paris.gif" height=100 alt="pcavideo_paris.mp4"></a>
<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_paris_first3.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_paris_first3.gif" height=100 alt="pcavideo_paris_first3.mp4"></a>
<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_paris_zero3.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_paris_zero3.gif" height=100 alt="pcavideo_paris_zero3.mp4"></a><br>
<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_vietnam.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_vietnam.gif" height=100 alt="pcavideo_vietnam.mp4"></a>
<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_vietnam_first3.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_vietnam_first3.gif" height=100 alt="pcavideo_vietnam_first3.mp4"></a>
<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_vietnam_zero3.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_vietnam_zero3.gif" height=100 alt="pcavideo_vietnam_zero3.mp4"></a><br>
<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_sunrise.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_sunrise.gif" height=100 alt="pcavideo_sunrise.mp4"></a>
<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_sunrise_first3.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_sunrise_first3.gif" height=100 alt="pcavideo_sunrise_first3.mp4"></a>
<a href="http://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_sunrise_zero3.mp4"><img src="https://pkarnakov.github.io/am205/slides/unit2/media/pcavideo/pcavideo_sunrise_zero3.gif" height=100 alt="pcavideo_sunrise_zero3.mp4"></a>
</details>

<details>
<summary>
Sound of the wave equation. <a href="https://github.com/pkarnakov/am205/blob/main/media/unit3/media/wave.py">Code</a> | <a href="https://pkarnakov.github.io/am205/slides/unit3/#/191">Slide</a>
</summary>

The forcing signal excites certain frequencies of an oscillator. Videos with (loud) sound:

| Forcing | Response |
|:---:|:---:|
| <a href="http://pkarnakov.github.io/am205/slides/unit3/media/wave_force.webm"><img src="https://pkarnakov.github.io/am205/slides/unit3/media/wave_force.gif" height=100 alt="wave_force.webm"></a> | <a href="http://pkarnakov.github.io/am205/slides/unit3/media/wave_signal.webm"><img src="https://pkarnakov.github.io/am205/slides/unit3/media/wave_signal.gif" height=100 alt="wave_signal.webm"></a> |
</details>

### [TinyOS](https://github.com/pkarnakov/tinyos)

Prototype operating system in x86 assembly.

<details>
<summary>
Story and screencast
</summary>
I started this project back in 2008 for a school competition in Russia's space capital Korolyev.
The plan was to push Windows out of the market, but it didn't work out.

<a href="http://pkarnakov.github.io/tinyos/media/tinyos.mp4"><img src="https://pkarnakov.github.io/tinyos/media/tinyos.gif" height=150 alt="tinyos.mp4"></a>
</details>
