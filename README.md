sacm-xml-catalog
================

XML Catalog for SACM-related schemata.

About
-----

sacm-xml-catalog provides copies of XML Schema documents commonly used in 
SACM/[SCAP](http://scap.nist.gov/)
XML documents allowing these copies to be used in lieu of direct
network access to the "canonical" locations. These schema documents do not
change very often, and local copies obviate the need for network access
to the schema documents.

Copies of various versions of
[XCCDF](http://scap.nist.gov/specifications/xccdf/)
, 
[CPE](http://cpe.mitre.org/)
, 
[OVAL](http://oval.mitre.org/)
, 
and 
[OCIL](http://scap.nist.gov/specifications/ocil/)
schemata are provided.

Usage
-----

Usage requires an 
[XML Catalog](https://en.wikipedia.org/wiki/XML_Catalog) 
aware implementation, such as
[libxml](http://www.xmlsoft.org/catalog.html)
.

License
-------

Copyright © 2012 Gary Gapinski

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    <http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.