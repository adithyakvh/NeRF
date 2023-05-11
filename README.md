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
