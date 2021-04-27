**Project ID:** [plumID:20.015]({{ '/' | absolute_url }}eggs/20/015/)  
Stderr for source:  EMMI-ASCT2/2-EMMI/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
EMMIVox.cpp: In member function ‘void PLMD::isdb::EMMIVOX::write_model_overlap(long int)’:
EMMIVox.cpp:535:17: warning: comparison of integer expressions of different signedness: ‘int’ and ‘std::vector<double>::size_type’ {aka ‘long unsigned int’} [-Wsign-compare]
  535 |   for(int i=0; i<ovmd_.size(); ++i) {
      |                ~^~~~~~~~~~~~~
EMMIVox.cpp: In member function ‘std::vector<double> PLMD::isdb::EMMIVOX::read_exp_errors(std::string)’:
EMMIVox.cpp:669:26: warning: comparison of integer expressions of different signedness: ‘unsigned int’ and ‘int’ [-Wsign-compare]
  669 |       for(unsigned i=0; i<nexp; ++i) {
      |                         ~^~~~~
EMMIVox.cpp: In member function ‘void PLMD::isdb::EMMIVOX::get_exp_data(std::string)’:
EMMIVox.cpp:800:22: warning: comparison of integer expressions of different signedness: ‘__gnu_cxx::__alloc_traits<std::allocator<int>, int>::value_type’ {aka ‘int’} and ‘std::vector<std::vector<int> >::size_type’ {aka ‘long unsigned int’} [-Wsign-compare]
  800 |     if(GMM_d_beta_[i]>=GMM_d_grps_.size()) error("Check Beta values");
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action WHOLEMOLECULES with label @3 : cannot understand the following words from the input line : REF0=5.3607,4.5911,3.1497, REF1=3.2439,3.3684,6.0308
[fv-az99-305:23166] *** Process received signal ***
[fv-az99-305:23166] Signal: Aborted (6)
[fv-az99-305:23166] Signal code:  (-6)
[fv-az99-305:23166] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc5dc404210]
[fv-az99-305:23166] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc5dc40418b]
[fv-az99-305:23166] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc5dc3e3859]
[fv-az99-305:23166] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc5dc66b951]
[fv-az99-305:23166] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc5dc67747c]
[fv-az99-305:23166] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc5dc6774e7]
[fv-az99-305:23166] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fc5dc6777ed]
[fv-az99-305:23166] [ 7] plumed_master(+0xf568)[0x5597e29c2568]
[fv-az99-305:23166] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc5dc3e50b3]
[fv-az99-305:23166] [ 9] plumed_master(+0xf79e)[0x5597e29c279e]
[fv-az99-305:23166] *** End of error message ***
</pre>
{% endraw %}
