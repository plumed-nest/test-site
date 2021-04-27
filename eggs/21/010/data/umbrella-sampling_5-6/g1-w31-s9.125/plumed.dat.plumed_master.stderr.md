**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w31-s9.125/plumed.dat   
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
[fv-az99-305:14972] *** Process received signal ***
[fv-az99-305:14972] Signal: Aborted (6)
[fv-az99-305:14972] Signal code:  (-6)
[fv-az99-305:14972] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f56694c5210]
[fv-az99-305:14972] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f56694c518b]
[fv-az99-305:14972] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f56694a4859]
[fv-az99-305:14972] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f566972c951]
[fv-az99-305:14972] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f566973847c]
[fv-az99-305:14972] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f56697384e7]
[fv-az99-305:14972] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f56697387ed]
[fv-az99-305:14972] [ 7] plumed_master(+0xf568)[0x55da8c950568]
[fv-az99-305:14972] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f56694a60b3]
[fv-az99-305:14972] [ 9] plumed_master(+0xf79e)[0x55da8c95079e]
[fv-az99-305:14972] *** End of error message ***
</pre>
{% endraw %}
