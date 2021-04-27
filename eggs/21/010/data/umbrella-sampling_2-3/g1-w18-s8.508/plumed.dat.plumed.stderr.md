**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w18-s8.508/plumed.dat   
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
[fv-az99-305:10164] *** Process received signal ***
[fv-az99-305:10164] Signal: Aborted (6)
[fv-az99-305:10164] Signal code:  (-6)
[fv-az99-305:10164] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9e5225f210]
[fv-az99-305:10164] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9e5225f18b]
[fv-az99-305:10164] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9e5223e859]
[fv-az99-305:10164] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9e524c6951]
[fv-az99-305:10164] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9e524d247c]
[fv-az99-305:10164] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9e524d24e7]
[fv-az99-305:10164] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f9e524d2799]
[fv-az99-305:10164] [ 7] plumed(+0xf47d)[0x5574b5d1947d]
[fv-az99-305:10164] [ 8] plumed(+0x14004)[0x5574b5d1e004]
[fv-az99-305:10164] [ 9] plumed(+0xf698)[0x5574b5d19698]
[fv-az99-305:10164] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9e522400b3]
[fv-az99-305:10164] [11] plumed(+0xf76e)[0x5574b5d1976e]
[fv-az99-305:10164] *** End of error message ***
</pre>
{% endraw %}
