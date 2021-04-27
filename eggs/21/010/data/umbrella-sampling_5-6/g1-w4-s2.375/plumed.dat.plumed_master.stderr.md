**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w4-s2.375/plumed.dat   
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
[fv-az99-305:15192] *** Process received signal ***
[fv-az99-305:15192] Signal: Aborted (6)
[fv-az99-305:15192] Signal code:  (-6)
[fv-az99-305:15192] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5284224210]
[fv-az99-305:15192] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f528422418b]
[fv-az99-305:15192] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5284203859]
[fv-az99-305:15192] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f528448b951]
[fv-az99-305:15192] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f528449747c]
[fv-az99-305:15192] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f52844974e7]
[fv-az99-305:15192] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f52844977ed]
[fv-az99-305:15192] [ 7] plumed_master(+0xf568)[0x557c4fd03568]
[fv-az99-305:15192] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f52842050b3]
[fv-az99-305:15192] [ 9] plumed_master(+0xf79e)[0x557c4fd0379e]
[fv-az99-305:15192] *** End of error message ***
</pre>
{% endraw %}
