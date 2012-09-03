sacm-xml-catalog
================

XML Catalog for SACM-related schemata.

About
-----

sacm-xml-catalog provides copies of XML Schema documents commonly used in 
SACM/[SCAP](http://scap.nist.gov/)
XML documents allowing these copies to be used in lieu of direct
network access to the "canonical" locations. These schema documents change infrequently,
and local copies obviate the need for network access
to the schema documents.

Copies of various versions of
[XCCDF](http://scap.nist.gov/specifications/xccdf/), 
[CPE](http://cpe.mitre.org/), 
[OVAL](http://oval.mitre.org/), 
and 
[OCIL](http://scap.nist.gov/specifications/ocil/)
schemata are provided.

Usage
-----

Usage requires an 
[XML Catalog](https://en.wikipedia.org/wiki/XML_Catalog) 
aware implementation, such as
[libxml](http://www.xmlsoft.org/catalog.html).

XML documents can specify the URI of a related XML Schema document 
using the `xsi:schemaLocation` attribute, e.g.,
```xml
<Benchmark
    xmlns="http://checklists.nist.gov/xccdf/1.1"
    xmlns:cdf="http://checklists.nist.gov/xccdf/1.1"
    xmlns:cpe="http://cpe.mitre.org/dictionary/2.0"
    xmlns:cpel="http://cpe.mitre.org/language/2.0"
    xmlns:dc="http://purl.org/dc/elements/1.1/"
    xmlns:dsig="http://w3.org/2000/09/xmldsig#"
    xmlns:xhtml="http://www.w3.org/1999/xhtml"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    id="USGCB-RHEL-5-Desktop"
    xml:lang="en-US"
    xsi:schemaLocation="http://checklists.nist.gov/xccdf/1.1 http://nvd.nist.gov/schema/xccdf-1.1.4.xsd 
                        http://cpe.mitre.org/dictionary/2.0  http://cpe.mitre.org/files/cpe-dictionary_2.1.xsd
                        "
    style="SCAP_1.1"
    resolved="false">
```
sacm-xml-catalog allows the use of local copies of
`http://nvd.nist.gov/schema/xccdf-1.1.4.xsd`
and
`http://cpe.mitre.org/files/cpe-dictionary_2.1.xsd`
rather than ones obtained from those URIs. 

License
-------

Copyright © 2012 Gary Gapinski.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at <http://www.apache.org/licenses/LICENSE-2.0>.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.