**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w29-s7.356/plumed.dat   
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
[fv-az99-305:09066] *** Process received signal ***
[fv-az99-305:09066] Signal: Aborted (6)
[fv-az99-305:09066] Signal code:  (-6)
[fv-az99-305:09066] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f0902102210]
[fv-az99-305:09066] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f090210218b]
[fv-az99-305:09066] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f09020e1859]
[fv-az99-305:09066] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f0902369951]
[fv-az99-305:09066] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f090237547c]
[fv-az99-305:09066] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f09023754e7]
[fv-az99-305:09066] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f09023757ed]
[fv-az99-305:09066] [ 7] plumed_master(+0xf568)[0x557be123d568]
[fv-az99-305:09066] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f09020e30b3]
[fv-az99-305:09066] [ 9] plumed_master(+0xf79e)[0x557be123d79e]
[fv-az99-305:09066] *** End of error message ***
</pre>
{% endraw %}
