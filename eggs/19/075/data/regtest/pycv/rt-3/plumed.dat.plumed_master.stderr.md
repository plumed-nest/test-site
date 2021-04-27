**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-3/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=distcv FUNCTION=cv
Maybe a missing space or a typo?
[fv-az99-305:30358] *** Process received signal ***
[fv-az99-305:30358] Signal: Aborted (6)
[fv-az99-305:30358] Signal code:  (-6)
[fv-az99-305:30358] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2438f74210]
[fv-az99-305:30358] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2438f7418b]
[fv-az99-305:30358] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2438f53859]
[fv-az99-305:30358] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f24391db951]
[fv-az99-305:30358] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f24391e747c]
[fv-az99-305:30358] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f24391e74e7]
[fv-az99-305:30358] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f24391e77ed]
[fv-az99-305:30358] [ 7] plumed_master(+0xf568)[0x5627688c8568]
[fv-az99-305:30358] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2438f550b3]
[fv-az99-305:30358] [ 9] plumed_master(+0xf79e)[0x5627688c879e]
[fv-az99-305:30358] *** End of error message ***
</pre>
{% endraw %}
