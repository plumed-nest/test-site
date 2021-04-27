**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w38-s7.588/plumed.dat   
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
[fv-az99-305:13553] *** Process received signal ***
[fv-az99-305:13553] Signal: Aborted (6)
[fv-az99-305:13553] Signal code:  (-6)
[fv-az99-305:13553] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fbb3435a210]
[fv-az99-305:13553] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fbb3435a18b]
[fv-az99-305:13553] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fbb34339859]
[fv-az99-305:13553] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fbb345c1951]
[fv-az99-305:13553] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fbb345cd47c]
[fv-az99-305:13553] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fbb345cd4e7]
[fv-az99-305:13553] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fbb345cd7ed]
[fv-az99-305:13553] [ 7] plumed_master(+0xf568)[0x556e58ad5568]
[fv-az99-305:13553] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fbb3433b0b3]
[fv-az99-305:13553] [ 9] plumed_master(+0xf79e)[0x556e58ad579e]
[fv-az99-305:13553] *** End of error message ***
</pre>
{% endraw %}
