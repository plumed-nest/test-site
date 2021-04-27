**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w35-s8.652/plumed.dat   
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
[fv-az99-305:09237] *** Process received signal ***
[fv-az99-305:09237] Signal: Aborted (6)
[fv-az99-305:09237] Signal code:  (-6)
[fv-az99-305:09237] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1f86384210]
[fv-az99-305:09237] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f1f8638418b]
[fv-az99-305:09237] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1f86363859]
[fv-az99-305:09237] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1f865eb951]
[fv-az99-305:09237] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f1f865f747c]
[fv-az99-305:09237] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f1f865f74e7]
[fv-az99-305:09237] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f1f865f77ed]
[fv-az99-305:09237] [ 7] plumed_master(+0xf568)[0x559c21584568]
[fv-az99-305:09237] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f1f863650b3]
[fv-az99-305:09237] [ 9] plumed_master(+0xf79e)[0x559c2158479e]
[fv-az99-305:09237] *** End of error message ***
</pre>
{% endraw %}
