**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w49-s11.676/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:09604] *** Process received signal ***
[fv-az99-305:09604] Signal: Aborted (6)
[fv-az99-305:09604] Signal code:  (-6)
[fv-az99-305:09604] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f81b5584210]
[fv-az99-305:09604] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f81b558418b]
[fv-az99-305:09604] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f81b5563859]
[fv-az99-305:09604] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f81b57eb951]
[fv-az99-305:09604] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f81b57f747c]
[fv-az99-305:09604] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f81b57f74e7]
[fv-az99-305:09604] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f81b57f77ed]
[fv-az99-305:09604] [ 7] plumed_master(+0xf568)[0x55c06dfa6568]
[fv-az99-305:09604] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f81b55650b3]
[fv-az99-305:09604] [ 9] plumed_master(+0xf79e)[0x55c06dfa679e]
[fv-az99-305:09604] *** End of error message ***
</pre>
{% endraw %}
