generate a Multiple Picture Object files (.MPO) 3D picture from two jpeg files.

This is a Lua fork of https://github.com/odrevet/Multi-Picture-Object

This software implement in Lua the CIPA's MPO official reference document
available at the following URL: http://www.cipa.jp/std/documents/download_e.html?DC-007_E


Nintendo 3DS Users can see the generated test 3D file here
on github by clicking the out.mpo file then "View Raw".

# Code comment and annotations

The code is documented and annoted with the chapter and paragraph references to the CIPA manual.

The adresses where the data will be written in the file created with the sample left.jpg and right.jpg are annoted in the comments.
(e.g @0x42). Theses values may be differant with another input files.

# Usage

## Command line

This Lua script can be used with a Command Line Interface by calling mpojoin.lua: 

* Command line arguments:

<pre>
	LEFTFILENAME : left jpg file (mandatory argument)
	RIGHTFILENAME : right jpg file (mandatory argument)
	OUTFILENAME : output mpo file (mandatory argument)
</pre>

* example :

```
 mpojoin.lua left.jpg right.jpg  out.mpo
```

# Testing
The original developer of the PHP version tested the out.mpo for
correctness. This Lua version produces the same out.mpo.

# 3DS limitations

The New 3DS can not read 3D pictures with a width superior at 800px.
