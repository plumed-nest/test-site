**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w46-s11.028/plumed.dat   
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
[fv-az99-305:09531] *** Process received signal ***
[fv-az99-305:09531] Signal: Aborted (6)
[fv-az99-305:09531] Signal code:  (-6)
[fv-az99-305:09531] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f0f24892210]
[fv-az99-305:09531] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f0f2489218b]
[fv-az99-305:09531] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f0f24871859]
[fv-az99-305:09531] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f0f24af9951]
[fv-az99-305:09531] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f0f24b0547c]
[fv-az99-305:09531] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f0f24b054e7]
[fv-az99-305:09531] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f0f24b057ed]
[fv-az99-305:09531] [ 7] plumed_master(+0xf568)[0x55a62e476568]
[fv-az99-305:09531] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f0f248730b3]
[fv-az99-305:09531] [ 9] plumed_master(+0xf79e)[0x55a62e47679e]
[fv-az99-305:09531] *** End of error message ***
</pre>
{% endraw %}
