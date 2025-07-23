# webgl-perf GPU/webgl performance tester

## Usage or development

Suggested method is to clone repository and add directory in Chrome's Sources/Filesystem tab.

For view only download webgl-perf.html and open it with browser.

## References
- http://threejs.org/
- http://soledadpenades.com/articles/three-js-tutorials/object-picking/


# WebGPU
Add support for WebGPU and compare its performance to webgl.
Device is selected using  powerPreference: "high-performance" or "low-power" in navigator.gpu.requestAdapter https://webgpu.rocks/reference/enum/gpupowerpreference/

webgl-perf.html:302  The powerPreference option is currently ignored when calling requestAdapter() on Windows. See https://crbug.com/369219127
https://issues.chromium.org/issues/369219127?pli=1 

High-performance adapter can be selected using command line options or using Display settings
<img width="875" height="189" alt="image" src="https://github.com/user-attachments/assets/7572e037-79f6-4fde-8ece-c48a3fc86384" />


Compare to desktop implementation (wgpu)

## Configuration for usage with threejs
 - context is needed in parameter unless renderer.domElement.getContext( 'webgpu' ) is set

## References
- https://google.github.io/tour-of-wgsl/
- https://github.com/gfx-rs/wgpu
- https://github.com/google/dawn - Dawn is the native implementation of the WebGPU graphics API


