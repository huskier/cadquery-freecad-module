Changes
=======


v0.1
-----
    * Initial Version

v0.1.6
-----
    * Added STEP import and supporting tests

v0.1.7
-----
    * Added revolve operation and supporting tests
    * Fixed minor documentation errors

v0.1.8
-----
    * Added toFreecad() function as a convenience for val().wrapped
    * Converted all examples to use toFreecad()
    * Updated all version numbers that were missed before
    * Fixed import issues in Windows caused by fc_import
    * Added/fixed Mac OS support
    * Improved STEP import
    * Fixed bug in rotateAboutCenter that negated its effect on solids
    * Added Travis config (thanks @krasin)
    * Removed redundant workplane.py file left over from the PParts.com migration
    * Fixed toWorldCoordinates bug in moveTo (thanks @xix-xeaon)
    * Added new tests for 2D drawing functions
    * Integrated Coveralls.io, with a badge in README.md
    * Integrated version badge in README.md
    
v0.2.0
-----
   * Fixed versioning to match the semantic versioning scheme
   * Added license badge in changes.md
   * Fixed Solid.makeSphere implementation
   * Added CQ.sphere operation that mirrors CQ.box
   * Updated copyright dates
   * Cleaned up spelling and misc errors in docstrings
   * Fixed FreeCAD import error on Arch Linux (thanks @moeb)
   * Made FreeCAD import report import error instead of silently failing (thanks @moeb)
   * Added ruled option for the loft operation (thanks @hyOzd)
   * Fixed close() not working in planes other than XY (thanks @hyOzd)
   * Added box selector with bounding box option (thanks @hyOzd)
   * CQ.translate and CQ.rotate documentation fixes (thanks @hyOzd)
   * Fixed centering of a sphere
   * Increased test coverage
   * Added a clean function to keep some operations from failing on solids that need simplified (thanks @hyOzd)
   * Added a mention of the new Google Group to the readme
   
v0.3.0 (Unreleased)
-----
   * Fixed a bug where clean() could not be called on appropriate objects other than solids (thanks @hyOzd) #108
   * Implemented new selectors that allow existing selectors to be combined with arithmetic/boolean operations (thanks @hyOzd) #110
   * Fixed a bug where only 1 random edge was returned with multiple min/max selector matches (thanks @hyOzd) #111
   * Implemented the creation of a workplane from multiple co-planar faces (thanks @hyOzd) #113
   * Fixed the operation of Center() when called on a compound with multiple solids
   * Add the named planes ZX YX ZY to define different normals (thanks @galou) #115
   * Code cleanup in accordance with PEP 8 (thanks @galou)
   * Fixed a bug with the close function not resetting the first point of the context correctly (thanks @huskier)
   * Fixed the findSolid function so that it handles compounds #107
   * Changed the polyline function so that it adds edges to the stack instead of a wire #102
   * Add the ability to find the center of the bounding box, rather than the center of mass (thanks @huskier)
