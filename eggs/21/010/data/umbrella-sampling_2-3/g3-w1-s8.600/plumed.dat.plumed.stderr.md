**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g3-w1-s8.600/plumed.dat   
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
[fv-az99-305:10795] *** Process received signal ***
[fv-az99-305:10795] Signal: Aborted (6)
[fv-az99-305:10795] Signal code:  (-6)
[fv-az99-305:10795] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fdae5b6b210]
[fv-az99-305:10795] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fdae5b6b18b]
[fv-az99-305:10795] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fdae5b4a859]
[fv-az99-305:10795] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fdae5dd2951]
[fv-az99-305:10795] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fdae5dde47c]
[fv-az99-305:10795] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fdae5dde4e7]
[fv-az99-305:10795] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fdae5dde799]
[fv-az99-305:10795] [ 7] plumed(+0xf47d)[0x55bd44fd747d]
[fv-az99-305:10795] [ 8] plumed(+0x14004)[0x55bd44fdc004]
[fv-az99-305:10795] [ 9] plumed(+0xf698)[0x55bd44fd7698]
[fv-az99-305:10795] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fdae5b4c0b3]
[fv-az99-305:10795] [11] plumed(+0xf76e)[0x55bd44fd776e]
[fv-az99-305:10795] *** End of error message ***
</pre>
{% endraw %}
