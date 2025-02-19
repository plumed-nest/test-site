**Project ID:** [plumID:22.039]({{ '/' | absolute_url }}eggs/22/039/)  
Stderr for source:  glycine_plumed.dat   
Download: [zipped raw stdout](glycine_plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](glycine_plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
PairOrientationalEntropy.Ni94rN.cpp: In constructor ‘PLMD::colvar::PairOrientationalEntropy::PairOrientationalEntropy(const PLMD::ActionOptions&)’:
PairOrientationalEntropy.Ni94rN.cpp:193:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
193 |     for(unsigned int i=0;i<nhist_[0];i++) {
PairOrientationalEntropy.Ni94rN.cpp:194:30: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
194 |        for(unsigned int j=0;j<nhist_[1];j++) {
PairOrientationalEntropy.Ni94rN.cpp:252:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
252 |   for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.Ni94rN.cpp:256:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
256 |   for(unsigned i=0;i<nhist_[1];++i){
PairOrientationalEntropy.Ni94rN.cpp: In member function ‘virtual void PLMD::colvar::PairOrientationalEntropy::calculate()’:
PairOrientationalEntropy.Ni94rN.cpp:511:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
511 |      for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.Ni94rN.cpp:512:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
512 |         for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.Ni94rN.cpp:523:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
523 |   for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.Ni94rN.cpp:524:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
524 |      for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.Ni94rN.cpp:562:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
562 |       for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.Ni94rN.cpp:563:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
563 |         for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.Ni94rN.cpp:581:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
581 |     for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.Ni94rN.cpp:582:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
582 |        for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.Ni94rN.cpp:593:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
593 |     for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.Ni94rN.cpp:594:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
594 |        for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.Ni94rN.cpp: In member function ‘double PLMD::colvar::PairOrientationalEntropy::integrate(PLMD::Matrix<double>, std::vector<double>) const’:
PairOrientationalEntropy.Ni94rN.cpp:626:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
626 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:627:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
627 |      for(unsigned j=1;j<(nhist_[1]-1);++j){
|                       ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:632:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
632 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:636:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
636 |   for(unsigned j=1;j<(nhist_[1]-1);++j){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp: In member function ‘PLMD::Vector PLMD::colvar::PairOrientationalEntropy::integrate(PLMD::Matrix<PLMD::VectorGeneric<3> >, std::vector<double>) const’:
PairOrientationalEntropy.Ni94rN.cpp:653:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
653 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:654:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
654 |      for(unsigned j=1;j<(nhist_[1]-1);++j){
|                       ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:659:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
659 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:663:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
663 |   for(unsigned j=1;j<(nhist_[1]-1);++j){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp: In member function ‘PLMD::Tensor PLMD::colvar::PairOrientationalEntropy::integrate(PLMD::Matrix<PLMD::TensorGeneric<3, 3> >, std::vector<double>) const’:
PairOrientationalEntropy.Ni94rN.cpp:680:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
680 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:681:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
681 |      for(unsigned j=1;j<(nhist_[1]-1);++j){
|                       ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:686:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
686 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp:690:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
690 |   for(unsigned j=1;j<(nhist_[1]-1);++j){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.Ni94rN.cpp: In member function ‘void PLMD::colvar::PairOrientationalEntropy::outputGofr(PLMD::Matrix<double>, const char*)’:
PairOrientationalEntropy.Ni94rN.cpp:705:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
705 |   for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.Ni94rN.cpp:706:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
706 |      for(unsigned j=0;j<nhist_[1];++j){
</pre>
{% endraw %}
