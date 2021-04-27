**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w22-s6.875/plumed.dat   
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
[fv-az99-305:14728] *** Process received signal ***
[fv-az99-305:14728] Signal: Aborted (6)
[fv-az99-305:14728] Signal code:  (-6)
[fv-az99-305:14728] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fab9e908210]
[fv-az99-305:14728] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fab9e90818b]
[fv-az99-305:14728] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fab9e8e7859]
[fv-az99-305:14728] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fab9eb6f951]
[fv-az99-305:14728] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fab9eb7b47c]
[fv-az99-305:14728] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fab9eb7b4e7]
[fv-az99-305:14728] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fab9eb7b7ed]
[fv-az99-305:14728] [ 7] plumed_master(+0xf568)[0x564945b29568]
[fv-az99-305:14728] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fab9e8e90b3]
[fv-az99-305:14728] [ 9] plumed_master(+0xf79e)[0x564945b2979e]
[fv-az99-305:14728] *** End of error message ***
</pre>
{% endraw %}
