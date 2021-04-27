**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w43-s8.346/plumed.dat   
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
[fv-az99-305:13700] *** Process received signal ***
[fv-az99-305:13700] Signal: Aborted (6)
[fv-az99-305:13700] Signal code:  (-6)
[fv-az99-305:13700] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f83e23a0210]
[fv-az99-305:13700] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f83e23a018b]
[fv-az99-305:13700] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f83e237f859]
[fv-az99-305:13700] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f83e2607951]
[fv-az99-305:13700] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f83e261347c]
[fv-az99-305:13700] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f83e26134e7]
[fv-az99-305:13700] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f83e26137ed]
[fv-az99-305:13700] [ 7] plumed_master(+0xf568)[0x5637dae30568]
[fv-az99-305:13700] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f83e23810b3]
[fv-az99-305:13700] [ 9] plumed_master(+0xf79e)[0x5637dae3079e]
[fv-az99-305:13700] *** End of error message ***
</pre>
{% endraw %}
