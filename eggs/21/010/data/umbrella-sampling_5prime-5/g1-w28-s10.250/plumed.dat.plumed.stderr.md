**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w28-s10.250/plumed.dat   
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
[fv-az99-305:16095] *** Process received signal ***
[fv-az99-305:16095] Signal: Aborted (6)
[fv-az99-305:16095] Signal code:  (-6)
[fv-az99-305:16095] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1f6b320210]
[fv-az99-305:16095] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f1f6b32018b]
[fv-az99-305:16095] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1f6b2ff859]
[fv-az99-305:16095] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1f6b587951]
[fv-az99-305:16095] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f1f6b59347c]
[fv-az99-305:16095] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f1f6b5934e7]
[fv-az99-305:16095] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f1f6b593799]
[fv-az99-305:16095] [ 7] plumed(+0xf47d)[0x55cc449e047d]
[fv-az99-305:16095] [ 8] plumed(+0x14004)[0x55cc449e5004]
[fv-az99-305:16095] [ 9] plumed(+0xf698)[0x55cc449e0698]
[fv-az99-305:16095] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f1f6b3010b3]
[fv-az99-305:16095] [11] plumed(+0xf76e)[0x55cc449e076e]
[fv-az99-305:16095] *** End of error message ***
</pre>
{% endraw %}
