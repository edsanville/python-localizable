python-localizable
==================

Localizable.strings parser for Python

# Usage

Install using pip.

    $ pip install localizable
    
You can either parse a full string directly or pass a file path:

	import localizable
	
	strings = localizable.read(filename='Localizable.strings')
	strings = localizable.parse(content="content of .strings file") # this works too
	
The output format is an array of dictionaries, in order, with the following key/value pairs:

    /* Comment */
    "Key" = "Value";

 * `key`: "Key"
 * `value`: "Value"
 * `comment`: "Comment"

You can also write a stringset back out to a file:

	localizable.write(filename='Localizable.strings')
 
# License

GPLv2. Adapted from Transifex.