# Godot Frame Accumulation Compositor

This CompositorEffect is a post transparent process effect that allows you to mix a copy of the current frame buffer into a persistent color buffer. This allows for the creation of frame accumulation-based fullscreen effects.

https://github.com/user-attachments/assets/09332969-f375-4f81-a11b-52807e3a8481

# Usage

In the accumulation_compositor.gd file set the SHADER_PATH const to the path of the provided glsl file. After that go to the Compositor on either your WorldEnvironment or Camera3D and add a new effect to the CompositorEffects array.

In the effect itself there is a blur_strength variable that will let you control how long it takes for the blur to fade. I personally found 0.75 to work pretty well but you may have to adjust based on your project.

If the AccumulationEffect does not appear you may have to restart your engine. 

To disable it I recommend setting the blur_strength to 0 rather than disabling the effect itself to prevent strange accumulation issues when restarting it.

# Installation

Add the provided .gd and .glsl files into your project.

# Known Issues

When the effect gets added to the compositor it will flash black for a frame and darken the image for a couple frames. This is quite apparent in editor but in game it shouldn't be too obvious and can be worked around by setting the effect when loading into a scene and having the blur strength at 0.
