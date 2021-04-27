**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
Stderr for source:  sodium/plumed-metad.dat   
(download [zipped raw stdout](plumed-metad.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
DebyeStructureFactor.cpp: In member function ‘virtual void PLMD::colvar::DebyeStructureFactor::calculate()’:
DebyeStructureFactor.cpp:490:25: warning: ‘prev_sin’ may be used uninitialized in this function [-Wmaybe-uninitialized]
  490 |           sinQR=base_cos*prev_sin+base_sin*prev_cos;
      |                 ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.cpp:489:25: warning: ‘prev_cos’ may be used uninitialized in this function [-Wmaybe-uninitialized]
  489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
      |                 ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.cpp:489:43: warning: ‘base_sin’ may be used uninitialized in this function [-Wmaybe-uninitialized]
  489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
      |                                   ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.cpp:490:25: warning: ‘base_cos’ may be used uninitialized in this function [-Wmaybe-uninitialized]
  490 |           sinQR=base_cos*prev_sin+base_sin*prev_cos;
      |                 ~~~~~~~~^~~~~~~~~
</pre>
{% endraw %}
