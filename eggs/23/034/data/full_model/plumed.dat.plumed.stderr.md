**Project ID:** [plumID:23.034]({{ '/' | absolute_url }}eggs/23/034/)  
Stderr for source:  full_model/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
PairOrientationalEntropy.x5hKIQ.cpp: In constructor ‘PLMD::colvar::PairOrientationalEntropy::PairOrientationalEntropy(const PLMD::ActionOptions&)’:
PairOrientationalEntropy.x5hKIQ.cpp:193:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
193 |     for(unsigned int i=0;i<nhist_[0];i++) {
PairOrientationalEntropy.x5hKIQ.cpp:194:30: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
194 |        for(unsigned int j=0;j<nhist_[1];j++) {
PairOrientationalEntropy.x5hKIQ.cpp:252:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
252 |   for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.x5hKIQ.cpp:256:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
256 |   for(unsigned i=0;i<nhist_[1];++i){
PairOrientationalEntropy.x5hKIQ.cpp: In member function ‘virtual void PLMD::colvar::PairOrientationalEntropy::calculate()’:
PairOrientationalEntropy.x5hKIQ.cpp:511:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
511 |      for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.x5hKIQ.cpp:512:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
512 |         for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.x5hKIQ.cpp:523:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
523 |   for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.x5hKIQ.cpp:524:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
524 |      for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.x5hKIQ.cpp:562:25: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
562 |       for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.x5hKIQ.cpp:563:27: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
563 |         for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.x5hKIQ.cpp:581:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
581 |     for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.x5hKIQ.cpp:582:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
582 |        for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.x5hKIQ.cpp:593:23: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
593 |     for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.x5hKIQ.cpp:594:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
594 |        for(unsigned j=0;j<nhist_[1];++j){
PairOrientationalEntropy.x5hKIQ.cpp: In member function ‘double PLMD::colvar::PairOrientationalEntropy::integrate(PLMD::Matrix<double>, std::vector<double>) const’:
PairOrientationalEntropy.x5hKIQ.cpp:626:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
626 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:627:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
627 |      for(unsigned j=1;j<(nhist_[1]-1);++j){
|                       ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:632:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
632 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:636:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
636 |   for(unsigned j=1;j<(nhist_[1]-1);++j){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp: In member function ‘PLMD::Vector PLMD::colvar::PairOrientationalEntropy::integrate(PLMD::Matrix<PLMD::VectorGeneric<3> >, std::vector<double>) const’:
PairOrientationalEntropy.x5hKIQ.cpp:653:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
653 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:654:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
654 |      for(unsigned j=1;j<(nhist_[1]-1);++j){
|                       ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:659:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
659 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:663:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
663 |   for(unsigned j=1;j<(nhist_[1]-1);++j){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp: In member function ‘PLMD::Tensor PLMD::colvar::PairOrientationalEntropy::integrate(PLMD::Matrix<PLMD::TensorGeneric<3, 3> >, std::vector<double>) const’:
PairOrientationalEntropy.x5hKIQ.cpp:680:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
680 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:681:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
681 |      for(unsigned j=1;j<(nhist_[1]-1);++j){
|                       ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:686:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
686 |   for(unsigned i=1;i<(nhist_[0]-1);++i){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp:690:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
690 |   for(unsigned j=1;j<(nhist_[1]-1);++j){
|                    ~^~~~~~~~~~~~~~
PairOrientationalEntropy.x5hKIQ.cpp: In member function ‘void PLMD::colvar::PairOrientationalEntropy::outputGofr(PLMD::Matrix<double>, const char*)’:
PairOrientationalEntropy.x5hKIQ.cpp:705:21: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
705 |   for(unsigned i=0;i<nhist_[0];++i){
PairOrientationalEntropy.x5hKIQ.cpp:706:24: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} [-Wsign-compare]
706 |      for(unsigned j=0;j<nhist_[1];++j){
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
ManyAnglePlus.ifQ4yc.cpp: In constructor ‘PLMD::colvar::ManyAngle::ManyAngle(const PLMD::ActionOptions&)’:
ManyAnglePlus.ifQ4yc.cpp:67:27: warning: ‘PLMD::colvar::ManyAngle::moment2’ will be initialized after [-Wreorder]
67 |   bool pbc, serial, mean, moment2;
|                           ^~~~~~~
ManyAnglePlus.ifQ4yc.cpp:67:13: warning:   ‘bool PLMD::colvar::ManyAngle::serial’ [-Wreorder]
67 |   bool pbc, serial, mean, moment2;
|             ^~~~~~
ManyAnglePlus.ifQ4yc.cpp:99:1: warning:   when initialized here [-Wreorder]
99 | ManyAngle::ManyAngle(const ActionOptions&ao):
| ^~~~~~~~~
ManyAnglePlus.ifQ4yc.cpp:123:3: warning: this ‘if’ clause does not guard... [-Wmisleading-indentation]
123 |   if(mean) addComponentWithDerivatives("mean"); componentIsNotPeriodic("mean"); moments[0]=getPntrToComponent("mean"); // (Z)
|   ^~
ManyAnglePlus.ifQ4yc.cpp:123:49: note: ...this statement, but the latter is misleadingly indented as if it were guarded by the ‘if’
123 |   if(mean) addComponentWithDerivatives("mean"); componentIsNotPeriodic("mean"); moments[0]=getPntrToComponent("mean"); // (Z)
|                                                 ^~~~~~~~~~~~~~~~~~~~~~
ManyAnglePlus.ifQ4yc.cpp:124:3: warning: this ‘if’ clause does not guard... [-Wmisleading-indentation]
124 |   if(moment2) addComponentWithDerivatives("moment2"); componentIsNotPeriodic("moment2"); moments[1]=getPntrToComponent("moment2"); // (Z)
|   ^~
ManyAnglePlus.ifQ4yc.cpp:124:55: note: ...this statement, but the latter is misleadingly indented as if it were guarded by the ‘if’
124 |   if(moment2) addComponentWithDerivatives("moment2"); componentIsNotPeriodic("moment2"); moments[1]=getPntrToComponent("moment2"); // (Z)
|                                                       ^~~~~~~~~~~~~~~~~~~~~~
</pre>
{% endraw %}
