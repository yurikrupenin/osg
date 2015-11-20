"OSG on steroids"
=================

A fork of OpenSceneGraph focused on speed, and less focused on accuracy & backwards compatibility.

Current list of patches:

- Use single precision matrices & planes by default.
- Added option for single precision osg::Quat's (enabled by default). [Similar change rejected on osg-submissions.](http://forum.openscenegraph.org/viewtopic.php?t=12953)
- Nodes with invalid bounding sphere (which you get e.g. when creating a completely empty node) are interpreted as "always culled". This type of node is common in a bone hierarchy for skeletal animation, and culling them early helps performance. [Rejected on osg-submissions](http://forum.openscenegraph.org/viewtopic.php?t=15412).

Planned changes: see https://github.com/scrawl/osg/issues

Please see "README.txt" for the original OpenSceneGraph read me and credits.
