webgl-perf
==========

GPU/webgl performance tester

TODO:

renderObjects calls renderBuffer for each object and calling it too often 
causes bottleneck in js->gl interface (mainly drawElements and setProgram).
Reorganize so that fewer objects are used.
Currently each box is distinct object.

References:
- http://threejs.org/
- http://soledadpenades.com/articles/three-js-tutorials/object-picking/


