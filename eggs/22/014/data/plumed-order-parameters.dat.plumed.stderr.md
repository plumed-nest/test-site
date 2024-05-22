**Project ID:** [plumID:22.014]({{ '/' | absolute_url }}eggs/22/014/)  
Stderr for source:  plumed-order-parameters.dat   
Download: [zipped raw stdout](plumed-order-parameters.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-order-parameters.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
PairEntropies.cpp: In member function ‘virtual double PLMD::multicolvar::PairEntropies::compute(const unsigned int&, PLMD::multicolvar::AtomValuePack&) const’:
PairEntropies.cpp:288:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
288 |            if (minBin > (nhist-1)) minBin=nhist-1;
|                ~~~~~~~^~~~~~~~~~~
PairEntropies.cpp:290:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
290 |            if (maxBin > (nhist-1)) maxBin=nhist-1;
|                ~~~~~~~^~~~~~~~~~~
</pre>
{% endraw %}
