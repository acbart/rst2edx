General strategy so far:
------------------------

Create a custom builder for Sphinx that outputs XML from the RST files. 

Taking notes from:

https://github.com/lehmannro/sphinx-mirror/blob/master/sphinx/builders/xml.py
https://github.com/coot/sphinx_latex/blob/master/clatex_builder.py#L210
https://github.com/lehmannro/sphinx-mirror/blob/0c07cf9487e02d18c4da720888d36f5ff4f233ad/sphinx/ext/coverage.py


Builder API Documentation:
    http://sphinx-doc.org/latest/extdev/builderapi.html#sphinx.builders.Builder
    
Notes:
------

The main extension (source/ext/rst2edx.py) is where the meat of this application is.

If you're running from the make files, I've only added the 'edx' target to the windows one.