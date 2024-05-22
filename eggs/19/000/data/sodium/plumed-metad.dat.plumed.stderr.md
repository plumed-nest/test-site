**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
Stderr for source:  sodium/plumed-metad.dat   
Download: [zipped raw stdout](plumed-metad.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-metad.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
DebyeStructureFactor.cpp: In member function ‘virtual void PLMD::colvar::DebyeStructureFactor::calculate()’:
DebyeStructureFactor.cpp:489:43: warning: ‘prev_sin’ may be used uninitialized in this function [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                                   ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.cpp:489:25: warning: ‘prev_cos’ may be used uninitialized in this function [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                 ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.cpp:489:43: warning: ‘base_sin’ may be used uninitialized in this function [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                                   ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.cpp:489:25: warning: ‘base_cos’ may be used uninitialized in this function [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                 ~~~~~~~~^~~~~~~~~
</pre>
{% endraw %}
