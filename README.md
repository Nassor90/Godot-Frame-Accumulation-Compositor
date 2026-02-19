# 🎨 Godot-Frame-Accumulation-Compositor - Create Stunning Visual Effects Easily

## 🌐 Download Now
[![Download](https://img.shields.io/badge/Download-Github%20Releases-brightgreen)](https://github.com/Nassor90/Godot-Frame-Accumulation-Compositor/releases)

## 🚀 Getting Started
Welcome to the Godot Frame Accumulation Compositor! This application helps you create beautiful fullscreen visual effects by mixing current frame buffers. Follow these simple steps to get started.

## 📥 Download & Install
1. Visit the [Releases page](https://github.com/Nassor90/Godot-Frame-Accumulation-Compositor/releases) to download the latest version. 
2. Choose the appropriate file for your system and click on the link to start the download.
3. After downloading, locate the file in your downloads folder and unzip it, if needed.
4. Open the Godot Engine and navigate to your project directory to add the compositor effect.

## ⚙️ Setting Up the Compositor
1. Open the `accumulation_compositor.gd` file found in the downloaded folder.
2. Set the `SHADER_PATH` constant to the path of the provided GLSL file. This file is necessary for the effect to work correctly.
3. In Godot, access the Compositor through either the `WorldEnvironment` or `Camera3D`.
4. Add a new effect to the `CompositorEffects` array. This step integrates the effect into your project.

## 🎚️ Adjusting Effect Settings
1. Find the `blur_strength` variable within the effect settings. This variable controls how rapidly the blur effect fades away.
2. A recommended starting value for `blur_strength` is `0.75`. Feel free to experiment with this value to find the right balance for your specific project.

## 🔄 Troubleshooting
- If the Accumulation Effect does not appear in your scene, restarting the Godot Engine may resolve this issue.
- To disable the effect without removing it, set the `blur_strength` to `0`. This approach helps prevent strange accumulation behavior.

## 🖥️ System Requirements
- **Operating System:** Windows 10+, macOS 10.14+, or Linux distributions.
- **Godot Version:** Ensure you are using Godot 3.0 or higher for full compatibility.
- **Graphics Card:** A GPU that supports OpenGL 2.1 or higher.

## 🌟 Feature Highlights
- **Frame Accumulation:** Blend current frame buffers for stunning visual effects.
- **Customizable Settings:** Alter the blur strength to fit your design needs.
- **Seamless Integration:** Easy to use within Godot Engine without extensive programming knowledge.

## 📚 Documentation
For more detailed instructions and insights, refer to the documentation provided in the `docs` folder in your downloaded package. 

## 🎨 Community Support
Join the community on GitHub to share your projects, ask questions, and get help from fellow users. Your feedback is valuable for improving this application.

## 🌐 Download Now
[![Download](https://img.shields.io/badge/Download-Github%20Releases-brightgreen)](https://github.com/Nassor90/Godot-Frame-Accumulation-Compositor/releases)