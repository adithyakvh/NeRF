# NeRF
In this project, the goal is to represent a 3D scene in a convenient and compact way,
to be later used for rendering 2D images. A 3D scene can be considered a set of points that contain
color and density. Though every fixed point in the scene has a fixed density, that’s not the case with
the color. Each point can have a different color depending on the viewing direction if we assume the
surface to be non-Lambertian.

Thus a 3D scene is representing by the mapping (x, y, z, θ, ϕ) = (x, d) → (c, σ) where x = (x, y, z)
is the 3D position of a point in the scene, d = (θ, ϕ) is the viewing direction, c = (r, g, b) is the color
of the point and σ is its density. The problem we will try to solve here, and the one that the NeRF
paper approached, is that given a number of 2D views of the same static scene, to be able to render
novel views of that scene.

![image](https://github.com/adithyakvh/NeRF/assets/42107613/a6735fd7-2d40-4016-868d-a3c074fcf86e)

The novel view that is rendered is below.


![NeRF Target](https://github.com/adithyakvh/NeRF/assets/42107613/2ec3d1f8-33ce-4f74-b2fc-6eace7090c35)


![download](https://github.com/adithyakvh/NeRF/assets/42107613/1e53fae0-cc46-425d-9eca-68dac4a51ee4)
