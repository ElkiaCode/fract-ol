# fract-ol

*An interactive fractal explorer written in C with MiniLibX, built as part of the 42 curriculum.*

fract-ol renders the **Mandelbrot** and **Julia** sets in real time. You can zoom toward the mouse cursor, pan, change the color palette and change how many iterations are computed.

## Build

Linux with X11 is required (`libx11-dev`, `libxext-dev`, `zlib1g-dev`). The project builds the bundled MiniLibX.

```bash
make
```

## Usage

```bash
./fractol Mandelbrot [max_iter]
./fractol Julia [max_iter] [c_real] [c_imaginary]

# examples
./fractol Mandelbrot 100
./fractol Julia 80 -0.8 0.156
```

When no values are given for Julia, it uses `c = 0 + 0.8i` and 50 iterations.

## Controls

| Input | Action |
|---|---|
| Mouse wheel | Zoom in / out toward the cursor |
| `W` `A` `S` `D` / arrow keys | Move the view |
| `1` `2` `3` | Change color palette |
| `0` | Turn color cycling on or off (the palette changes on every zoom) |
| `=` / `-` | Add or remove 5 iterations |
| `Esc` | Quit |

## Author

[ElkiaCode](https://github.com/ElkiaCode) (cparodi), 42 Nice.
