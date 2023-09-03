# Triangle Art - Triangles filled with a crazy pattern

You click on the screen three times to draw a triangle with a random color.
The application fills the triangle with a crazy inner triangle pattern.

Algorithm for the pattern:

```
    // Draw a dot between the first 2 edges
    currentDot = midpoint(edges[0], edges[1])
    drawDot(currentDot)

    loop 50000
        // Draw a dot between the last drawn dot and a random edge
        currentDot = midpoint(currentDot, getRandomEdge())
        drawDot(currentDot)

```