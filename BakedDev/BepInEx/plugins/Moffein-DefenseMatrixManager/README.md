## DefenseMatrixManager

Allows mods to create Defense Matrixes that can block hitscan attacks on a per-team basis.

**Projectile deletion functionality is not included**, and should be handled by your own custom logic.

This mod was mainly made for my own personal mods since they share this functionality.

## How to Implement

1. Create a `DefenseMatrixManager.DefenseMatrixInfo` instance.
	- This should contain all colliders to be included.
	- TeamIndex of the owner.
	
2. Add `DefenseMatrixInfo` instance to the `DefenseMatrixManager` using  `DefenseMatrixManager.AddMatrix(DefenseMatrixInfo)`.

3. When destroying your GameObject, remove your `DefenseMatrixInfo` using `DefenseMatrixManager.RemoveMatrix(DefenseMatrixInfo)`.

If you want to automatically handle `DefenseMatrix` instance lifecycle, add a `DefenseMatrixComponent` to your prefab (requires `TeamFilter`), and it will automatically handle it for you.