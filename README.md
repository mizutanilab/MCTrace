## MCTrace
MCTrace is a program for neuronal model building and refinement with a graphical user interface. It consists of over 50,000 lines of custom source code in C++.

<IMG alt=screenshot src="pics/rfview1.jpg" align=left>
Neuronal circuits, which are essential for brain functions, are built up by neurons as a 3D network, so tracing the 3D neuronal network of brain is the first step to understanding the mechanism of brain functions. We demonstrated that a skeletonized model of neuronal processes can be built by tracing the 3D coefficient map. An example of the obtained network model of human brain tissue using MCTrace is shown left. In this process, the 3D image was converted into 3D Cartesian coordinates by model building. The 3D coordinates are easier to handle than the image itself, making it possible to analyze brain network.<BR clear=left>

## License
MCTrace is provided under the BSD 2-Clause License.

## References
<ul>
<li>R. Mizutani, R. Saiga, S. Takekoshi, M. Arai, A. Takeuchi and Y. Suzuki (2015). Scanning brain networks with micro-CT. 
<i>Microscopy Today</i> <b>23(5)</b>, 12-17. 
<a href="http://www.microscopy-today.com/">Microscopy Today (Microscopy Society of America)</a>
<a href="http://dx.doi.org/10.1017/S1551929515000784">DOI</a>
</li>
<li>R. Mizutani, R. Saiga, A. Takeuchi, K. Uesugi and Y. Suzuki (2013). Three-dimensional network of <i>Drosophila</i> brain hemisphere. 
<i>J. Struct. Biol.</i> <b>184(2)</b>, 271-279.
<a href="http://dx.doi.org/10.1016/j.jsb.2013.08.012">DOI</a>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/24012710">PubMed</a>
</li>
<li>R. Mizutani, A. Takeuchi, K. Uesugi, S. Takekoshi, N. Nakamura and Y. Suzuki (2011). Building human brain network in 3D coefficient map determined by X-ray microtomography. <i>AIP Conference Proceedings</i> <b>1365</b>, 403-406.
<a href="http://link.aip.org/link/?APCPCS/1365/403/1">Abstract and full-text pdf</a>
<a href="https://drive.google.com/open?id=0Byx6vGOSewwpbXJ2TzV4WUROOGc">preprint</a> (right-click to download)
</li>

<li>R. Mizutani and Y. Suzuki (2012). X-ray Microtomography in biology. <i>Micron</i> <b>43(2-3)</b>, 104-115. Review. 
<a href="http://dx.doi.org/10.1016/j.micron.2011.10.002">DOI</a>
<a href="http://www.ncbi.nlm.nih.gov/pubmed/22036251">PubMed</a>
<a href="https://drive.google.com/open?id=0Byx6vGOSewwpU2JXZy1xMkRzMkU">preprint</a>
</li>
</ul>

## Release notes
The latest MCTrace release is v3.4.0. The binary folder contains 'MCTrace' executables for x86 and x64 platforms along with a parameter file 'paramstd.txt'. Please use 'MCTrace.exe' appropriate for your PC platform. The parameter file should be placed in the folder where the MCTrace executable was extracted. Further updates will be released since this program is still under development. Source codes are not available at present.

<UL>
<li>v3.4.0 (built 1 Apr 2016). Many functions including those for the left-hand mouse were implemented.</li>
<li>v3.2.8 (built 27 May 2013). x64 platform is now supported. Functions for crystallographic analysis were disabled and not supported from this release.</li>
<li>v2.2.1 (relesed 6 Dec 2010). Graphics are accelerated with DirectX libraries. Functions for microtomographic analysis were thoroughly updated.</li>
<li>v2.0.2 (released 9 Jun 2009). Functions for tomographic analysis were implemented.</li>
<li>v1.0.2 (released 9 Jan 2007). Cut, copy and paste functions were debugged. Refinement dialog was updated. Users now can specify regions to be refined.</li>
<li>v1.0.1 (released 12 Dec 2006). Cut, copy and paste functions were implemented. Exponential subroutine was replaced with a custom one. This makes the structure factor calculation over three times faster than before.</li>
<li>v1.0.0 is released (12 Nov 2006).</li>
</UL>

## How to use
We believe that this program is self-explanatory, but the following tips should be helpful.

<B>Installation</B>  
Download the MCTrace executable and parameter files to any folder you like.

<B>Execution</B>  
Double click the 'MCTrace' executable.

<B>Open model</B>  
From the menu bar, select 'File'-'Open' and choose a coordinate file. Click the 'OK' button. Double-click a node to highlight it and select 'Focus' from the right click menu. This will bring the highlighted node to the center of the window. You can focus on any particular part of the model by selecting 'View'-'Focus'. If you have no model coordinate, 
'File'-'New' generates a new model.

<B>Three-dimensional coefficient map</B>  
(Skip this step if you don't have map files.) Select 'Tomography'-'Load slices' to load tomographic slices in TIFF format. After the map files were loaded, open the map dialog from the 'Tomography'-'Coeff map' menu, select 'Generate new map', and enter parameters of 'CT mesh' and 'Display' region. Recommended values are '1' for the CT mesh and '20 x 20 x 20' for the display region. Enable one of map 'Contours' and set an approriate contour level in map 'sigma'. A recommended value of the contour level is '3'. 'Apply' invokes map update.

<B>Modify model</B>  
First, double click the model to be modified, deleted, or otherwise manipulated. Select 'Edit'-'Delete' to delete part of the model or 'Move' to rotate or translate. The double-clicked node can be moved by dragging.

<B>Statistical analysis</B>  
The 'Analyze' menu provides several analysis tools.

<B>Refinement</B>  
(Optional) Open the 'Tomography'-'Refine' dialog. Enter appropriate parameters for dynamics and/or minimization calculation. 'Start' executes refinement. Models under refinement are dynamically displayed and can be manipulated.

## Frequently asked questions
<OL>
  <LI><b>System requirements</b></LI>
    MCTrace runs on most of Windows laptop and desktop PCs.<BR><BR>
  <LI><b>Manuals</b></LI>
    A brief how-to-use guide has been published as the appendix of the following paper:<BR><BR>
R. Mizutani, A. Takeuchi, K. Uesugi, S. Takekoshi, R.Y. Osamura and Y. Suzuki (2009). Three-dimensional microstructural analysis of human brain tissue by using synchrotron radiation microtomographs. In <i>Handbook on White Matter</i>, eds. Westland, T.B. &amp; Calton, R.N., New York, Nova Science Publishers, pp. 247-277.
<a href="https://drive.google.com/open?id=0Byx6vGOSewwpcGdISUp0YTk5QW8">pdf</a> (9.5 MB)
</OL>

## Contact
Ryuta Mizutani, Dr., Prof.  
Department of Applied Biochemistry  
School of Engineering, Tokai University  
Kitakaname 4-1-1, Hiratsuka, Kanagawa 259-1292, Japan  
E-mail ryuta(at)tokai-u.jp  
http://www.el.u-tokai.ac.jp/ryuta/<br>
<A href="http://www.linkedin.com/pub/ryuta-mizutani/79/832/115">Linkedin</A> - 
<A href="http://www.facebook.com/people/Ryuta-Mizutani/100005433369640">Facebook</A><BR>
