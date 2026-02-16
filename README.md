# Unused Bone Track Remover

A Godot editor plugin that removes animation tracks referencing bones that no longer exist in the target `Skeleton3D`.

## How to use

1. Select an `AnimationPlayer` node in your scene.
2. In the Inspector, you'll see a new section with:
   - A dropdown menu listing all animations in that player.
   - A button "Clean Unused Animation Tracks".
3. Choose an animation from the dropdown.
4. Click the button – all tracks that target bones not found in the corresponding `Skeleton3D` will be removed.
5. Check the console output to see which tracks were deleted.

## Notes
- The plugin works with `Skeleton3D` nodes only (3D skeletons).
- Paths in animation tracks are resolved relative to the animation's root node (`AnimationPlayer.root_node`).

## License
MIT
