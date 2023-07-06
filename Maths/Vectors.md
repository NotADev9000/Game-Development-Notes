# Vectors
A quantity having **direction** as well as **magnitude**, especially as determining the position of one point in space relative to another.

2D Vector: `(x, y)`<br>
3D Vector: `(x, y, z)`

<br>

## Magnitude:
---
**Length** of a vector. Doesn't denote the Vector's direction.

Calculated with `pythagoras theorem`:
```c#
m = sqrt(x^2 + y^2 + z^2)
```

<br>

## Normalize:
---
The process of changing a Vector's **magnitude** to 1 while keeping it pointing in the same direction.

Sometimes called a **Unit Vector (u)** or **Directional Vector**.

<br>

```c#
u = v / |v| // vector / magnitude of vector
```

Calculated by dividing each element in the Vector by the Vector's **magnitude**.
