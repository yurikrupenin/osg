"OSG on steroids"
=================

A fork of OpenSceneGraph focused on speed, and less focused on accuracy & backwards compatibility.

This fork was created to experiment with performance enhancements for [OpenMW](https://github.com/OpenMW/openmw), that are too controversial to be included in the general purpose OSG project - either for design reasons or backward compatibility reasons.

OpenMW still works with "vanilla" OpenSceneGraph - but it will run at slightly lower framerate.

Current list of patches in this repository:

- Use single precision matrices & planes by default.
- Added option for single precision osg::Quat's (enabled by default). [Similar change rejected on osg-submissions.](http://forum.openscenegraph.org/viewtopic.php?t=12953)
- Nodes with invalid bounding sphere (which you get e.g. when creating a completely empty node) are interpreted as "always culled". This type of node is common in a bone hierarchy for skeletal animation, and culling them early helps performance. [Rejected on osg-submissions](http://forum.openscenegraph.org/viewtopic.php?t=15412).
- Removed several dynamic_cast's.
- (Occasionally:) Uncontroversial bug fixes that were proposed upstream but have not been merged yet.

Planned changes: see https://github.com/scrawl/osg/issues

Please see "README.txt" for the original OpenSceneGraph read me and credits.
