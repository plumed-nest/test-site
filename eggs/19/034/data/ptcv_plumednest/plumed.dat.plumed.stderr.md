**Project ID:** [plumID:19.034]({{ '/' | absolute_url }}eggs/19/034/)  
Stderr for source:  ptcv_plumednest/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
Proton.cpp: In constructor ‘PLMD::vatom::Proton::Proton(const PLMD::ActionOptions&)’:
Proton.cpp:158:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  158 |     for(unsigned i=0;i<no;i++) derivcn[i].resize(no+nh);
      |                      ~^~~
Proton.cpp:161:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  161 |     for(unsigned i=0;i<no;i++) derivw[i].resize(no);
      |                      ~^~~
Proton.cpp:171:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  171 |   for(unsigned i=0;i<no;i++) offset[i] = offsetdefault;
      |                    ~^~~
Proton.cpp: In member function ‘virtual void PLMD::vatom::Proton::calculate()’:
Proton.cpp:222:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  222 |   for(unsigned i=0;i<no;i++){
      |                    ~^~~
Proton.cpp:226:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  226 |     for(unsigned j=0;j<no+nh;j++){
      |                      ~^~~~~~
Proton.cpp:231:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  231 |     for(unsigned j=0;j<no;j++){
      |                      ~^~~
Proton.cpp:241:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  241 |   for(unsigned io=0;io<no;io++){
      |                     ~~^~~
Proton.cpp:243:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  243 |     for(unsigned ih=no;ih<nh+no;ih++){
      |                        ~~^~~~~~
Proton.cpp:267:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  267 |   for(unsigned iat=0;iat<no;iat++){
      |                      ~~~^~~
Proton.cpp:271:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  271 |   for(unsigned iat=0;iat<no;iat++) weight[iat] /= sum;
      |                      ~~~^~~
Proton.cpp:275:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  275 |   for(unsigned i=0;i<no;i++){
      |                    ~^~~
Proton.cpp:286:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  286 |     for(unsigned iat=0;iat<no;iat++){
      |                        ~~~^~~
Proton.cpp:296:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  296 |     for(unsigned iat=0;iat<no;iat++) weight[iat] /= sum;
      |                        ~~~^~~
Proton.cpp:301:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  301 |   for(unsigned i=0;i<no;i++){
      |                    ~^~~
Proton.cpp:302:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  302 |     for(unsigned j=0;j<no;j++){
      |                      ~^~~
Proton.cpp:313:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  313 |   for(unsigned i=0;i<no;i++){
      |                    ~^~~
Proton.cpp:320:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  320 |      for(unsigned j=0;j<no;j++){
      |                       ~^~~
Proton.cpp:321:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  321 |         for(unsigned l=0;l<no;l++){
      |                          ~^~~
Proton.cpp:331:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  331 |   for(unsigned j=0;j<no;j++){
      |                    ~^~~
Proton.cpp:332:10: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  332 |      if(j!=imax){
      |         ~^~~~~~
Proton.cpp:206:7: warning: unused variable ‘io’ [-Wunused-variable]
  206 |   int io, i;
      |       ^~
Proton.cpp:206:11: warning: unused variable ‘i’ [-Wunused-variable]
  206 |   int io, i;
      |           ^
PathCV.cpp: In destructor ‘virtual PLMD::function::PathCV::~PathCV()’:
PathCV.cpp:209:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  209 |   for(int i=0;i<mw_n_;++i){
      |               ~^~~~~~
PathCV.cpp: In constructor ‘PLMD::function::PathCV::PathCV(const PLMD::ActionOptions&)’:
PathCV.cpp:237:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  237 |   for(int i=0;i<mw_n_;++i){
      |               ~^~~~~~
PathCV.cpp:260:11: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  260 |       if(i==mw_id_) ifiles[i]->close();
      |          ~^~~~~~~~
PathCV.cpp: In member function ‘void PLMD::function::PathCV::generatePath()’:
PathCV.cpp:484:26: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  484 |     for(int inode=0;inode<nnodes;inode++){
      |                     ~~~~~^~~~~~~
PathCV.cpp: In member function ‘void PLMD::function::PathCV::readMultipleWalkers()’:
PathCV.cpp:942:16: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  942 |   for(int i=0;i<mw_n_;++i){
      |               ~^~~~~~
PathCV.cpp:943:9: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
  943 |     if(i==mw_id_) continue;
      |        ~^~~~~~~~
</pre>
{% endraw %}
