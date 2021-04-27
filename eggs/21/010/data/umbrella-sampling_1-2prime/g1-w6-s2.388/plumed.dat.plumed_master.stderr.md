**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w6-s2.388/plumed.dat   
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
[fv-az99-305:09681] *** Process received signal ***
[fv-az99-305:09681] Signal: Aborted (6)
[fv-az99-305:09681] Signal code:  (-6)
[fv-az99-305:09681] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f3d9f66a210]
[fv-az99-305:09681] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f3d9f66a18b]
[fv-az99-305:09681] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f3d9f649859]
[fv-az99-305:09681] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3d9f8d1951]
[fv-az99-305:09681] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3d9f8dd47c]
[fv-az99-305:09681] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3d9f8dd4e7]
[fv-az99-305:09681] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f3d9f8dd7ed]
[fv-az99-305:09681] [ 7] plumed_master(+0xf568)[0x558b10528568]
[fv-az99-305:09681] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f3d9f64b0b3]
[fv-az99-305:09681] [ 9] plumed_master(+0xf79e)[0x558b1052879e]
[fv-az99-305:09681] *** End of error message ***
</pre>
{% endraw %}
