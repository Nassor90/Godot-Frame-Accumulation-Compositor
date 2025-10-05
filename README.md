# Godot-Frame-Accumulation-Compositor

This CompositorEffect is a post transparent process effect that allows you to mix a copy of the current frame buffer into a persistent color buffer. This allows for the creation of frame accumulation-based fullscreen effects.

# Usage

In the accumulation_compositor.gd file set the SHADER_PATH const to the path of the provided glsl file. After that go to the Compositor on either your WorldEnvironment or Camera3D and add a new effect to the CompositorEffects array.

In the effect itself there is a blur_strength variable that will let you control how long it takes for the blur to fade. I personally found 0.75 to work pretty well but you may have to adjust based on your project.

If the AccumulationEffect does not appear you may have to restart your engine. 

# Installation

Add the provided .gd and .glsl files into your project.
