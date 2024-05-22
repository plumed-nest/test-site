**Project ID:** [plumID:21.033]({{ '/' | absolute_url }}eggs/21/033/)  
Stderr for source:  inside_path/plumed.2.dat   
Download: [zipped raw stdout](plumed.2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../PathCV.cpp: In destructor ‘virtual PLMD::function::PathCV::~PathCV()’:
../PathCV.cpp:209:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
209 |   for(int i=0;i<mw_n_;++i){
|               ~^~~~~~
../PathCV.cpp: In constructor ‘PLMD::function::PathCV::PathCV(const PLMD::ActionOptions&)’:
../PathCV.cpp:237:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
237 |   for(int i=0;i<mw_n_;++i){
|               ~^~~~~~
../PathCV.cpp:260:11: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
260 |       if(i==mw_id_) ifiles[i]->close();
|          ~^~~~~~~~
../PathCV.cpp: In member function ‘void PLMD::function::PathCV::generatePath()’:
../PathCV.cpp:484:26: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
484 |     for(int inode=0;inode<nnodes;inode++){
|                     ~~~~~^~~~~~~
../PathCV.cpp: In member function ‘void PLMD::function::PathCV::readMultipleWalkers()’:
../PathCV.cpp:942:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
942 |   for(int i=0;i<mw_n_;++i){
|               ~^~~~~~
../PathCV.cpp:943:9: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
943 |     if(i==mw_id_) continue;
|        ~^~~~~~~~
</pre>
{% endraw %}
