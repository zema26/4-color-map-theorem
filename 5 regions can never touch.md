To prove mathematically why five regions can never mutually touch on a 2D plane, graph theory translates the map into a "dual graph." Each region becomes a single point (vertex), and the shared border between any two regions becomes a line (edge) connecting them.

If five regions could all touch one another, their dual graph would be a Complete Graph with 5 vertices, known as K5. In this configuration, every vertex connects directly to the other four, resulting in exactly 10 edges.

Key insight: No matter how you arrange the 5 nodes, the moment you try to draw the 10th connection, you are forced to cross an existing line.

The Mathematical Trap (Euler's Formula)

The impossibility is formally proven by Euler's Formula for planar graphs, which dictates that for any flat, non-crossing network, the Vertices (V), Edges (E), and Faces/empty spaces (F) must always satisfy V - E + F = 2.
 * Calculate the Faces: For a K5 graph, V = 5 and E = 10. Plugging these into Euler's formula (5 - 10 + F = 2) means F would have to equal 7.
 * The Geometric Rule: In any simple planar graph without self-looping edges, every face (including the infinite background area outside the graph) must be bounded by a minimum of 3 edges.
 * The Edge Count: If there are 7 faces, and each requires a minimum of 3 edges, you count at least 21 "boundary edges" (7 x 3).
 * The Contradiction: Every single edge on the graph serves as a boundary for exactly two faces. Therefore, the maximum sum of all face boundaries is exactly 2E. For K5, this is 2 x 10 = 20.

The math creates an impossible scenario where 20 >= 21. Because this statement is false, a K5 graph physically cannot exist on a flat plane without edges crossing.
In physical map terms, once you draw four mutually touching regions, their borders form a completely closed ring. A fifth region is physically blocked: it must exist either entirely inside that ring or entirely outside it, preventing it from touching at least one of the original four.
