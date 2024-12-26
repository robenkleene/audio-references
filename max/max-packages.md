# Max Packages

For this to work, an ancestor directory has to be included in `Options > File Preferences...`.

Folders with `*` are automatically included in the search path:

```
* clippings
Patchers to list in the "Paste From..." contextual menu when patching

* code
Gen patchers

collections
Collections to list in the File Browser that are associated with the package

default-definitions
Definition info for Object Defaults support in UI externals

default-settings
Saved color schemes for Object Defaults

* devices
Max for Live devices (AMXDs)

* docs
Reference pages and Vignettes to be accessible from the Documentation Window

* examples
Example patchers and supporting material

* extensions
Special external objects loaded on Max launch

* externals
External objects

* extras
Patchers to be listed in the "Extras" menu

* fonts
Custom fonts available to Max when the Package is present

* help
Help patchers and supporting material


  icon.png


A PNG graphic file (500x500px) for display in the
Package Manager


init
Text files interpreted by Max at launch

interfaces
Supporting files for objects to display in the top patcher toolbar and other Max integration.

* java-classes
Compiled Java classes for use in mxj/mxj~. Place .jar folders in a 'lib' subfolder.

java-doc
Documentation for Java classes

* javascript
Javascript files to be used by js

* jsextensions
Extensions to JS implemented as special externals or js files

* jsui
Javascript files to be used by jsui, and listed in the contextual menu for jsui


  
    license.txt
  
  or
  
    license.md
  


Terms of use / redistribution of your package (plain text or
Markdown
permitted)


* media
Media files to be included in the searchpath

* misc
Anything

* patchers
Patchers or abstractions to be included in the searchpath

* projects
Projects to be included in the searchpath. Note that only the project file will be added to the searchpath.

* object-icons
An SVG-format object icon for a particular Max object (named <objectname>.svg), used in the Object Browser

object-prototypes
Object Prototypes will be listed in the context menu for a selected UI object


  
    readme.txt
  
  or
  
    readme.md
  


Information about your package (plain text or
Markdown
permitted)


snippets
Snippets associated with this package

source
Source code for external objects, ignored by Max

support
Special location for DLL or dylib dependencies of external objects. Added to the DLL search path on Windows.

templates
Patchers to be listed in the "File > New From Template" menu
```
