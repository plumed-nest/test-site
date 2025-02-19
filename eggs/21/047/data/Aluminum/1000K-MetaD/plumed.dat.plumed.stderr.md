**Project ID:** [plumID:21.047]({{ '/' | absolute_url }}eggs/21/047/)  
Stderr for source:  Aluminum/1000K-MetaD/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../PairEntropy.0RGJmp.cpp: In member function ‘virtual void PLMD::colvar::PairEntropy::calculate()’:
../../PairEntropy.0RGJmp.cpp:264:21: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
264 |          if (minBin > (nhist-1)) minBin=nhist-1;
|              ~~~~~~~^~~~~~~~~~~
../../PairEntropy.0RGJmp.cpp:266:21: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
266 |          if (maxBin > (nhist-1)) maxBin=nhist-1;
|              ~~~~~~~^~~~~~~~~~~
</pre>
{% endraw %}
