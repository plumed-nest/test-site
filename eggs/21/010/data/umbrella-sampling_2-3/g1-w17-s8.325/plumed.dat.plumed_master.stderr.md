**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w17-s8.325/plumed.dat   
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
[fv-az99-305:10147] *** Process received signal ***
[fv-az99-305:10147] Signal: Aborted (6)
[fv-az99-305:10147] Signal code:  (-6)
[fv-az99-305:10147] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5bb52ae210]
[fv-az99-305:10147] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5bb52ae18b]
[fv-az99-305:10147] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5bb528d859]
[fv-az99-305:10147] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5bb5515951]
[fv-az99-305:10147] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5bb552147c]
[fv-az99-305:10147] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5bb55214e7]
[fv-az99-305:10147] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f5bb55217ed]
[fv-az99-305:10147] [ 7] plumed_master(+0xf568)[0x559261942568]
[fv-az99-305:10147] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5bb528f0b3]
[fv-az99-305:10147] [ 9] plumed_master(+0xf79e)[0x55926194279e]
[fv-az99-305:10147] *** End of error message ***
</pre>
{% endraw %}
