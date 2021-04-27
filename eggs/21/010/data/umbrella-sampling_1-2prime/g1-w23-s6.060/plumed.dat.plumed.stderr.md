**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w23-s6.060/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:08910] *** Process received signal ***
[fv-az99-305:08910] Signal: Aborted (6)
[fv-az99-305:08910] Signal code:  (-6)
[fv-az99-305:08910] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb4bc4d7210]
[fv-az99-305:08910] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb4bc4d718b]
[fv-az99-305:08910] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb4bc4b6859]
[fv-az99-305:08910] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb4bc73e951]
[fv-az99-305:08910] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb4bc74a47c]
[fv-az99-305:08910] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb4bc74a4e7]
[fv-az99-305:08910] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fb4bc74a799]
[fv-az99-305:08910] [ 7] plumed(+0xf47d)[0x56252fc0c47d]
[fv-az99-305:08910] [ 8] plumed(+0x14004)[0x56252fc11004]
[fv-az99-305:08910] [ 9] plumed(+0xf698)[0x56252fc0c698]
[fv-az99-305:08910] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb4bc4b80b3]
[fv-az99-305:08910] [11] plumed(+0xf76e)[0x56252fc0c76e]
[fv-az99-305:08910] *** End of error message ***
</pre>
{% endraw %}
