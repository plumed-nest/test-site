**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w26-s7.875/plumed.dat   
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
[fv-az99-305:14826] *** Process received signal ***
[fv-az99-305:14826] Signal: Aborted (6)
[fv-az99-305:14826] Signal code:  (-6)
[fv-az99-305:14826] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5cf47de210]
[fv-az99-305:14826] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5cf47de18b]
[fv-az99-305:14826] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5cf47bd859]
[fv-az99-305:14826] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5cf4a45951]
[fv-az99-305:14826] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5cf4a5147c]
[fv-az99-305:14826] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5cf4a514e7]
[fv-az99-305:14826] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f5cf4a517ed]
[fv-az99-305:14826] [ 7] plumed_master(+0xf568)[0x5556318b4568]
[fv-az99-305:14826] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5cf47bf0b3]
[fv-az99-305:14826] [ 9] plumed_master(+0xf79e)[0x5556318b479e]
[fv-az99-305:14826] *** End of error message ***
</pre>
{% endraw %}
