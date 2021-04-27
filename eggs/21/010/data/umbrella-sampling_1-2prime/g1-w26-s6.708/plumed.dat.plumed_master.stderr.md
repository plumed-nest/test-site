**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w26-s6.708/plumed.dat   
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
[fv-az99-305:08991] *** Process received signal ***
[fv-az99-305:08991] Signal: Aborted (6)
[fv-az99-305:08991] Signal code:  (-6)
[fv-az99-305:08991] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa29c5ba210]
[fv-az99-305:08991] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa29c5ba18b]
[fv-az99-305:08991] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa29c599859]
[fv-az99-305:08991] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa29c821951]
[fv-az99-305:08991] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa29c82d47c]
[fv-az99-305:08991] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa29c82d4e7]
[fv-az99-305:08991] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fa29c82d7ed]
[fv-az99-305:08991] [ 7] plumed_master(+0xf568)[0x559aba3cc568]
[fv-az99-305:08991] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa29c59b0b3]
[fv-az99-305:08991] [ 9] plumed_master(+0xf79e)[0x559aba3cc79e]
[fv-az99-305:08991] *** End of error message ***
</pre>
{% endraw %}
