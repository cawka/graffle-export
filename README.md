OmniGraffle export scripts
--------------------------

Created by David Faitelson <davidf@comlab.ox.ac.uk>
Modified by Douglas Creager <dougc@comlab.ox.ac.uk>
Modified by Alexander Afanasyev <alexander.afanasyev@ucla.edu>


This package provides command-line access to the export functionality
of OmniGraffle.  This allows you, for instance, to automatically
generate the necessary EPS and PDF versions of an OmniGraffle figure
for incorporating into an automatic build system for a LaTeX document.

The package consists of an AppleScript command-line tool (``graffle2pdf``)
that can be run to convert ``.graffle`` files into the desired EPS or PDF format.
  The tool is designed to work with OmniGraffle Professional
version, but ``graffle2pdf`` can be adapted to work with standard version
as well. 

The usage of the ``graffle2pdf`` tool:

    graffle2pdf <input file> <output file>

Both filenames are mandatory and the desired format is automatically guessed by 
OmniGraffle based on the output file extension and will fail if OmniGraffle fails
to detect the exported format.
If OmniGraffle cannot recognize the selected format (based on the extension), it
will simply save a copy of the input file into ``<output file>.graffle``.
