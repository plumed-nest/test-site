**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w32-s8.004/plumed.dat   
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
[fv-az99-305:09164] *** Process received signal ***
[fv-az99-305:09164] Signal: Aborted (6)
[fv-az99-305:09164] Signal code:  (-6)
[fv-az99-305:09164] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2983559210]
[fv-az99-305:09164] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f298355918b]
[fv-az99-305:09164] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2983538859]
[fv-az99-305:09164] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f29837c0951]
[fv-az99-305:09164] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f29837cc47c]
[fv-az99-305:09164] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f29837cc4e7]
[fv-az99-305:09164] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f29837cc7ed]
[fv-az99-305:09164] [ 7] plumed_master(+0xf568)[0x55d95719e568]
[fv-az99-305:09164] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f298353a0b3]
[fv-az99-305:09164] [ 9] plumed_master(+0xf79e)[0x55d95719e79e]
[fv-az99-305:09164] *** End of error message ***
</pre>
{% endraw %}
