**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2prime-2/g1-w1-s5.463/plumed.dat   
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
[fv-az99-305:10819] *** Process received signal ***
[fv-az99-305:10819] Signal: Aborted (6)
[fv-az99-305:10819] Signal code:  (-6)
[fv-az99-305:10819] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd319632210]
[fv-az99-305:10819] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd31963218b]
[fv-az99-305:10819] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd319611859]
[fv-az99-305:10819] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd319899951]
[fv-az99-305:10819] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd3198a547c]
[fv-az99-305:10819] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd3198a54e7]
[fv-az99-305:10819] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd3198a5799]
[fv-az99-305:10819] [ 7] plumed(+0xf47d)[0x5591b9a2947d]
[fv-az99-305:10819] [ 8] plumed(+0x14004)[0x5591b9a2e004]
[fv-az99-305:10819] [ 9] plumed(+0xf698)[0x5591b9a29698]
[fv-az99-305:10819] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd3196130b3]
[fv-az99-305:10819] [11] plumed(+0xf76e)[0x5591b9a2976e]
[fv-az99-305:10819] *** End of error message ***
</pre>
{% endraw %}
