# Godot SSR Water
(c) Marcel Bankmann 2023 - present

![Demo Scene Screenshot](screenshot.png)

## What is this about?

This intends to solve the problem that the SSR (Screen Space Reflection) implementation of Godot 4.1 is limited to surfaces that are not transparent. For a water shader it is often necessary to support both transparency and reflections. In a lot of cases this can be worked around with reflection probes, but the need for SSR stands, especially because SSR works quiet well for water. The only solution is to write a custom SSR shader for that matter.

This is a full water shader implementation supporting:

- Screen Space Reflection
- Transparency
- 3D waves
- Edge detection
- Normal textures for a varied surface
- Fake Refraction

This respository includes the shader and a demo scene.

The SSR part of the shader is done in a function of its own, so it should be possible to use the SSR functionality separately.

## Usage

Load the project in Godot 4.1 (or possibly later) and hit "Run".

Use the shader settings to both change look and performance of the shader. 

Especially the SSR settings have great impact on the shaders performance. In many cases low quality settings might be more than enough (low value distance, high value resolution).

