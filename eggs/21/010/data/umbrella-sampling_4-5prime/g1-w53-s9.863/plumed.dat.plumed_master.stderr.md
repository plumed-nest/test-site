**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w53-s9.863/plumed.dat   
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
[fv-az99-305:13969] *** Process received signal ***
[fv-az99-305:13969] Signal: Aborted (6)
[fv-az99-305:13969] Signal code:  (-6)
[fv-az99-305:13969] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7efdec4c4210]
[fv-az99-305:13969] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7efdec4c418b]
[fv-az99-305:13969] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7efdec4a3859]
[fv-az99-305:13969] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7efdec72b951]
[fv-az99-305:13969] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7efdec73747c]
[fv-az99-305:13969] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7efdec7374e7]
[fv-az99-305:13969] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7efdec7377ed]
[fv-az99-305:13969] [ 7] plumed_master(+0xf568)[0x563f06009568]
[fv-az99-305:13969] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7efdec4a50b3]
[fv-az99-305:13969] [ 9] plumed_master(+0xf79e)[0x563f0600979e]
[fv-az99-305:13969] *** End of error message ***
</pre>
{% endraw %}
