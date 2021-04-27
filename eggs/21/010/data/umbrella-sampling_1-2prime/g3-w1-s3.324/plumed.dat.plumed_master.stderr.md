**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g3-w1-s3.324/plumed.dat   
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
[fv-az99-305:09804] *** Process received signal ***
[fv-az99-305:09804] Signal: Aborted (6)
[fv-az99-305:09804] Signal code:  (-6)
[fv-az99-305:09804] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f8e7cc13210]
[fv-az99-305:09804] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f8e7cc1318b]
[fv-az99-305:09804] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f8e7cbf2859]
[fv-az99-305:09804] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8e7ce7a951]
[fv-az99-305:09804] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f8e7ce8647c]
[fv-az99-305:09804] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f8e7ce864e7]
[fv-az99-305:09804] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f8e7ce867ed]
[fv-az99-305:09804] [ 7] plumed_master(+0xf568)[0x560426283568]
[fv-az99-305:09804] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f8e7cbf40b3]
[fv-az99-305:09804] [ 9] plumed_master(+0xf79e)[0x56042628379e]
[fv-az99-305:09804] *** End of error message ***
</pre>
{% endraw %}
