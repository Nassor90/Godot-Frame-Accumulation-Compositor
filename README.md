# Godot Frame Accumulation Compositor

This CompositorEffect is a post transparent process effect that allows you to mix a copy of the current frame buffer into a persistent color buffer. This allows for the creation of frame accumulation-based fullscreen effects.

https://github.com/user-attachments/assets/09332969-f375-4f81-a11b-52807e3a8481

# Usage

In the accumulation_compositor.gd file set the SHADER_PATH const to the path of the provided glsl file. After that go to the Compositor on either your WorldEnvironment or Camera3D and add a new effect to the CompositorEffects array.

In the effect itself there is a blur_strength variable that will let you control how long it takes for the blur to fade. I personally found 0.75 to work pretty well but you may have to adjust based on your project.

If the AccumulationEffect does not appear you may have to restart your engine. 

# Installation

Add the provided .gd and .glsl files into your project.

# Known Issues

When the effect gets added to the compositor it will flash black for a frame and darken the image for a short while. This'll be fixed very soon.

If you use the enabled variable to enable and disable the compositor it'll accumulate a frame from before you disabled it which looks bad. I'll look into this ASAP.
