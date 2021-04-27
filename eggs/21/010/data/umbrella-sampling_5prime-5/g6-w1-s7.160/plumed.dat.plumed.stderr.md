**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g6-w1-s7.160/plumed.dat   
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
[fv-az99-305:16437] *** Process received signal ***
[fv-az99-305:16437] Signal: Aborted (6)
[fv-az99-305:16437] Signal code:  (-6)
[fv-az99-305:16437] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f552991f210]
[fv-az99-305:16437] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f552991f18b]
[fv-az99-305:16437] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f55298fe859]
[fv-az99-305:16437] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5529b86951]
[fv-az99-305:16437] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5529b9247c]
[fv-az99-305:16437] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5529b924e7]
[fv-az99-305:16437] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f5529b92799]
[fv-az99-305:16437] [ 7] plumed(+0xf47d)[0x556d9b91e47d]
[fv-az99-305:16437] [ 8] plumed(+0x14004)[0x556d9b923004]
[fv-az99-305:16437] [ 9] plumed(+0xf698)[0x556d9b91e698]
[fv-az99-305:16437] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f55299000b3]
[fv-az99-305:16437] [11] plumed(+0xf76e)[0x556d9b91e76e]
[fv-az99-305:16437] *** End of error message ***
</pre>
{% endraw %}
