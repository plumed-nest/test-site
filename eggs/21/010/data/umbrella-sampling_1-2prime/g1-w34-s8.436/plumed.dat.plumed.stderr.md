**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w34-s8.436/plumed.dat   
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
[fv-az99-305:09205] *** Process received signal ***
[fv-az99-305:09205] Signal: Aborted (6)
[fv-az99-305:09205] Signal code:  (-6)
[fv-az99-305:09205] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f73b0c4b210]
[fv-az99-305:09205] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f73b0c4b18b]
[fv-az99-305:09205] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f73b0c2a859]
[fv-az99-305:09205] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f73b0eb2951]
[fv-az99-305:09205] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f73b0ebe47c]
[fv-az99-305:09205] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f73b0ebe4e7]
[fv-az99-305:09205] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f73b0ebe799]
[fv-az99-305:09205] [ 7] plumed(+0xf47d)[0x560c68cf147d]
[fv-az99-305:09205] [ 8] plumed(+0x14004)[0x560c68cf6004]
[fv-az99-305:09205] [ 9] plumed(+0xf698)[0x560c68cf1698]
[fv-az99-305:09205] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f73b0c2c0b3]
[fv-az99-305:09205] [11] plumed(+0xf76e)[0x560c68cf176e]
[fv-az99-305:09205] *** End of error message ***
</pre>
{% endraw %}
