"OSG on steroids"
=================

A fork of OpenSceneGraph focused on performance, and less concerned with accuracy & backwards compatibility.

This fork was created to experiment with performance enhancements for [OpenMW](https://github.com/OpenMW/openmw) that are too controversial to be included in the general purpose OSG project - either for design reasons or backward compatibility reasons.

OpenMW still works with "vanilla" OpenSceneGraph, but it is recommended to use the fork for better performance (around 10-15% on most devices). Occasionally, we will also apply OpenMW-relevant bug fixes that have not made it into a released version of OSG yet.

The fork is currently based on the OpenSceneGraph-3.4 branch and will continue to be based on the latest stable branch of OSG at the time. 

A list of all changes can be viewed [here](https://github.com/openscenegraph/OpenSceneGraph/compare/OpenSceneGraph-3.4...OpenMW:master).

For planned changes: see https://github.com/scrawl/osg/issues

Please see "README.txt" for the original OpenSceneGraph read me and credits.
