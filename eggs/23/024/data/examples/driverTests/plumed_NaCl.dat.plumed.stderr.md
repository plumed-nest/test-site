**Project ID:** [plumID:23.024]({{ '/' | absolute_url }}eggs/23/024/)  
Stderr for source:  examples/driverTests/plumed_NaCl.dat   
Download: [zipped raw stdout](plumed_NaCl.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_NaCl.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../src/pines/PINES.cpp: In constructor ‘PLMD::PINES::PINES::PINES(const PLMD::ActionOptions&)’:
../../src/pines/PINES.cpp:379:14: warning: comparison of integer expressions of different signedness: ‘int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<unsigned int>, unsigned int>::value_type’ {aka ‘unsigned int’} [-Wsign-compare]
379 |       if(rind==Presind[j]) {
../../src/pines/PINES.cpp:416:11: warning: unused variable ‘rind’ [-Wunused-variable]
416 |       int rind=mypdb.getResidueNumber(anum);
|           ^~~~
../../src/pines/PINES.cpp:1012:21: warning: comparison of integer expressions of different signedness: ‘int’ and ‘std::vector<std::vector<PLMD::VectorGeneric<3> > >::size_type’ {aka ‘long unsigned int’} [-Wsign-compare]
1012 |   for (int i = 0; i < ann_deriv.size(); i++) {
|                   ~~^~~~~~~~~~~~~~~~~~
../../src/pines/PINES.cpp: In member function ‘virtual void PLMD::PINES::PINES::prepare()’:
../../src/pines/PINES.cpp:1090:11: warning: unused variable ‘buffer’ [-Wunused-variable]
1090 |       int buffer=10;
|           ^~~~~~
../../src/pines/PINES.cpp: In member function ‘virtual void PLMD::PINES::PINES::calculate()’:
../../src/pines/PINES.cpp:1512:27: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
1512 |               if(sb_count > max_solv_atoms) {
|                  ~~~~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.cpp:1567:34: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
1567 |           if(nl_small[j]->size() >= max_solv_atoms) {
|              ~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~
../../src/pines/PINES.cpp:1575:44: warning: comparison of integer expressions of different signedness: ‘std::vector<int>::size_type’ {aka ‘long unsigned int’} and ‘int’ [-Wsign-compare]
1575 |                 if(sb_count - A0[i].size() < max_solv_atoms) {
|                    ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.cpp:1656:34: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
1656 |               for(unsigned m=0; m<OrdVecAll[i+l*Nprec]; m++) {
../../src/pines/PINES.cpp:1668:32: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
1668 |             for(unsigned m=0; m<OrdVec[i]; m++) {
../../src/pines/PINES.cpp:1723:18: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
1723 |         if(limit > max_solv_atoms) {
|            ~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.cpp:1704:10: warning: unused variable ‘dosorting’ [-Wunused-variable]
1704 |     bool dosorting=dosort[j];
|          ^~~~~~~~~
../../src/pines/PINES.cpp:1801:18: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
1801 |         if(limit > max_solv_atoms) {
|            ~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.cpp:1826:16: warning: unused variable ‘tPINES’ [-Wunused-variable]
1826 |         double tPINES = sfs[j].calculate(dm*Fvol, dfunc);
|                ^~~~~~
../../src/pines/PINES.cpp:1902:18: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
1902 |       if( (limit > max_solv_atoms) && (solv_blocks != 0) ){
|            ~~~~~~^~~~~~~~~~~~~~~~
../../src/pines/PINES.cpp:1771:8: warning: unused variable ‘Nder’ [-Wunused-variable]
1771 |   bool Nder=CompDer;
|        ^~~~
../../src/pines/PINES.cpp:1772:8: warning: unused variable ‘Scalevol’ [-Wunused-variable]
1772 |   bool Scalevol=Svol;
|        ^~~~~~~~
../../src/pines/PINES.cpp: In constructor ‘PLMD::PINES::PINES::PINES(const PLMD::ActionOptions&)’:
../../src/pines/PINES.cpp:465:46: warning: ‘oind’ may be used uninitialized in this function [-Wmaybe-uninitialized]
465 |     gname=mypdb.getAtomName(comatm[Pind0[oind]-1][0]);
|                                              ^
../../src/pines/PINES.cpp: In constructor ‘PLMD::PINES::PINES::PINES(const PLMD::ActionOptions&)’:
../../src/pines/PINES.cpp:465:46: warning: ‘oind’ may be used uninitialized in this function [-Wmaybe-uninitialized]
465 |     gname=mypdb.getAtomName(comatm[Pind0[oind]-1][0]);
|                                              ^
../../src/annbfunc/ANNB.cpp:487:94: warning: backslash and newline separated by space
487 |               derivatives_of_each_layer[jj + 1][kk] += derivatives_of_each_layer[jj + 1][kk] \
|
../../src/annbfunc/ANNB.cpp: In constructor ‘PLMD::function::annfunc::ANNB::ANNB(const PLMD::ActionOptions&)’:
../../src/annbfunc/ANNB.cpp:221:29: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
221 |   if(getNumberOfArguments() != num_nodes[0]) {
../../src/annbfunc/ANNB.cpp:236:25: warning: comparison of integer expressions of different signedness: ‘int’ and ‘std::vector<double>::size_type’ {aka ‘long unsigned int’} [-Wsign-compare]
236 |     for (int jj = 0; jj < temp_coeff[ii].size(); jj ++) {
|                      ~~~^~~~~~~~~~~~~~~~~~~~~~~
../../src/annbfunc/ANNB.cpp: In member function ‘void PLMD::function::annfunc::ANNB::calculate_output_of_each_layer(const std::vector<double>&)’:
../../src/annbfunc/ANNB.cpp:324:22: warning: comparison of integer expressions of different signedness: ‘int’ and ‘std::vector<int>::size_type’ {aka ‘long unsigned int’} [-Wsign-compare]
324 |   for(int ii = 1; ii < num_nodes.size(); ii ++) {
|                   ~~~^~~~~~~~~~~~~~~~~~
</pre>
{% endraw %}
