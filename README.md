"OSG on steroids"
=================

This fork was created to experiment with performance enhancements for [OpenMW](https://github.com/OpenMW/openmw) that are too controversial to be included in the general purpose OSG project - either for design reasons or backward compatibility reasons.

OpenMW still works with "vanilla" OpenSceneGraph, but it is recommended to use the fork for better performance (around 10-15% on most devices). Note that the improvements are very specific to OpenMW and its animation code in particular; other OpenSceneGraph applications are not likely to see the same speed-up, or any speed-up at all if they are already GPU limited.

The fork is currently based on the OpenSceneGraph-3.4 branch and will continue to be based on the latest stable branch of OSG at the time. 

A list of all changes can be viewed [here](https://github.com/openscenegraph/OpenSceneGraph/compare/OpenSceneGraph-3.4...OpenMW:master).

For planned changes: see https://github.com/scrawl/osg/issues

Please see "README.txt" for the original OpenSceneGraph read me and credits.
