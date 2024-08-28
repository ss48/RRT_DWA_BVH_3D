# RRT_DWA_BVH_3D
RRT_DWA_BVH
#the RRT and DWA algorithms function with the optimized collision checking using Bounding Volume Hierarchies (BVH).
#BVH Implementation: We use an R-tree (a type of BVH) to store axis-aligned bounding boxes (AABB) for each obstacle. This allows us to quickly identify which obstacles might intersect with a given point or path segment.
#Efficient Collision Checking: Instead of checking every obstacle for collision, we first use the BVH to narrow down the list to only those obstacles whose bounding boxes intersect with the point or path segment in question.
#Integration with DWA: The code remains the same in terms of how paths are generated and optimized, but now the collision checking is more efficient, leading to faster overall performance.
